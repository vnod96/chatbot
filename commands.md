Creating EC2 Instance-
Before creating EC2 instance create a key pair.
Install MobaXterm to use SSH Client for security.

Downlod the Key Pair to laptop and in MobaExterm change the access level for the pem file

cd ~/Desktop
chmod 400 ec2-key.pem
ssh -i ec2-key.pem ec2-user@MY-IP

FOR INSTALLING NGINX
sudo su -
yum install nginx
amazon-linux-extras install nginx1.12
systemctl status nginx
systemctl start nginx

echo " Welcome to Chatbot app" > index.html

FOR INSTALLING NODE
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.34.0/install.sh | bash
. ~/.nvm/nvm.sh
nvm install node
npx create-react-app mysampleapp

