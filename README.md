# crowdsec-library

Public CrowdSec extras for PortaDesign — small **delta** lists and scenarios that are not in the CrowdSec Hub defaults.

Hub `crowdsecurity/http-bad-user-agent` already covers scanners and many scrapers. This repo only adds User-Agents that spam our sites and are missing from that list. Do not duplicate Hub entries.

## Contents

| Path | Purpose |
|------|---------|
| [`web/unwanted-bots.regex.txt`](web/unwanted-bots.regex.txt) | Regex list of unwanted User-Agents |
| [`scenarios/porta/http-unwanted-bots.yaml`](scenarios/porta/http-unwanted-bots.yaml) | Leaky scenario (~5 req/min → remediation) |

The regex list is fetched at runtime through the scenario `source_url`.
