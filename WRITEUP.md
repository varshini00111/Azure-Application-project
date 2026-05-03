# Write-up: Deployment Choice (VM vs App Service)
## 1. Analysis of Virtual Machine (VM)

### Cost

Using a Virtual Machine can be more expensive because you have to pay for the VM even when it is idle. Additional costs may also come from storage, networking, and maintenance.

### Scalability

Scaling a VM is not automatic. If traffic increases, we need to manually upgrade the VM size or create additional VMs, which takes time and effort.

### Availability

Availability depends on how well the VM is managed. If the VM goes down, manual intervention is required to restart or fix it.

### Workflow

Using a VM requires setting up the environment manually (installing Python, dependencies, configuring server, etc.). Deployment and updates are more complex and time-consuming.

## 2. Analysis of Azure App Service

### Cost

Azure App Service provides a free tier (F1), which is enough for small projects like this. It is more cost-effective compared to running a VM continuously.

### Scalability

App Service supports easy scaling. It can be scaled up or down with minimal effort, and Azure handles most of the infrastructure automatically.

### Availability

Azure manages uptime and reliability. The platform ensures better availability compared to manually managed VMs.

### Workflow

Deployment is simple. Code can be directly connected through GitHub, and Azure handles the environment setup. This reduces development and deployment complexity.

## 3. Final Choice: Azure App Service

I chose Azure App Service for deploying this project because it is easier to use, cost-effective, and requires less maintenance. It allows quick deployment and automatic handling of infrastructure, which is suitable for this type of web application.
