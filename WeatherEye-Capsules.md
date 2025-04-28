Reusable framework-agnostic processes and components

A capsule encapsulates:
- One or more OGC API - Process(es)
- One or more W3C Web Component(s)
- Gherkin tests for process(es) and component(s)
- Documentation for process(es), component(s), tests and also the use of the process(es) and component(s) together

A capsule process can be used in automation (e.g. DCPS ETL) or it can be access through OGC API to communicate with corresponding capsule components.

A capsule component is expected to be framework-agnostic and be suitable for inclusion in multiple systems including WeatherEye CDMS (VueJS), WeatherEye Forecaster Desktop (ReactJS) and other places. WeatherEye CMS uses ClimWeb (Wagtail/Django) where capsule components can be added to CMS pages using Wagtail blocks.

Development of capsules is intended to be:
- Documentation first
- TDD Gherkin features using Behave for process testing and Cucumber for component testing
- Framework-agnostic reusable Components are likely to be developed with StencilJS

An aspiration of WeatherEye is to extend pygeoapi to allow both the process(es) and the corresponding component(s) to both be registered. This will allow users to interact with the calsule process(es) APIs via the capsule components.