# AWS
Just a notes

## connection through ssh key

### open terminal cd ~/.ssh include this in config file
    Host ec2cluster
            HostName 54.175.62.10
            User ec2-user
            IdentityFile /Users/naren/Documents/Narendra/Work/AWS/Key_Pair/EC2Instance.pem

*to connect through terminal ssh ec2cluster*

# Running bootstrap script so whenever the server launch this script will run

## This Script to enable httpd in ec2 instance.

    #!/bin/bash
    
    # install http (Linux2 version)

    yum update -y
    yum install -y https.x86_64
    systemctl start httpd.service
    systemctl enable httpd.service
