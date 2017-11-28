# AWS
# AWS Tutorials

sudo -s
cd
yum -y update
yum install wget
sudo yum install R -y
sudo yum groupinstall "Development Tools" -y
sudo wget https://download2.rstudio.org/rstudio-server-rhel-1.1.383-x86_64.rpm
sudo yum install --nogpgcheck rstudio-server-rhel-1.1.383-x86_64.rpm -y
useradd ruser
echo ruser:rpassword | chpasswd
