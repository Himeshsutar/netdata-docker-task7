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
