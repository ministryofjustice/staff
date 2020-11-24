# Ministry of Justice Official Staff Infrastructure and Devices

## About this repository
Repositories used for MoJ Official infrastructure and staff device provision and management.
### Environment Deployments
- https://github.com/ministryofjustice/pttp-shared-services-infrastructure - to create infrastructure from the main AWS shared account into Dev, Prep and Production via AWS CodePipelines
### Infrastrastrcuture Monitoring and Alerting
- [IMA Platform](https://github.com/ministryofjustice/staff-infrastructure-monitoring) - to monitor PTTP infrastructure and physical devices
- [Data Source Configuration](https://github.com/ministryofjustice/staff-infrastructure-monitoring-datasource-config) - to provision data sources for the IMA Platform
- [SNMP Exporter](https://github.com/ministryofjustice/staff-infrastructure-monitoring-snmpexporter) - to scrape data from physical devices (Docker image)
- [Blackbox Exporter](https://github.com/ministryofjustice/staff-infrastructure-monitoring-blackbox-exporter) - to probe endpoints over HTTP, HTTPS, DNS, TCP and ICMP (Docker image)
- [Metric Aggregation Server](https://github.com/ministryofjustice/staff-infrastructure-metric-aggregation-server) - to pull data from the SNMP exporter (Docker image)

DHCP / DNS
- https://github.com/ministryofjustice/staff-device-dhcp-server - creates the AWS ECR container image for ISC Kea
- https://github.com/ministryofjustice/staff-device-dns-dhcp-admin - frontend for managing staff device site dhcp dns
- https://github.com/ministryofjustice/staff-device-dns-dhcp-infrastructure - code to build the aws infrastructure for the DNS and DHCP platform

Security Log Shipping
- https://github.com/ministryofjustice/staff-device-logging-infrastructure - log shipping infrastructure
- https://github.com/ministryofjustice/staff-device-logging-syslog-to-cloudwatch - syslog to aws cloudwatch

Palo Alto Transit Gateway deployment
- https://github.com/ministryofjustice/deployment-GlobalProtect - global protec rotect firewall deployment
- https://github.com/ministryofjustice/deployment-tgw - aws transit gateway deployment
- https://github.com/ministryofjustice/terraform-aws-step_function_globalprotect
- https://github.com/ministryofjustice/terraform-panorama-config - Panorama Config written in Terraform
- https://github.com/ministryofjustice/deployment-PSN - Public Services Network connection in AWS, connected via Lumen (previously CenturyLink)

Azure Landing Zone
- https://github.com/ministryofjustice/staff-infrastructure-azure-landing-zone

Device Management
- https://github.com/ministryofjustice/staff-device-management-windows10-configuration
- https://github.com/ministryofjustice/staff-device-management-windows10-apps
- https://github.com/ministryofjustice/staff-device-management-ios-configuration
- https://github.com/ministryofjustice/staff-device-management-ios-apps
- https://github.com/ministryofjustice/staff-device-management-virtualdesktop
- https://github.com/ministryofjustice/moj-official-intune

Certificate Services 
- https://github.com/ministryofjustice/staff-infrastructure-certificate-services - Public Key Infrastructure for devices and users.