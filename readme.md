aws ecr get-login-password --region us-east-2 | sudo docker login --username AWS --password-stdin 971065425827.dkr.ecr.us-east-2.amazonaws.com
sudo docker build -t 971065425827.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER .
sudo docker push 971065425827.dkr.ecr.us-east-2.amazonaws.com/jquery-eks:$BUILD_NUMBER

