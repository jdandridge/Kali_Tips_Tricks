# 9 Things To Do After Installing Kali Linux
- **Important**Perfom these actions before connecting to the internet. Connect on 8 before update and upgrade

## **Check**, 1. Change Hostname
    $ whatis hostnamectl
    $ sudo hostnamectl set-hostname Demo
### Use nano and change (kali) to (Demo) in the /etc/hosts file
    $ sudo nano /etc/hosts
    $ exit

## **Check**2. Create New User - Hit enter to bypass the value for default
    $ sudo adduser goku
### **Note**Check on new user
    $ cat /etc/passwd | grep goku
    $ ls /home
    $ cat /etc/passwd

## **Check**3. Add New User To Sudo Group
    $ sudo usermod -G sudo goku
### **Note**Change to user - logout to change to new user
    $ su goku
    $ sudo -l
    $ exit

## **Check**4. Lock Kali Default User
    $ sudo usermod -L kali
### **Note**Cat into /etc/shadow to see the staus of the locked kali acct.(!) will mean its locked
    $ sudo cat /etc/shadow | grep kali

## **Check**5. Generate SSH Key Pair. Used to login into servers/remote connect. Continue with Enter
    $ ssh-keygen -t ecdsa -b 521
    $ ls .ssh

    $ ssh localhost

## **Check**6. Check For Running Service (+) is running, (-) is not running.
    $ service --status-all
### **Note**Turn off ssh to reduce attack surface
    $ sudo service ssh stop
    $ sudo service ssh status
### **Note**Disable on startup
    $ sudo systemctl disable ssh
    $ sudo service ssh status

## **Check**7. Change Settings in Power Mgmt
- Presentation Mode

## **Check**8. Update Repos & Upgrade Packages
    $ sudo apt update
    $ apt list --upgradable
    $ sudo apt upgrade -y

## **Check**9. Installing Kali Metapackages
    $ sudo kali-tweaks
**Note**
- use space/enter to select
- tab to select Apply/Back
- select 802-11 and bluetooth












