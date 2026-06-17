# AWS-MONITORING-THROUGH-SHELL-SCRIPT
AWS MONITORING THROUGH SHELL SCRIPT




#!/bin/bash
#######################
#vishnu
#aws monitoring proj
#17.06.2026
#aws-cli-
#s3,iam,ec2,lamda
####################

set -x
set -e  fail
set -o pipe line

# list of s3 buckets
echo "s3 details"
aws s3 ls
# list of ec2 instance
echo "ec2 details"
aws ec2 describe-instance
# list of i am user
echo "iam user details"
aws iam list-user
# list aws lamda
echo "aws lamda function details"
aws lamda list-functions
