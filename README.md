# Windows-Twerks

## Overview

**Sysmon (System Monitor)** is a Windows system service and device driver that logs system activity to the Windows Event Log. It is a part of the Sysinternals Suite by Microsoft. Sysmon provides detailed information about process creation, network connections, file creation time, and other system activities that help in monitoring and troubleshooting.

By logging detailed event information about system activity, Sysmon enables IT administrators and security teams to identify malicious activity, troubleshoot issues, and enhance security.

## SysmonConfig.xml Update

The `sysmonconfig.xml` file included in this project has been updated to improve its effectiveness in monitoring systems. This updated configuration has been specially tailored to handle remote requests targeting servers, enhancing the monitoring capabilities of your Sysmon installation.

### Key Updates:
- **Remote Request Handling**: The `sysmonconfig.xml` configuration now includes enhanced filtering and event generation to capture potentially malicious remote requests targeting your servers.
- **Security Improvements**: Additional logging and event filtering have been added to detect suspicious network activities, particularly those that originate from outside the local network.

This configuration helps strengthen your system’s defenses against unauthorized access and ensures better monitoring of any remote threats.

---

## Installation

1. Download and extract the Sysmon files in this repository.
2. Replace the default `sysmonconfig.xml` with the updated configuration provided.
3. Run Sysmon with the updated config to start monitoring.

```bash
sysmon -accepteula -c sysmonconfig.xml

