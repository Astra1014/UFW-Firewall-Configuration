# UFW-Firewall-Configuration
Basic Firewall Configuration using UFW on Kali Linux

## Objective
To configure and test a host-based firewall using UFW (Uncomplicated Firewall) on a Kali Linux system. The goal is to control inbound and outbound traffic by allowing SSH and blocking HTTP traffic.


## Tools Used
- Kali Linux
- UFW (Uncomplicated Firewall)

## Steps Performed

### 1. Installation
UFW was installed using:

sudo apt install ufw -y

### 2. Initial Status Check
Checked firewall status before configuration:

sudo ufw status verbose


### 3. Default Policies
Configured firewall to:
- Deny all incoming traffic
- Allow all outgoing traffic

### 4. SSH Rule
Allowed SSH access for remote management:

sudo ufw allow 22/tcp
or 
sudo ufw allow ssh


### 5. HTTP Rule
Blocked HTTP traffic for security demonstration:

sudo ufw deny 80/tcp


### 6. Enabled Firewall
Activated UFW:

sudo ufw enable


### 7. Verification
Final rules confirmed using:

sudo ufw status numbered
or
sudo ufw status verbose


## Security Outcome
- SSH access is allowed (secure remote management)
- HTTP traffic is blocked
- System is protected from unwanted incoming connections


## Files Included
- ufw_configuration.sh
- ufw_status_initial.txt
- ufw_status_final.txt
- screenshots folder


## Conclusion
This task demonstrates basic firewall configuration and traffic filtering using UFW, a critical skill in system and network security.
