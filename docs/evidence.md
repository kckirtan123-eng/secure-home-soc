# Evidence register

**Baseline date:** 23–24 September 2026. These observations are historical; a current system state requires a fresh check.

| ID | Claim | Observation | Scope and limit |
| --- | --- | --- | --- |
| E01 | Monitoring services installed and running | Ubuntu host reported Wazuh manager, indexer, dashboard and Filebeat enabled and active; Wazuh components were version 4.14.7 | A running service is not proof of every function or future uptime |
| E02 | Windows agent connected | Dashboard displayed the Windows 11 agent as Active with a recent keep-alive on 24 September | A historical status is not a current connection test |
| E03 | A Windows event produced a visible Wazuh alert | Windows Event ID `4634` was visible as Wazuh rule `67023`, severity level `3` | This verifies one alert path; it does not validate all event channels or detection rules |
| E04 | Benign Application event created locally | Windows `eventcreate` succeeded; `Get-WinEvent` showed Event ID `901` | No matching Threat Hunting alert appeared, and all-event archives were disabled. Manager ingestion remains unverified |
| E05 | Dashboard reachable to a home-network client | HTTPS redirected to the login page and the user reported a successful sign-in | Management access from other network locations was not tested |
| E06 | Capacity measured once | RAM, swap, root filesystem and volume-group capacity were recorded | A seven-day trend and retention policy have not been completed |

## Evidence to add

- A redacted screenshot showing the enrolled endpoint and observation date.
- A redacted alert detail for Windows Event ID `4634` and rule `67023`.
- A redacted source-side Event Viewer or PowerShell view for test Event ID `901`, clearly labeled *local event only*.
- A dated result for each future test, including failures and recovery steps.

No images are included in this initial public version because screenshots with identifying logs and access details have not yet been reviewed for publication.
