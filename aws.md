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

### Install httpd
```sh
yum install httpd.x86_64
```

### Start service
```sh
systemctl start httpd.service
systemctl enable https.service
```

### Test server
```sh
curl localhost:80
curl google.com
```

### Update page
```sh
echo "Hello World from $(hostname -f)" > /var/www/html/index.html
```
