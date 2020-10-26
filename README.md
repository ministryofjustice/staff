# Ministry of Justice Official Staff Infrastructure and Devices

## About this repository
Below are the repositories we use for MoJ Official infrastructure and staff devices
### Core Repositories
| Name                   | Description                                                                  | Link                                                        |
|------------------------|------------------------------------------------------------------------------|-------------------------------------------------------------|
Infrastructure Monitoring and Alerting Platoform | Our repository for monitoring the health of MoJO services| https://github.com/ministryofjustice/staff-infrastructure-monitoring-datasource-config |

- [IMA Platform](https://github.com/ministryofjustice/staff-infrastructure-monitoring) - to monitor PTTP infrastructure and physical devices
- [Data Source Configuration](https://github.com/ministryofjustice/staff-infrastructure-monitoring-datasource-config) - to provision data sources for the IMA Platform
- [SNMP Exporter](https://github.com/ministryofjustice/staff-infrastructure-monitoring-snmpexporter) - to scrape data from physical devices (Docker image)
- [Blackbox Exporter](https://github.com/ministryofjustice/staff-infrastructure-monitoring-blackbox-exporter) - to probe endpoints over HTTP, HTTPS, DNS, TCP and ICMP.s (Docker image)
- [Metric Aggregation Server](https://github.com/ministryofjustice/staff-infrastructure-metric-aggregation-server) - to pull data from the SNMP exporter (Docker image)

DHCP / DNS
- https://github.com/ministryofjustice/staff-device-dhcp-server
- https://github.com/ministryofjustice/staff-device-dns-dhcp-admin
- https://github.com/ministryofjustice/staff-device-dns-dhcp-infrastructure


Security Log Shipping
- https://github.com/ministryofjustice/staff-device-logging-infrastructure
- https://github.com/ministryofjustice/staff-device-logging-syslog-to-cloudwatch
- https://github.com/ministryofjustice/staff-device-logging-dns-dhcp-integration-tests
- https://github.com/ministryofjustice/pttp-shared-services-infrastructure

Palo Alto Transit Gateway deployment
- https://github.com/ministryofjustice/deployment-GlobalProtect
- https://github.com/ministryofjustice/deployment-tgw
- https://github.com/ministryofjustice/terraform-aws-step_function_globalprotect


Azure Landing Zone
- https://github.com/ministryofjustice/staff-infrastructure-azure-landing-zone

Device Management
- https://github.com/ministryofjustice/staff-device-management-ios-apps
- https://github.com/ministryofjustice/staff-device-management-virtualdesktop
- https://github.com/ministryofjustice/moj-official-intune

Certificate Services 
- https://github.com/ministryofjustice/staff-infrastructure-certificate-services

## Other Useful Repositories
