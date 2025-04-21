# Database Monitoring and Management System

This project sets up monitoring and alerting for SQL Server (or Oracle) databases. The system collects performance metrics, monitors the health of your databases, and sends alerts for any critical issues, such as high CPU usage or slow queries.

## 🚀 Project Goals

- Monitor database health (CPU, memory, disk usage) using xxxx.
- Track slow-running queries and set up alerts for performance issues.
- Create a dashboard for real-time database performance.
- Set up alert notifications via email, Slack, or other channels.

## 🛠️ Tech Stack

- **Backend:** SQL Server (or Oracle)
- **Monitoring:** Datadog
- **Alerting:** Email, Slack, or SMS notifications via Datadog
- **Version Control:** GitHub

## 🗂️ Project Structure

```plaintext
db-monitoring/
│
├── config/                  # Configuration files for agent
│   └── sqlserver.yaml       # Integration config for SQL Server
│
├── scripts/                 # Setup scripts for agent and database
│   └── setup.sh     # Script to install and configure agent
│
├── .github/
│   └── workflows/           # GitHub Actions for deployment (optional)
│       └── deploy.yml       # GitHub Actions pipeline for deployment
│
├── README.md                # Project documentation

## Steps to integrate with SQL server

1. Install the agent
2. Configure the Agent.
```
init_config:

instances:
  - host: localhost
    username: 'sa'
    password: 'xxxx'
    driver: 'ODBC Driver 17 for SQL Server'
    port: 1433
    tags:
      - 'environment:production'
      - 'db:sqlserver'
```
3. Start the agent
4. Check if the data in Coming up in the UI
5. Set up monitors and then create dashboards


