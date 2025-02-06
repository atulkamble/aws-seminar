```
aws ec2 launch - ssh 

SG: ssh, http, https, 3000

cd Downloads
chmod 400 key.pem
ssh -i "key.pem" ec2-user@ec2-44-207-1-254.compute-1.amazonaws.com

sudo yum update -y
sudo yum install git -y
git --version

git config --global user.name "Atul Kamble"
git config --global user.email "atul_kamble@hotmail.com"
git config --list 

curl -sL https://rpm.nodesource.com/setup_16.x | sudo bash -
sudo yum install -y nodejs
node -v
npm -v

git clone https://github.com/atulkamble/aws-seminar.git
cd aws-seminar/

sudo yum install docker -y
sudo systemctl start docker
sudo systemctl enable docker
sudo docker login

sudo docker build -t atuljkamble/user-data-app .
sudo docker images
sudo docker push atuljkamble/user-data-app

sudo docker run -d -p 3000:3000 atuljkamble/user-data-app
sudo docker logs 3e6ff071002
```
