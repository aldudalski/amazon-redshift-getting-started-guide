# Step 1: Set Up Prerequisites<a name="rs-gsg-prereq"></a>

 Before you begin setting up an Amazon Redshift cluster, make sure that you complete the following prerequisites in this section: 
+ [Sign Up for AWS](#rs-gsg-prereq-signup)
+ [Determine Firewall Rules](#rs-gsg-prereq-firewall-rules)

## Sign Up for AWS<a name="rs-gsg-prereq-signup"></a>

If you don’t already have an AWS account, you must sign up for one\. If you already have an account, you can skip this prerequisite and use your existing account\.

1. Open [https://aws\.amazon\.com/](https://aws.amazon.com/), and then choose **Create an AWS Account**\.
**Note**  
If you previously signed in to the AWS Management Console using AWS account root user credentials, choose **Sign in to a different account**\. If you previously signed in to the console using IAM credentials, choose **Sign\-in using root account credentials**\. Then choose **Create a new AWS account**\.

1. Follow the online instructions\.

   Part of the sign\-up procedure involves receiving a phone call and entering a verification code using the phone keypad\.

## Determine Firewall Rules<a name="rs-gsg-prereq-firewall-rules"></a>

As part of this tutorial, you will specify a port when you launch your Amazon Redshift cluster\. You will also create an inbound ingress rule in a security group to allow access through the port to your cluster\.

If your client computer is behind a firewall, you need to know an open port that you can use so you can connect to the cluster from a SQL client tool and run queries\. If you do not know this, you should work with someone who understands your network firewall rules to determine an open port in your firewall\. Though Amazon Redshift uses port 5439 by default, the connection will not work if that port is not open in your firewall\. Because you cannot change the port number for your Amazon Redshift cluster after it is created, make sure that you specify an open port that will work in your environment during the launch process\.