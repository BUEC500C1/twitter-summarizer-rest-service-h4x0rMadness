# Configuration

- Connect to my EC2 instance:

```
ssh -i /Users/robertmorrislike/flask-restful.pem ubuntu@ec2-34-230-16-206.compute-1.amazonaws.com
```

To do that, I have to firstly modify the permission of secure key file to 400 instead of 700, otherwise it fails, using

```
sudo chmod 400 /Users/robertmorrislike/flask-restful.pem
```


- Transfer python script for twitter feed:

scp -i /Users/robertmorrislike/flask-restful.pem /Users/robertmorrislike/PycharmProjects/EC500/HW5/twitter_feed.py ubuntu@ec2-34-230-16-206.compute-1.amazonaws.com:~

scp -i /Users/robertmorrislike/flask-restful.pem /Users/robertmorrislike/PycharmProjects/EC500/HW5/sample_flask.py ubuntu@ec2-34-230-16-206.compute-1.amazonaws.com:~

scp -i /Users/robertmorrislike/flask-restful.pem /Users/robertmorrislike/PycharmProjects/EC500/HW5/keys ubuntu@ec2-34-230-16-206.compute-1.amazonaws.com:~
