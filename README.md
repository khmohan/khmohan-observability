Atlan Observability Challenge 2025 - Monitoring Stack 🚀
Repository Description:
Welcome to the Atlan Observability Challenge 2025! This repository contains a powerful Kubernetes-based Observability Stack using Prometheus, Grafana, and Alertmanager to monitor REST API performance. It comes with automated deployment scripts, pre-configured dashboards, and alerting mechanisms to help you quickly detect and resolve API issues in real-time.

Features:
API Monitoring: Collects and stores API performance metrics using Prometheus.

Visualization: Beautiful and customizable dashboards to visualize API metrics in Grafana.

Alerting: Sends alerts via Alertmanager for any API performance issues.

Automated Deployment: Easily deployable stack using Kubernetes manifests.

Deployment Steps 🚀:
1️⃣ Clone the Repository
Clone the repository to your local machine:

bash
Copy
Edit
git clone https://github.com/khmohan/khmohan-observability.git
cd khmohan-observability
2️⃣ Deploy the Monitoring Stack
Deploy the complete stack (Prometheus, Grafana, Alertmanager):

bash
Copy
Edit
kubectl apply -f manifests/
3️⃣ Access Grafana Dashboard
To access Grafana's UI, run the port-forwarding command:

bash
Copy
Edit
kubectl port-forward svc/grafana 3000:3000 -n monitoring
Then open your browser and go to: http://localhost:3000

Login:

Username: admin

Password: admin

4️⃣ Verify Prometheus Targets
To verify that Prometheus is scraping the API targets, run:

bash
Copy
Edit
kubectl port-forward svc/prometheus 9090:9090 -n monitoring
Visit http://localhost:9090/targets to ensure the API is being scraped successfully.

5️⃣ Test Alerts in Alertmanager
To check the alerts set up in Alertmanager, run:

bash
Copy
Edit
kubectl port-forward svc/alertmanager 9093:9093 -n monitoring
Then, open http://localhost:9093 and check for any active alerts.

Additional Resources 📚
Grafana Dashboards: JSON files are available for importing dashboards directly into Grafana.

Prometheus Metrics: View the metrics and monitor your services in real-time.

Final Notes ⚡
This repository contains everything you need to deploy an end-to-end observability stack with Prometheus, Grafana, and Alertmanager to monitor and manage REST API performance. It’s easy to set up and ready to use!

💬 Feel free to open issues or contribute if you find any bugs or improvements!
About
Monitoring API performance in real-time has never been easier. This repo provides a highly flexible solution to track your services and receive alerts when something goes wrong.

Contributions 🌱
We welcome contributions to improve the observability stack! Feel free to fork the repo and open a PR for improvements.

Resources 🔗
Prometheus Documentation

Grafana Documentation

Alertmanager Documentation

Badges & Stats:



This structure provides a clear, engaging, and professional README that will attract potential contributors, users, and maintainers. The use of emoji, sections, and step-by-step instructions makes the guide easy to follow and visually appealing.


