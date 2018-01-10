# Setting up AWS server

Goal of this tutorial is to set u pan aws ec2 instance for deep learning purposes,
to be worked on via Jupyter.

Strongly based on
* <https://www.datacamp.com/community/tutorials/deep-learning-jupyter-aws>
* <https://aws.amazon.com/getting-started/tutorials/launch-a-virtual-machine/>


* set up an AWS account
* go to the EC2 dashboard and click `launch instance`
* select the *Deep learning AMI Ubuntu*
* go to *Configure Security group*
* add rule for Jupyter:  TCP for the protocol, 8888 for the Port, and 0.0.0.0/0 for the last column

![](pics\aws_configure_groups.png)

* launch
* create a new keypair
* save key pair in your user directory in a sub-directory called .ssh
 (ex. C:\user\{yourusername}\.ssh\{keypairname}.pem).

Tip: You can't use Windows Explorer to create a folder with a name that begins
with a period unless you also end the folder name with a period. After you enter
the name (.ssh.), the final period is removed automatically.

* go to this folder with git bash
```
$ chmod 400 {keypairname}.pem
$ ssh-add {keypairname}.pem
```

## SSH connection
```
$ ssh -i /c/Users/yourusername/.ssh.<keypairname>.pem' ubuntu@{IP_Address}
```

This works at home, but not at work...
