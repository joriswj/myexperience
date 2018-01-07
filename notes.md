# NOTES and IDEAS

## Data Science Experience

This document describes how a complete datasceince eco system can be set up.

Goals:
- learn
- share
- build community
- have discussion


Set up Git Hub account and structure
Set up an AWS instance for datascience
Make solutions scalable


* GIT
* GitHub
* linux
* AWS EC2
* conda
* blogging
* documenting (Sphinx)

Ideas for Use case

Analyse my email usage, by writing a small script in vba (or python??) that will
get the time and subject and maybe word count from all emails.
Analyse the behaviour, and try to forecast my workload.


EXPERIENCES

* setup aws
* what is ssh
* ssh on Chromebook

* in order to connect after a restart of the ec2 instance, I used the following command:
``ssh -i 'location to pem file>.pem' ubuntu@<ip adress>``




RESOURCES
* setting up AWS (Datacamp article): <https://www.datacamp.com/community/tutorials/deep-learning-jupyter-aws>
* setting up AWS for deeplearning: <https://aws.amazon.com/marketplace/pp/B077GCH38C?qid=1513206300209&sr=0-5&ref_=srh_res_product_title>


Blogs:

podcasts:
* Hugo Bown Anderson?
* talk python



NOTES

### Blogging
* https://github.com/holman/left



# Experiences

## using github on corporate pc
Ran into some firewall issues.
The following worked for me:


<https://stackoverflow.com/a/18618941/7619017>

This and could be implemented via:

```
$ git config --global http.proxy http://<proxy>:<port>
$ git config --global https.proxy https://<proxy>:<port>
```

And then for easy acces you could use the following tool:
<https://help.github.com/articles/caching-your-github-password-in-git/>
