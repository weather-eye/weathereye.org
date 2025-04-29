> ⚠️ **Caution:** Not Implemented

Initial backup is implemented at the server level with Proxmox Backup client installed in each VM.

In the future, additional more targeted backup tools will also be provided for [[WeatherEye RDBMS]], [[WeatherEye Filestore]] and also the capture the configuration (state) of applications without a full-server backup.

CAUTION: Installing Proxmox Backup Client in a Cloud environments may result in large data transfer out fees unless [[WeatherEye Backup]] is installed in the same network.

---
*Status:*
- Available, but not yet integrated into WeatherEye

*Powered by:*
- [Proxmox backup server](https://github.com/proxmox/proxmox-backup) (AGPL3)