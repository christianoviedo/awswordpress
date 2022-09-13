# awswordpress
Cloudformation file for installing HA Wordpress in AWS, in a simple way

Architecture:
- Mysql Aurora Database 
- 2 servers
- Load Balancer
- EFS for uploads folder

Notes:
- Only works in us-east-1
- Uses Amazon Linux 2
- Has 2 instances, one 
- Does not support scallability


Note: this is a beta development, if there's any problem with installing Wordpress on Amazon Linux try this command to check the error messages:

   grep -ni 'error\|failure' $(sudo find /var/log -name cfn-init\* -or -name cloud-init\*)
