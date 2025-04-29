> ⚠️ **Caution:** Not Implemented

WeatherEye Monitor uses Prometheus to scrape, store and query time-series metric from the WeatherEye applications and infrastructure. Loki collects and indexes logs using the same labels (but without costly full-text indexing), making log streams easy to filter and correlate and Grafana ties everything together by providing a unified UI with dashboards, chart metrics, spin up alerts on Prometheus data and drill directly into the matching Loki log lines—letting you seamlessly explore both metrics and logs in one place.

Sentry (deployed on [[WeatherEye Cloud]]) is an error tracking system that allows WeatherEye to track any errors that are raised in applications during production use in order to provide feedback to developer teams.

---
*Status:*
- Currently bundled as part of [[WeatherEye Broker]] (using wis2box)

*Powered by:*
- [Grafana](https://github.com/grafana/loki) (AGPL3) Monitoring dashboards
- [Loki](https://github.com/grafana/loki) (AGPL3) Log storage
- [Prometheus](https://github.com/prometheus/prometheus) (Apache 2.0) Metrics collection
- [Sentry](https://github.com/getsentry/sentry) ([FSL-1.1-Apache-2.0](https://www.tldrlegal.com/license/functional-source-license-fsl)) Live error tracking ([[WeatherEye Cloud]] only)
