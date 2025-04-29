> ⚠️ **Caution:** Not Implemented

WeatherEye Controller (wxc) is a single codebase, implemented using the Python Textualize package, that provides a Command Line Interface (CLI), Text User Interface (TUI) and Web UI for [provisioning](https://www.redhat.com/en/topics/automation/what-is-provisioning) (Terraform), [orchestrating](https://www.redhat.com/en/topics/automation/what-is-orchestration) (Ansible) and configuring WeatherEye software on Linux servers.

[[wxc]]: Controller command line tool / TUI (used by [[WeatherEye OS]] and [[WeatherEye Setup]])

wxc is aware of environments that it can install to including:
1. Provisioning
  - Infrastructure Providers (e.g. Locally [Proxmox](https://github.com/Telmate/terraform-provider-proxmox) or [VMWare](https://registry.terraform.io/providers/hashicorp/vsphere/latest). Remote: Amazon Web Services, Google Cloud Platform etc. see [supported providers](https://registry.terraform.io/search/providers)
2. Orchestrating
  - Linux servers (VMs, cloud instances) 
3. Configuration Management
  - WeatherEye Admin Django project (determining which Django apps are running in a single Django instance)
  - Other WeatherEye application configurations

The command line tool includes the following modules which can also be accessed through WeatherEye Admin:
- [[wx-upgrade]]
- [[wx-rollback]]
- [[wx-backup]]

---
*Powered by:*
- [Terraform](https://developer.hashicorp.com/terraform) for [server provisioning](https://www.redhat.com/en/topics/automation/what-is-provisioning)
- [Ansible](https://docs.ansible.com/) for [server orchestration](https://www.redhat.com/en/topics/automation/what-is-orchestration)
- [Textualize](https://www.textualize.io/) - An application framework for CLI, TUI and WebUI in a single codebase
- [pipx](https://pipx.pypa.io/stable/) - A way to install Python CLI's as a tool in a contained environment
