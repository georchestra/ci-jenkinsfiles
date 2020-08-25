# About

This repository contains the descriptions of the Jenkins-ci jobs used by the
official geOrchestra CI.

# Requirements

A Jenkins 2.x is mandatory.

# Creating jobs using ansible

Create a virtualenv:

```
$ virtualenv -p python3 venv
```

Install the required python libraries:

```
$ source venv/bin/activate
$ pip install -r requirements.txt
```

Create an inventory:

```
$ cp inventory.yaml.dist inventory.yaml
```

Modify the created file to suit your environment, then launch the playbook:

```
$ ansible-playbook playbooks/jenkins-jobs.yaml
```
