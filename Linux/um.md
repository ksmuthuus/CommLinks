# User Management Commands

## Switch to root user

```sh
sudo su -
```

## Create User

```sh
useradd <username>
```

## Set password

```sh
passwd <username>
```

## List User groups

```sh
cat /etc/group
```

## List User details

```sh
id <user_name>
```

## Add user to a group

```sh
usermod -aG <group_name> <user_name>
```

## Manage Permissions

```sh
chown -R user:group <dir>

```