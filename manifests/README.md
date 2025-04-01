# Observability Stack for API Monitoring 🚀

## Overview
This project sets up a complete observability stack using:
- **Prometheus** – Collects and stores API metrics.
- **Grafana** – Visualizes real-time data.
- **Alertmanager** – Sends alerts when issues occur.

## Features
✅ Monitor API performance (latency, errors, traffic).  
✅ Set up dashboards for real-time insights.  
✅ Get instant alerts when something goes wrong.  

## Prometheus Dashboard Access
You can access the **Prometheus Dashboard** using the following URL:

[Prometheus Dashboard](http://192.168.59.100:32121)

This URL will give you access to the metrics collected by Prometheus for API performance monitoring.

## Grafana Dashboard Access
The **Grafana Dashboard** provides real-time insights into the API performance, error rates, and latency. To access the Grafana dashboard, you can follow these steps:

1. Open your browser and go to the Grafana URL:
   [Grafana Dashboard](http://localhost:3000)  
   (By default, Grafana runs on port 3000 in Kubernetes, but you can change this if necessary.)

2. Login to Grafana using the default credentials:
   - **Username**: admin
   - **Password**: admin

3. Once logged in, you will have access to the pre-configured dashboards that show:
   - API response time trends
   - Error rate over time
   - Database performance metrics

## Alertmanager Setup
Alertmanager integrates with Prometheus to notify engineers of issues:
- **Slack, Email, PagerDuty** integrations are configured to notify about critical issues.
- Alerts will trigger if the error rate exceeds the threshold (e.g., 5% failure rate over 2 minutes).

## How to Get Started
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/khmohan/khmohan-observability.git
