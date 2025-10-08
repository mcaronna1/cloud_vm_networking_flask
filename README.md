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
[creatingvm](images/creatingvm.png)
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
1. **Copy the Flask template**:  
   ```bash
   git clone https://github.com/hantswilliams/HHA-504-2025-FlaskStarter.git
   cd flask_template
   ```
    Change directory:
   ```
   cd HHA-504-2025-flaskstarter
    ```   
    Create new virutal environment: 
    ```
    python3 -m venv venv
    ```
    If that didnt go and create add:
    ```
    sudo apt install python3.12
    ```
   Go back and copy the virtual enironment again:
   ```
    python3 -m venv venv
    ```
   Type in terminal to see if all list of files are loaded:
    ```
    ls -l
     ```
     Then activate virtual environment:
    ```
    source venv/bin/activate
    ```
    Install: 
    ```
    pip install -r requirements.txt
    ``` 
3. **Run the app on port 5003**:  
   ```bash
   python3 app.py
   ```  
4. **Verify public access**:  
   - In browser: `http://48.221.122.79:5003`  
   - Take screenshot of the page loading.  

### 5. Public IP Access
URL: http://48.221.122.79:5003/ 
[screenshot]

### 6. (Bonus) Domain Name
Domain: http://mydomain.tech:5003  
[screenshot]
