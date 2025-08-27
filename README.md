# Server Metrics Monitoring (Dockerized)

A general-purpose monitoring stack using **Prometheus + Node Exporter + cAdvisor + Grafana**.  
This stack provides an easy way to monitor your server’s health and visualize metrics in Grafana dashboards.

---

## 📦 Stack Components
- **Prometheus** → collects and stores metrics  
- **Node Exporter** → exposes system metrics (CPU, RAM, disk, etc.)  
- **cAdvisor** → collects Docker container metrics  
- **Grafana** → dashboard & visualization layer  

---

## 🚀 Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/mehdiuserone1/server-metrics-monitoring-Dockerized.git
cd server-metrics-monitoring-Dockerized


2. Start the stack
docker compose up -d

3. Access the services

Grafana → http://localhost:3000

Default login: admin / admin (you can change in provisioning config)

Prometheus → http://localhost:9090

Node Exporter → http://localhost:9100/metrics

cAdvisor → http://localhost:8080

📊 Grafana Dashboards

Provisioned automatically:

Node Exporter Full Dashboard (system metrics)

cAdvisor Dashboard (container metrics)


⚙️ Configuration

Prometheus config → prometheus/prometheus.yml

Grafana provisioning → grafana/provisioning/

If you edit configs, restart affected containers:

docker compose restart prometheus grafana


🛠️ Requirements

Docker

Docker Compose



📜 License

This project is licensed under the MIT License – feel free to use and modify.



🤝 Contributing

Pull requests are welcome! For major changes, open an issue first to discuss what you’d like to change.
