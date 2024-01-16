## **Create Instance in Google Cloud Console**

### 1. **Sign in to Google Cloud Console**
   - 🌐 [Open Google Cloud Console](https://console.cloud.google.com/).
   - 🚀 Log in to your Google Cloud account.
   - In the search bar at the top, type “Compute Engine API” and select it.
   - Click the “Enable” button to activate the API for your project.

---

### 2. **Navigate to Compute Engine**
   - 🖥️ In the left sidebar, click on **"Compute Engine" > "VM instances"**.
   - 🌟 Click on the **"Create Instance"** button.

<img src="/images/1.png" alt="Step 1" width="750">

---

### 3. **Create a New Instance**
   - 💡 **Name**: Enter "docker-playpit" or a name of your choice.
   - 🌍 **Region**: Choose **"europe-central2 (Warsaw)"**.
   - 📍 **Zone**: Select **"europe-central2-a"**.
   - ⚙️ **Machine type**: Pick **"e2-medium"**.

<img src="/images/2.png" alt="Step 2" width="750">

---

### 4. **Select Boot Disk**
   - 💽 **Operating System**: Ubuntu Pro
   - 📀 **Version**: Ubuntu 22.04 LTS Pro Server
   - 💾 **Size (GB)**: 20 GB

<img src="/images/3.png" alt="Step 3" width="750">

---

### 5. **Configure Firewall**
   - 🛡️ Add tags and firewall rules: **http-server**, **https-server**.

<img src="/images/4_1.png" alt="Step 4" width="750">

---

### 6. **Management & Automation**
   - 🤖 **Startup Script**:
     ```bash
     sudo su
     export SSL="yes"
     export USER_NAME="Ivan Sidorov"
     export DOMAIN_NAME="gcp.xip.playpit.net"
     export BASICAUTH="isidorov:mysuperstrongpassword"
     export TRAINING="docker"
     curl -s http://assets.playpit.net/deploy.sh | bash
     ```

<img src="/images/5.png" alt="Step 5" width="750">

---

### 7. **Set Metadata Finalize & Create **
   - 🏷️ **Key 1: login**, **Value 1: isidorov** 
   - 🏷️ **Key 2: passw**, **Value 2: mysuperstrongpassword**
   - 🚀 Click on **"Create"** to start creating your instance.

<img src="/images/6.png" alt="Step 6" width="750">

