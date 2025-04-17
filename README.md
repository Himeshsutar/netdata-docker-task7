# netdata-docker-task7

# ✅ TASK 7: Monitor System Resources Using Netdata

## 🎯 Objective
Install **Netdata** using Docker and visualize real-time system and application performance metrics including CPU, memory, disk usage, and Docker containers.

---

## 🛠 Tools Used

- **Netdata** (Free, open-source performance monitoring tool)
- **Docker**

---

## 🚀 Steps to Run Netdata

1. **Pull and Run Netdata via Docker**:

   ```bash
   docker run -d \
     --name=netdata \
     -p 19999:19999 \
     --cap-add=SYS_PTRACE \
     --security-opt apparmor=unconfined \
     netdata/netdata

2.  **Access the Netdata Dashboard**:

Open your browser and go to:

👉 http://localhost:19999

3.  **Monitor System Resources:**

📈 CPU Usage

💾 Memory Consumption

📀 Disk I/O

🐳 Docker Container Metrics

4.  **Explore Alerts and Chart Panels**:

Real-time visual charts for each metric

Built-in alert system with thresholds

Indicators for warning/critical states

Charts auto-refresh with live data

5.  **Explore Logs in Netdata Container**:

Open a terminal and run:

'''
docker exec -it netdata bash
cd /var/log/netdata
ls -lh
cat netdata.log
'''

  **Results**


  
