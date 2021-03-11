# Ministry of Justice Official - Staff Infrastructure and Devices

## About this repository

Lists repositories used of MoJ Official infrastructure, staff device configuration, provisioning and management. Terraform is used to deploy most services to public cloud services.

### High Level Diagram

![High Level Diagram](diagrams/hld.png)
[image source](diagrams/hld-diagrams.drawio)

### Amazon Web Services Deployment

- [Shared Services Infrastructure](https://github.com/ministryofjustice/staff-device-shared-services-infrastructure) - Create infrastructure from the main AWS shared account into Development, Pre Prodiction and Production via AWS CodePipelines.
- [Docker Container base Images](https://github.com/ministryofjustice/staff-device-docker-base-images) - Repository for base container images used across multiple services. Created as the solution to dockerhub rate limts as suggested by AWS.

### Azure Landing Zone

- [Azure DevOps Pipeline](https://github.com/ministryofjustice/staff-infrastructure-azure-landing-zone) - Azure DevOps pipeline configuration for staff device management and the Azure Landing Zone Hub and Spoke configuration.

### Certificate Services

- [Public Key Infrastructure](https://github.com/ministryofjustice/staff-infrastructure-certificate-services) - Public Key Infrastructure for devices and users. This repository can redeploy the EC2 instances which Entrust build their managed service on.

### Device Management

- [Windows 10 Configuration](https://github.com/ministryofjustice/staff-device-management-windows10-configuration) - Intune Windows Configuration
- [Windows 10 Applications](https://github.com/ministryofjuestice/staff-device-management-windows10-apps) - Intune Windows Applications
- [iOS Configuration](https://github.com/ministryofjustice/staff-device-management-ios-configuration) - iOS Configuration
- [iOS Applications](https://github.com/ministryofjustice/staff-device-management-ios-apps) - iOS Applications
- [Windows Virtual Desktop](https://github.com/ministryofjustice/staff-device-management-virtualdesktop) - WVD - Windows Virtual Desktop
- [Intune Configuration](https://github.com/ministryofjustice/moj-official-intune) - Intune Configuration

### DHCP / DNS

- [DHCP Server ECR Image](https://github.com/ministryofjustice/staff-device-dhcp-server) - Creates the AWS ECR container image for ISC Kea
- [Admin console for DHCP and DNS](https://github.com/ministryofjustice/staff-device-dns-dhcp-admin) - Frontend for managing staff device site dhcp dns
- [Provision infrastructure](https://github.com/ministryofjustice/staff-device-dns-dhcp-infrastructure) - Code to build the AWS infrastructure for the DNS and DHCP platform

### AWS Environment Deployments

![AWS Environments](diagrams/hld-aws-env.png)
[Image Source](diagrams/hld-diagrams.drawio)

### Infrastrastructure Monitoring and Alerting

- [IMA Platform](https://github.com/ministryofjustice/staff-infrastructure-monitoring) - To monitor and alert on MoJO infrastructure and physical devices
- [Data Source Configuration](https://github.com/ministryofjustice/staff-infrastructure-monitoring-datasource-config) - To provision data sources for the IMA Platform
- [SNMP Exporter](https://github.com/ministryofjustice/staff-infrastructure-monitoring-snmpexporter) - To scrape data from physical devices (Docker image)
- [Blackbox Exporter](https://github.com/ministryofjustice/staff-infrastructure-monitoring-blackbox-exporter) - To probe endpoints over HTTP, HTTPS, DNS, TCP and ICMP
- [Metric Aggregation Server](https://github.com/ministryofjustice/staff-infrastructure-metric-aggregation-server) - To pull data from the SNMP exporter (Docker image)

### Security Log Aggregration and Shipping

- [Log Shipping Infrastructure](https://github.com/ministryofjustice/staff-device-logging-infrastructure) - Log shipping to infrastructure > OST
- [Syslog to CloudWatch](https://github.com/ministryofjustice/staff-device-logging-syslog-to-cloudwatch) - Syslog to aws cloudwatch > OST

### Palo Alto Transit Gateway deployment

- [GlobalProtect FW EC2 Deployment](https://github.com/ministryofjustice/deployment-GlobalProtect) - GlobalProtect firewall deployment
- [GlobalProtect lambda functions](https://github.com/ministryofjustice/terraform-aws-step_function_globalprotect) - GlobalProtect lambda funtions
- [AWS Transit Gateway](https://github.com/ministryofjustice/deployment-tgw) - AWS transit gateway deployment
- [Panorama Configuration](https://github.com/ministryofjustice/terraform-panorama-config) - Panorama Config written in Terraform
- [Public Services Network](https://github.com/ministryofjustice/deployment-PSN) - Public Services Network connection in AWS, connected via Lumen (previously CenturyLink)
