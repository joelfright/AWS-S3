# AWS-S3
Using S3 on AWS

1) The first order of business is to set up an AWS EC2 instance. This will use both the port 80 as well as a simple ssh port and IP.
2) You must then ssh in with `ssh -i (pem file) ubuntu@(iPv4 DNS)`. Then update and upgrade your system.
3) You then need to install some prerequisites which include; `sudo apt-get install python` and `sudo apt-get install python-pip` and `sudo apt-get install awscli`.
4) Then simply type `aws configure`, enter you keys, then use the required region (in my case `eu-west-1`) and `json` as the output format.
5) You can finally make a bucket, in order to make one type `aws s3 mb s3://(bucket-name)`.
6) After this you can enter copy a file over after making one by using `aws s3 cp <file name> s://(bucket-name)`.
7) In order to make the bucket policy global [click here](https://docs.aws.amazon.com/AmazonS3/latest/userguide/add-bucket-policy.html)
