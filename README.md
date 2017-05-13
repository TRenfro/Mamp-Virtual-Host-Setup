# Mamp-Virtual-Host-Setup
Instructions on how to set up a local environment with MAMP and NGINX

#Set up Mamp Virtual Host

## Step 1

Download Mamp
```
https://www.mamp.info/en/downloads/
```

## Step 2

#### Set Up Ports
Set Web & MySQL Ports to 80 & 3306
Set NGINX port to 8080

## Step 3

#### Configure Host
Open terminal and use the following commands
```
cd /private/etc
```
```
sudo nano hosts
```
add localhost dev URL and save
```
cd ~; cd /Applications/MAMP/conf/apache
```
```
nano httpd.conf
```
find Virtual hosts include and remove # before the path and save

#### Configure Virtual Host
```
cd extra/
```
```
nano httpd-vhost.conf
```
add virtual host path and dev URL

## Step 4

#### Set Up Alias Commands
```
cd ~
```
```
nano .bash_profile
```
#### Add Alias commands
```
alias host='cd ~; cd /private/etc; sudo nano hosts'
```
```
alis vhost='cd ~; cd /Applications/MAMP/conf/apache/extra; nano httpd-vhost.conf'
```

