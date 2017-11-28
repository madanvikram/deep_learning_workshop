# MCL310 - Building Deep Learning Applications with Apache MXNet and Gluon

This repository includes the tutorial Python notebooks that will be used as part of re:Invent 2017 session MCL310: Building Deep Learning Applications with Apache MXNet and Gluon. We have taken these notebooks from The Straight Dope tutorial book available here: http://gluon.mxnet.io/ 

Instructions for getting started: 

1. Launch EC2 Instance using the Ubuntu deep learning AMI in eu-west-1, Ireland (p2.xlarge - $0.972/hour) http://amzn.to/2j3FdOZ
2. Connect via SSH and tunnel port 8888:
    * Linux, Mac:
        - `ssh -i user.pem -L 8888:localhost:8888 ubuntu@ec2-ip-ip-ip-ip.region.compute.amazonaws.com`
    * Windows: 
        - Follow the instructions [here](http://docs.aws.amazon.com/AWSEC2/latest/UserGuide/putty.html) to download PuTTY and to convert your private key
        - Host Name: `ubuntu@ec2-ip-ip-ip-ip.region.compute.amazonaws.com`
        - Expand Connection and choose Auth, select your .ppk file
        - Expand Connection > SSH, choose Tunnels, specify Source Port: `8888`, Destination: `localhost:8888`
        - Choose Add and Open
3. Clone aws-ai-bootcamp-labs github repository `git clone https://github.com/awslabs/aws-ai-bootcamp-labs`
4. Start jupyter notebook: `nohup jupyter notebook &`
5. `tail nohup.out` to get the login token
    * look for `http://localhost:8888/?token=<your_login_token>`
