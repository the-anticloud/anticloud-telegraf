# TELEGRAF

![licence](https://img.shields.io/badge/licence-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![checks](https://img.shields.io/badge/checks-16_PASS-brightgreen)

> Governed Anticloud packaging of the upstream project `TELEGRAF` in category **FACTORY_MANUFACTURING**. 16/16 checks PASS (measured). Every number below traces to a named file + run stamp; nothing is borrowed from other projects.

**Upstream:** https://github.com/influxdata/telegraf · **Upstream pin:** `f361ad4aa98d63deb0baffcb16fbaf058189da48` · **Category:** FACTORY_MANUFACTURING · **Vendor:** Anticloud FZ LLE · **Licence:** MIT

---

## What This Project Does

# ![tiger](assets/TelegrafTigerSmall.png "tiger") Telegraf

[![GoDoc](https://img.shields.io/badge/doc-reference-00ADD8.svg?logo=go)](https://godoc.org/github.com/influxdata/telegraf)
[![Docker pulls](https://img.shields.io/docker/pulls/library/telegraf.svg)](https://hub.docker.com/_/telegraf/)
[![Go Report Card](https://goreportcard.com/badge/github.com/influxdata/telegraf)](https://goreportcard.com/report/github.com/influxdata/telegraf)
[![Circle CI](https://circleci.com/gh/influxdata/telegraf.svg?style=svg)](https://circleci.com/gh/influxdata/telegraf)

Telegraf is an agent for collecting, processing, aggregating, and writing
metrics, logs, and other arbitrary data.

* Offers a comprehensive suite of over 300 plugins, covering a wide range of
  functionalities including system monitoring, cloud services, and message
  passing
* Enables the integration of user-defined code to collect, transform, and
  transmit data efficiently
* Compiles into a standalone static binary without any external dependencies,
  ensuring a streamlined deployment process
* Utilizes TOML for configuration, providing a user-friendly and unambiguous
  setup experience
* Developed with contributions from a diverse community of over 1,200
  contributors

Users can choose plugins from a wide range of topics, including but not limited
to:

* Devices: [OPC UA][], [Modbus][]
* Logs: [File][], [Tail][], [Directory Monitor][]
* Messaging: [AMQP][], [Kafka][], [MQTT][]
* Monitoring: [OpenTelemetry][], [Prometheus][]
* Networking: [Cisco TelemetryMDT][], [gNMI][]
* System monitoring: [CPU][], [Memory][], [Disk][], [Network][], [SMART][],
  [Docker][], [Nvidia SMI][], etc.
* Universal: [Exec][], [HTTP][], [HTTP Listener][], [SNMP][], [SQL][]
* Windows: [Event Log][], [Management Instrumentation][],
  [Performance Counters][]

## 🔨 Installation

For binary builds, Docker images, RPM & DEB packages, and other builds of
Telegraf, please see the [install guide](/docs/INSTALL_GUIDE.md).

See the [releases documentation](/docs/RELEASES.md) for details on versioning
and when releases are made.

## 💻 Usage

Users define a TOML configuration with the plugins and settings they wish to
use, then pass that configuration to Telegraf. The Telegraf agent then
collects data from inputs at each interval and sends data to outputs at each
flush interval.

For a basic walkthrough see [quick start](/docs/QUICK_START.md).

## 📖 Documentation

For a full list of documentation including tutorials, reference and other
material, start with the [/docs directory](/docs/README.md).

Additionally, each plugin has its own README that includes details about how to
configure, use, and sometimes debug or troubleshoot. Look under the
[/plugins directory](/plugins/) for specific plugins.

Here are some commonly used documents:

* [Changelog](/CHANGELOG.md)
* [Configuration](/docs/CONFIGURATION.md)
* [FAQ](/docs/FAQ.md)
* [Releases](https://github.com/influxdata/telegraf/releases)
* [Security](/SECURITY.md)

## ❤️ Contribute

[![Contribute](https://img.shields.io/badge/contribute-to_telegraf-blue.svg?logo=influxdb)](https://github.com/influxdata/telegraf/blob/master/CONTRIBUTING.md)

We love our community of over 1,200 contributors! Many of the plugins included
in Telegraf were originally contributed by community members. Check out
our [contributing guide](CONTRIBUTING.md) if you are interested in helping out.
Also, join us on our [Community Slack](https://influxdata.com/slack) or
[Community Forums](https://community.influxdata.com/) if you have questions or
comments for our engineering teams.

If you are completely new to Telegraf and InfluxDB, you can also enroll for free
at [InfluxDB university](https://www.influxdata.com/university/) to take courses
to learn more.

## ℹ️ Support

[![Slack](https://img.shields.io/badge/slack-join_chat-blue.svg?logo=slack)](https://www.influxdata.com/slack)
[![Forums](https://img.shields.io/badge/discourse-join_forums-blue.svg?logo=discourse)](https://community.influxdata.com/)

Please use the [Community Slack](https://influxdata.com/slack) or
[Community Forums](https://community.influxdata.com/) if you have questions or
comments for our engineering teams. GitHub issues are limited to actual issues
and feature requests only.

## 📜 License

[![MIT](https://img.shields.io/badge/license-MIT-blue)](https://github.com/influxdata/telegraf/blob/master/LICENSE)

[OPC UA]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/opcua
[Modbus]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/modbus
[File]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/file
[Tail]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/tail
[Directory Monitor]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/directory_monitor
[AMQP]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/amqp_consumer
[Kafka]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/kafka_consumer
[MQTT]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/mqtt_consumer
[OpenTelemetry]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/opentelemetry
[Prometheus]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/prometheus
[Cisco TelemetryMDT]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/cisco_telemetry_mdt
[gNMI]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/gnmi
[CPU]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/cpu
[Memory]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/mem
[Disk]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/disk
[Network]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/net
[SMART]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/smartctl
[Docker]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/docker
[Nvidia SMI]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/nvidia_smi
[Exec]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/exec
[HTTP]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/http
[HTTP Listener]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/http_listener_v2
[SNMP]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/snmp
[SQL]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/sql
[Event Log]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/win_eventlog
[Management Instrumentation]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/win_wmi
[Performance Counters]: https://github.com/influxdata/telegraf/tree/master/plugins/inputs/win_perf_counters

---

## Installation

* Developed with contributions from a diverse community of over 1,200
  contributors

Users can choose plugins from a wide range of topics, including but not limited
to:

* Devices: [OPC UA][], [Modbus][]
* Logs: [File][], [Tail][], [Directory Monitor][]
* Messaging: [AMQP][], [Kafka][], [MQTT][]
* Monitoring: [OpenTelemetry][], [Prometheus][]
* Networking: [Cisco TelemetryMDT][], [gNMI][]
* System monitoring: [CPU][], [Memory][], [Disk][], [Network][], [SMART][],
  [Docker][], [Nvidia SMI][], etc.
* Universal: [Exec][], [HTTP][], [HTTP Listener][], [SNMP][], [SQL][]
* Windows: [Event Log][], [Management Instrumentation][],
  [Performance Counters][]

## Usage

transmit data efficiently
* Compiles into a standalone static binary without any external dependencies,
  ensuring a streamlined deployment process
* Utilizes TOML for configuration, providing a user-friendly and unambiguous
  setup experience
* Developed with contributions from a diverse community of over 1,200
  contributors

Users can choose plugins from a wide range of topics, including but not limited
to:

* Devices: [OPC UA][], [Modbus][]
* Logs: [File][], [Tail][], [Directory Monitor][]
* Messaging: [AMQP][], [Kafka][], [MQTT][]
* Monitoring: [OpenTelemetry][], [Prometheus][]
* Networking: [Cisco TelemetryMDT][], [gNMI][]
* System monitoring: [CPU][], [Memory][], [Disk][], [Network][], [SMART][],
  [Docker][], [Nvidia SMI][], etc.
* Universal: [Exec][], [HTTP][], [HTTP Listener][], [SNMP][], [SQL][]
* Windows: [Event Log][], [Management Instrumentation][],
  [Performance Counters][]

## API

[![Docker pulls](https://img.shields.io/docker/pulls/library/telegraf.svg)](https://hub.docker.com/_/telegraf/)
[![Go Report Card](https://goreportcard.com/badge/github.com/influxdata/telegraf)](https://goreportcard.com/report/github.com/influxdata/telegraf)
[![Circle CI](https://circleci.com/gh/influxdata/telegraf.svg?style=svg)](https://circleci.com/gh/influxdata/telegraf)

Telegraf is an agent for collecting, processing, aggregating, and writing
metrics, logs, and other arbitrary data.

* Offers a comprehensive suite of over 300 plugins, covering a wide range of
  functionalities including system monitoring, cloud services, and message
  passing
* Enables the integration of user-defined code to collect, transform, and
  transmit data efficiently
* Compiles into a standalone static binary without any external dependencies,
  ensuring a streamlined deployment process
* Utilizes TOML for configuration, providing a user-friendly and unambiguous
  setup experience
* Developed with contributions from a diverse community of over 1,200
  contributors

Users can choose plugins from a wide range of topics, including but not limited
to:

* Devices: [OPC UA][], [Modbus][]
* Logs: [File][], [Tail][], [Directory Monitor][]
* Messaging: [AMQP][], [Kafka][], [MQTT][]
* Monitoring: [OpenTelemetry][], [Prometheus][]
* Networking: [Cisco TelemetryMDT][], [gNMI][]
* System monitoring: [CPU][], [Memory][], [Disk][], [Network][], [SMART][],
  [Docker][], [Nvidia SMI][], etc.
* Universal: [Exec][], [HTTP][], [HTTP Listener][], [SNMP][], [SQL][]
* Windows: [Event Log][], [Management Instrumentation][],
  [Performance Counters][]

## Dependencies

| Metric | Value |
|--------|-------|
| Files | unknown |
| Lines of Code | unknown |
| Dependencies | unknown |
| Upstream license (harvested) | MIT |
| Overlay license | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

setup experience
* Developed with contributions from a diverse community of over 1,200
  contributors

Users can choose plugins from a wide range of topics, including but not limited
to:

* Devices: [OPC UA][], [Modbus][]
* Logs: [File][], [Tail][], [Directory Monitor][]
* Messaging: [AMQP][], [Kafka][], [MQTT][]
* Monitoring: [OpenTelemetry][], [Prometheus][]
* Networking: [Cisco TelemetryMDT][], [gNMI][]
* System monitoring: [CPU][], [Memory][], [Disk][], [Network][], [SMART][],
  [Docker][], [Nvidia SMI][], etc.
* Universal: [Exec][], [HTTP][], [HTTP Listener][], [SNMP][], [SQL][]
* Windows: [Event Log][], [Management Instrumentation][],
  [Performance Counters][]

## Contributing

# Contributing to Telegraf

There are many ways to get involved in the Telegraf project! From opening
issues, creating pull requests, to joining the conversation in Slack. We would
love to see you contribute your expertise and join our community. To get started
review this document to learn best practices.

![tiger](assets/GopherAndTiger.png "tiger")

## Opening Issues

### Bug reports

Before you file an issue, please search existing issues in case it has already
been filed, or perhaps even fixed. If you file an issue, please ensure you
include all the requested details (e.g. Telegraf config, logs, platform, etc.)

Please note that issues are not the place to file general support requests such
as "How do I use the mongoDB plugin?" Questions of this nature should be sent
to the [Community Slack][slack] or [Community Page][forum], not filed as issues.

[slack]: https://influxdata.com/slack
[forum]: https://community.influxdata.com/

### Feature requests

We really like to receive feature requests as it helps us prioritize our work.
Before you file a feature request, please search existing issues, you can filter
issues that have the label `feature request`. Please be clear about your
requirements and goals, help us to understand what you would like to see added
to Telegraf with examples and the reasons why it is important to you. If you
find your feature request already exists as a Github issue please indicate your
support for that feature by using the "thumbs up" reaction.

### Support questions

We recommend posting support questions in our [Community Slack][slack] or
[Community Page][forum], we have a lot of talented community members there who
could help answer your question more quickly.

## Contributing code

### AI Generated Code

We currently cannot accept AI generated code contributions. Code contributed
should be your own per the CLA.

### Creating a pull request

1. [Sign the CLA][cla].
2. Open a [new issue][] to discuss the changes you would like to make.  This is
   not strictly required but it may help reduce the amount of rework you need
   to do later.
3. Make changes or write plugin using the guidelines in the following
   documents:
   - [Input Plugins][inputs]
   - [Processor Plugins][processors]
   - [Aggregator Plugins][aggregators]
   - [Output Plugins][outputs]
4. Ensure you have added proper unit tests and documentation.
5. Open a new [pull request][].
6. The pull request title needs to follow [conventional commit format][semcommit]

> [!NOTE]
> If you have a pull request with only one commit, then that commit needs to
> follow the conventional commit format or the `Semantic Pull Request` check
> will fail. This is because github will use the pull request title if there are
> multiple commits, but if there is only one commit it will use it instead.

[semcommit]: https://www.conventionalcommits.org/en/v1.0.0/#summary

### When will your contribution get released?

We have two kinds of releases: patch releases, which happen ev

## License

Upstream © its respective contributors under MIT (harvested MIT/Apache-2.0/BSD source; see `UPSTREAM_CLONE/LICENSE`). This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- **project:** https://github.com/influxdata/telegraf
- **Pinned SHA:** `f361ad4aa98d63deb0baffcb16fbaf058189da48`
- **source:** `UPSTREAM_CLONE/` (pinned at the SHA above)
- **Upstream README source:** `UPSTREAM_CLONE/README.md`

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`923ceedff43e67cfbf175d1e7bcb193b0dda1f988f4b49b772e765117ff1e2c2`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

