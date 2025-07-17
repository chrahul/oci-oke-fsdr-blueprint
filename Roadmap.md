
---

### PHASE 1: Lab Setup Roadmap



---

### **STEP 1: OKE Cluster Setup (Primary Region)**

Goal: Provision a working Kubernetes cluster using **OKE (Oracle Kubernetes Engine)**

#### Sub-Steps:

1. Login to OCI Console
2. Setup a **Custom VCN** with public + private subnets
3. Create an **OKE Cluster** (Managed or Basic)
4. Install **OCI CLI & kubectl** on your laptop or a bastion VM
5. Fetch kubeconfig to connect to your cluster

---

### **STEP 2: Deploy Microservice App**

Goal: Deploy a multi-tier app (e.g. frontend, backend, and DB or PVC storage)

We’ll use:

* **Helm Charts** (for automation)
* **Sample Microservice App** (e.g. Sock Shop, WordPress, or NodeJS+Mongo)
* **Block Volume CSI Driver** for stateful backend

---

### **STEP 3: Enable Persistent Storage**

Goal: Use **OCI Block Volume via CSI driver**

* Install CSI plugin
* Create `StorageClass`
* Deploy PVC-based backend service

---

### **STEP 4: DR Preparation (Region B Infra)**

Goal: Prepare mirror infra in DR region (same VCN, OKE layout)

---

### **STEP 5: FSDR Setup**

Goal: Use **OCI FSDR** to automate failover

* Define **DR Plan**
* Add OKE resources
* Link Block Volume, Secrets, NSGs, etc.

---


