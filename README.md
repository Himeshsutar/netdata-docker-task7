
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

    📈 CPU Usage – Tracks real-time processor load.

    💾 Memory Consumption – Shows used, free, and cached RAM.

    📀 Disk I/O – Monitors read/write speed and disk activity.

    🐳 Docker Container Metrics – Displays per-container resource usage.


4. **Explore Alerts and Chart Panels**:

   Real-time visual charts for each metric

   Built-in alert system with thresholds

   Indicators for warning/critical states

   Charts auto-refresh with live data
   

5.  **Explore Logs in Netdata Container**:

    Open a terminal and run:

      ```
      docker exec -it netdata bash
      cd /var/log/netdata
      ls -lh
      cat netdata.log
     ```

    **Results**

   📈 Netdata Dashboard Metrics


   ![Dashboard](https://github.com/user-attachments/assets/4fa47f25-a193-45b0-8f93-4f193ef06768)




   🐳 Docker Container Monitoring



   ![Container](https://github.com/user-attachments/assets/87b7f846-37b9-49a8-b77f-e6527884dd02)


  
