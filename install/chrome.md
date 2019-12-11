[centos]
yum -y install  redhat-lsb
yum -y install libappindicator-gtk3

rpm -ivh google-chrome-stable_current_x86_64.rpm 
cd /etc/yum.repos.d/

touch google-chrome.repo
vim google-chrome.repo 

    [google-chrome]
    name=google-chrome
    baseurl=http://dl.google.com/linux/chrome/rpm/stable/x86_64
    enabled=1
    gpgcheck=1
    gpgkey=https://dl.google.com/linux/linux_signing_key.pub

yum install google-chrome-stable --nogpgcheck

#start
google-chrome --no-sandbox
