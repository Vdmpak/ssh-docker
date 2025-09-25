See the [docker-image repo](https://gitlab.computing.dcu.ie/aslaimi/csc1037/week11-docker-image-repo) containing the docker image which
contains and runs `sshd`, the SSH daemon. Follow the instructions in the [docker-image repo](https://gitlab.computing.dcu.ie/aslaimi/csc1037/week11-docker-image-repo) to load the docker image and run it.

It is configured to have an account for each CSC1037 student, with their regular DCU username.

Run a docker container using this image, publishing port 22 (the SSH port) to either port 22 or port 2022. If you use the docker-compose.yml file supplied in the docker0image repo, it will run the ssh server at port 2022.

You will have received an SSH key private key by email.  The passphrase for that private key is *foobar*.

Use that key to access your account in the container, and then run this command:

    $ my-hash

You can also visit this [web page](https://www.cyberciti.biz/faq/unix-linux-execute-command-using-ssh/) to learn how to run a remote command using ssh.

The output will be an encrypted message which looks like this:

```
U2FsdGVkX1+SJNuLk6R1nVD6uU/zeB+kfaDLToSKlR5MB+ff6qwCA/DKWMgqQiEE
ahKqtusK39ePs6f5lezLECdWk3u0iHV/hpqkc8Re7xH/RzPosdTjsFT7oQGKWf4G
MdAGozs16fpT7hp9RCOMByMXR3BmmrZ7IISjhgATDnL3S1An/0FH4gJYpvXryPMv
.
.
.
0P3/D3mFmv77v1n0EKHz/nH6l4K50FNqjLNT/aW6mWGnf8nWCOYsGff8ylP9weR4
acsxqGCN4ZpUA5ntHHihCWVEdBBcRUSfUl74cXom5g+pU/2PDn4uTysuE4L1x2CQ
fwjQcF+pF3jwKrZ9riT+FsjIgQ58Q1PcDseUOaXmLU0=
```

Copy that encrypted message to a file named `ssh-my-hash-1.txt` and upload it to
[_Einstein_](https://csc1037.computing.dcu.ie/einstein/).
