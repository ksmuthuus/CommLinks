1. Generate SSH Key pair via Git Bash
    ssh-keygen -t rsa -b 4096 -C "email"
2. Ensure SSH agent PID
    eval $(ssh-agent -s)
3. Add identity to SSH agent
    ssh-add ~/.ssh/id_rsa
4. Check key pair exists
    ls-a -l ~/.ssh
