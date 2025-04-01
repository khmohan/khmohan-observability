# 🌟 **Atlan Observability Challenge 2025 - Monitoring Stack 🚀**

---

## **📝 About the Project:**

Welcome to **Atlan Observability Challenge 2025**! This repository provides an **end-to-end Kubernetes-based observability stack** built using **Prometheus**, **Grafana**, and **Alertmanager** to monitor and visualize **REST API performance** in real-time. With **automated deployment**, **pre-configured dashboards**, and **alerting mechanisms**, it's easy to stay on top of your system's health and performance!

> 🚀 **Deploy and monitor your API stack effortlessly!**

---

## **🔧 Features:**

- **🔍 API Monitoring with Prometheus**: Collect metrics from your APIs and monitor system performance.
- **📊 Grafana Dashboards**: Visualize the data with beautiful, customizable Grafana dashboards.
- **🚨 Real-time Alerts with Alertmanager**: Get notified instantly when performance issues are detected.
- **⚙️ Automated Kubernetes Deployment**: Easy deployment using Kubernetes manifests.

---

## **🚀 Quick Start Guide:**

### **1️⃣ Clone the Repository**

Start by cloning the repo to your local machine:

```bash
git clone https://github.com/khmohan/khmohan-observability.git
cd khmohan-observability
```

### **2️⃣ Deploy the Monitoring Stack**

Next, deploy the full stack (Prometheus, Grafana, Alertmanager) using Kubernetes manifests:

```bash
kubectl apply -f manifests/
```

This command will apply all necessary Kubernetes configurations and deploy the monitoring stack.

### **3️⃣ Access the Prometheus Dashboard**

To access the Prometheus UI, run the following port-forward command:

```bash
kubectl port-forward svc/prometheus 9090:9090 -n monitoring
```

Then, open [http://localhost:9090](http://localhost:9090) in your browser and navigate to the **Targets** section to ensure your API is being scraped.

### **4️⃣ Access the Grafana Dashboard**

To access the Grafana UI, run the following command:

```bash
kubectl port-forward svc/grafana 3000:3000 -n monitoring
```

Then, visit [http://localhost:3000](http://localhost:3000) in your browser.

**Default Login Credentials:**
- **Username**: `admin`
- **Password**: `admin`

### **5️⃣ Test Alerts in Alertmanager**

To verify the Alertmanager configuration, run:

```bash
kubectl port-forward svc/alertmanager 9093:9093 -n monitoring
```

Then, open [http://localhost:9093](http://localhost:9093) and check for any active alerts.

---

## **💡 Additional Resources:**

- **Grafana Dashboards**: Pre-configured dashboards are available for importing into Grafana.
- **Prometheus Metrics**: Explore the collected metrics in real-time and ensure API health.
- **Alertmanager Setup**: Check active alerts and monitor your system's health status.

---

## **💬 Contribute & Improve:**

We welcome contributions to improve the observability stack! If you find bugs or have suggestions, feel free to fork the repository and create a pull request. Your contributions are highly appreciated!

---

## **🔍 Final Notes:**

This repository has everything you need to get up and running with **Prometheus, Grafana, and Alertmanager** to monitor your **REST API performance**. It's easy to set up, flexible, and ready to be used for any microservices-based infrastructure.

Stay ahead of the game with proactive monitoring and alerts! 🚀

---

## **📚 Documentation & Resources:**

- [Prometheus Documentation](https://prometheus.io/docs/)
- [Grafana Documentation](https://grafana.com/docs/)
- [Alertmanager Documentation](https://prometheus.io/docs/alerting/latest/alertmanager/)
- [Kubernetes Documentation](https://kubernetes.io/docs/)




