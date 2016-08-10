# ipcheck
Bash script to run with cron or the like to monitor a public IP address and either
notify via email (version 1.0.0) or update the A Name record in AWS Route53 (version 2.0.0).
Useful for remote hosts without static IP addresses.  A home SSH server, for example.

##Version 1.0.0
Must have an email server configured (Postfix,Sendmail).
Edit to use the path to your ipcheck directory.

##Version 2.0.0
Depends on Python, uses awscli and virtualenvwrapper, and assumes AWS DNS hosting (Route53).
Edit to use your virtualenv, your aws hosted zone id, and your domain name.
