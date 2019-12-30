1. Generate SSH Key pair via Git Bash:
    ssh-keygen -t rsa -b 4096 -C "email"
2. Ensure SSH agent PID:
    eval $(ssh-agent -s)
3. Add identity to SSH agent:
    ssh-add ~/.ssh/id_rsa
4. Check key pair exists:
    ls-a -l ~/.ssh
5. Show RSA public key: cat ~/.ssh/id_rsa.pub
6. Test SSH to git hub: ssh -T git@github.com
