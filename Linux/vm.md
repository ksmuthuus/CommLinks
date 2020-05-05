# VM specific commands

## Show IP

```sh
ip addr
```

## Set hostname

```sh

```

## Enable Password based authentication

```sh
nano /etc/ssh/sshd_config
# PasswordAuthentication yes
```
## Change hostname

```sh
hostname <newname>
```

## Copy SSH Key

```sh
ssh-copy-id user@targetVMIP
```
