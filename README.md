# crowdsec-library

Public CrowdSec extras for PortaDesign — a small **delta** User-Agent list that is not in the CrowdSec Hub defaults.

Hub `crowdsecurity/http-bad-user-agent` already covers scanners and many scrapers. This repo only adds User-Agents that spam our sites and are missing from that list. Do not duplicate Hub entries.

The leaky scenario that consumes this list (`porta/http-unwanted-bots`) lives in the Dokploy Ansible role in [`docker-library`](https://github.com/portadesign/docker-library) and fetches the file at runtime via `source_url`.

## Contents

| Path | Purpose |
|------|---------|
| [`web/unwanted-bots.regex.txt`](web/unwanted-bots.regex.txt) | Regex list of unwanted User-Agents |
