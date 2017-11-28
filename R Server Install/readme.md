# Installing R Server on AWS Linux
## Create Security Group for R Server
![create security group for r server](https://user-images.githubusercontent.com/33963568/33333382-b47230ac-d434-11e7-8170-74bf6ca9671a.png)

## Launch EC2 Instance
![launch ec2 instance](https://user-images.githubusercontent.com/33963568/33333398-bda5a726-d434-11e7-9330-199f2efbe5da.png)

## Select Instance Type
![select instance type](https://user-images.githubusercontent.com/33963568/33333411-c5555c0a-d434-11e7-9897-888847948fd9.png)

## Configure Instance Details
![configure instance details](https://user-images.githubusercontent.com/33963568/33333419-cf177124-d434-11e7-8b62-12f23cbe4b87.png)

## Add Tags
![add tags](https://user-images.githubusercontent.com/33963568/33333430-d7d48afe-d434-11e7-96f1-e8a4a354b1a5.png)

## Configure Security Group
![configure security group](https://user-images.githubusercontent.com/33963568/33333444-dd85c5c6-d434-11e7-8d4c-bde64efdaa31.png)

## Review Instance Launch
![review instance launch](https://user-images.githubusercontent.com/33963568/33333452-e5d80aae-d434-11e7-960a-bef5fcdef446.png)

## Select a Key Pair
![select a key pair](https://user-images.githubusercontent.com/33963568/33333464-ec6813dc-d434-11e7-90a5-3bef609bf8b2.png)

## Review Instance Status
![review instance status](https://user-images.githubusercontent.com/33963568/33333479-f3beb8de-d434-11e7-8a0d-c2c95b85ff83.png)

## Note the Public DNS and connect SSH
![note the public dns and connect ssh](https://user-images.githubusercontent.com/33963568/33333494-faa0c0f2-d434-11e7-8cc6-32cd07a70398.png)

## Run following script:
```
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
```

## go to http://IP_ADDRESS:8787 and sign in
![go to ipaddress and sign in](https://user-images.githubusercontent.com/33963568/33333512-0494d864-d435-11e7-82fd-222b6a5ffb21.png)

## Enjoy R
![enjoy r](https://user-images.githubusercontent.com/33963568/33333516-0924123c-d435-11e7-8edc-fde3a168bed7.png)
