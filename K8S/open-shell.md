```sh
kubectl run my-shell --rm -i --tty --image ubuntu -- bash
apt update
apt install telnet

exit
```

* my-shell: This ends up being the name of the Deployment that is created. Your pod name will typically be this plus a unique hash or ID at the end.
* --rm: Delete any resources we've created once we detach. When you exit out of your session, this cleans up the Deployment and Pod.
* -i/--tty: The combination of these two are what allows us to attach to an interactive session. 
* --: Delimits the end of the kubectl run options from the positional arg (bash).
* bash: Overrides the container's CMD. In this case, we want to launch bash as our container's command.


