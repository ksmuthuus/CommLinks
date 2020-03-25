# AWS Commands
## EC2
### SSH EC2 Instance
```sh
ssh -i *.pem user@ip
```

### Update all packages
```sh
yum update -y
```

### get admin privileges
```sh
sudo su -
```

### install httpd (Linux 2 version)
```sh
yum update -y
yum install -y httpd.x86_64
systemctl start httpd.service
systemctl enable httpd.service
echo "Hello World from $(hostname -f)" > /var/www/html/index.html
```

### Test server
```sh
curl localhost:80
curl google.com
```