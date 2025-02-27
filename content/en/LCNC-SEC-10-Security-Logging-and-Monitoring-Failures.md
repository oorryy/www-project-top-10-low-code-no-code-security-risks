# LCNC-SEC-10: Security Logging and Monitoring Failures

## Risk Rating [*](https://owasp.org/www-project-top-ten/2017/Note_About_Risks)

| Prevalence | Detectability | Exploitability | Technical Impact |
| --- | --- | --- | --- |
| 2 | 2 | 3 | 2 |

## The Gist

No-code/low-code applications often lack a comprehensive audit trail, produce none or insufficient logs, and fail to scrub sensitive data from logs.

## Description

No-code/low-code applications often rely on vendors to generate logs and monitoring data.
In many cases, logs are either insufficient or not being collected, impeding security investigations and failing to satisfy compliance requirements.
Applications often lack a comprehensive audit trail, preventing change management processes and inquires.

Furthermore, many native log streams mix between application logs, metrics and sensitive data being passed through the application.
In many platforms and by default, logs will contain actual data points used by the application.

## Example Attack Scenarios

### Scenario #1

TBD

### Scenario #2

TBD

## How to Prevent

- Leverage platform built-in capabilities to collect user access and platform audit logs.
- Where applicable, instrument applications with logging mechanisms to provide extra visibility.
- Ensure logs are not contaminated with sensitive data by configuring the platform to avoid logging raw application data.

## References

- [A08:2021 – Software and Data Integrity Failures, OWASP Top 10](https://owasp.org/Top10/A08_2021-Software_and_Data_Integrity_Failures/)