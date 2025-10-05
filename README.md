# cloud_vm_networking_flask
networking
# Flask on Cloud VM (Assignment 2)

## Student Info
- Name:  Mairsa Caronna
- Cloud Provider: Azure 

## Video recording: 
- Zoom/Loom: [https://www.loom.com/share/5e43c5fcf2734ff492db14afdb2a87e8?sid=4e6cfb91-edb2-452d-b501-c81938b4f6da] 

## Steps
### 1. VM Creation
[screenshot]
### Part A — VM Setup
1. **Create a VM** on your chosen provider:  
   - Smallest/free-tier size  
   - Ubuntu LTS image  
   - Public IP assigned  

2. **Open port 5003**:  
   - Add a firewall/security group rule to allow inbound TCP traffic on **5003**.  
   - Verify rule is active.  ### 2. Networking (Port 5003 Open)
[screenshot]

### 3. OS Update + Python Install
[commands + screenshot]
### Part B — Environment Configuration
1. **SSH into your VM** (cloud console or terminal).  
2. **Update OS**:  
   ```bash
   sudo apt update && sudo apt upgrade -y
   ```  
3. **Install Git, Python 3 + pip**:
   ```bash
      sudo apt install python3 python3-pip git -y
    ```    

### 4. Flask App Running
[screenshot of terminal + browser]

### 5. Public IP Access
URL: http://XX.XX.XXX.XXX:5003  
[screenshot]

### 6. (Bonus) Domain Name
Domain: http://mydomain.tech:5003  
[screenshot]
