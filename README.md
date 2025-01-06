# SOC-Automation-Lab

This project demonstrates the creation of a Security Orchestration, Automation, and Response (SOAR) system to detect and respond to cybersecurity threats in real-time.

## Features

- Log Ingestion:
  - Utilized **Sysmon** and **Wazuh** to collect and ingest security logs from multiple endpoints.
- Threat Detection:
  - Developed custom detection rules to identify malicious activities.
  - Identified threats such as unauthorized access attempts, malware execution, and privilege escalations.
- Incident Response:
  - Integrated with **TheHive** to receive and manage security alerts and incidents.
  - Designed workflows in **Shuffler** to automate incident response.
- Automated Alerts:
  - Configured workflows to automatically send email alerts containing critical details (e.g., system host, IP address, threat type) to an analyst for further investigation.

## Workflow

1. Log Collection:
- Sysmon and Wazuh monitor and ingest system activity logs.
2. Threat Detection Rules:
- Custom rules are applied to identify potential threats.
3. Alert Generation:
- Alerts are sent to TheHive for incident management.
4. Automated Workflow:
- Shuffler workflows process alerts and trigger email notifications to analysts.
5. Analyst Notification:
- Analysts receive detailed emails with all relevant information to guide next steps.

## Tools and Technologies

- **Sysmon**: For detailed system monitoring.
- **Wazuh**: For centralized log management and analysis.
- **TheHive**: As a Security Incident Response Platform (SIRP).
- **Shuffler**: For orchestration and automated workflows.
- **Email Notifications**: Configured to provide real-time alerting to analysts.

## Installation and Setup

1. Set up Sysmon and Wazuh on target machines to start log collection.
2. Configure TheHive to receive alerts from Wazuh.
3. Develop custom detection rules to identify threats.
4. Create automated workflows in Shuffler.
5. Test the full workflow by simulating potential security incidents.

