
#  Build a Modern Application on AWS

https://github.com/aws-samples/aws-modern-application-workshop/tree/java/module-1

 aws s3 mb s3://REPLACE_ME_BUCKET_NAME
  
  aws s3 mb s3://cheungm-MythicalMysfitsIDE-20220914
  
  aws s3 mb s3://cheungm-mythicalmysfits-20220914
  
  aws s3 ls s3://cheungm-mythicalmysfits-20220914
  
  aws s3 cp ~/environment/aws-modern-application-workshop/module-1/web/index.html s3://cheungm-mythicalmysfits-20220914/index.html
  
    
  curl -I "https://cheungm-mythicalmysfits-20220914.s3-ap-southeast-1.amazonaws.com/index.html"
  
  aws s3api put-bucket-policy --bucket cheungm-mythicalmysfits-20220914 --policy file://~/environment/aws-modern-application-workshop/module-1/aws-cli/website-bucket-policy.json


aacb-developer:~/environment $   aws s3api put-bucket-policy --bucket cheungm-mythicalmysfits-20220914 --policy file://~/environment/aws-modern-application-workshop/module-1/aws-cli/website-bucket-policy.json

An error occurred (AccessDenied) when calling the PutBucketPolicy operation: Access Denied


## Create presigned URL
https://cheungm-mythicalmysfits-20220914.s3.ap-southeast-1.amazonaws.com/index.html?response-content-disposition=inline&X-Amz-Security-Token=IQoJb3JpZ2luX2VjEEYaDmFwLXNvdXRoZWFzdC0yIkcwRQIhAOqxpZvOXK7mCYTV1WIQqH%2FUmlKhK45BlZXIkFSMsnlaAiBV7RFiJAKqZTzFtiUZs3NfD%2BCHsYNUK7Nev9RXfNFgYirpAgjf%2F%2F%2F%2F%2F%2F%2F%2F%2F%2F8BEAEaDDA3NzAyMzQ1NjM5MiIMdawIC0iiqu5C3nMxKr0CzK7H8jfjIWFnyCYGz%2FZHe7psgwa%2BHcfqQpxeQTFt12Im6hucJB0s1PnOCiP2vkP6TOP5MisK%2BPNQYkhXOfHRrpiSJ%2BArIXTb3Xjq2Uvrc5%2B4%2BOJnvPdkPVJlcGJyhqWZzyZXKzNtKDA9Q1zkBNs7Z8yZztsH76AlTWhdRgbnbc9WVOHceMApdy4LTlRRxsETQifWJlRCXgWNfguvEpZu9hvLN9TSII5nuhLS2K%2Bjw53ss%2FIAwa7ZdqBB51VFnuH9cuUDdXkVzIa9zKl3PfK0UqVck2dRe%2BbyhSkZnAbfXNiTkKKRB1kty0DgEeIEB0wg%2BHasH%2FsgrQZpz4J%2BMIGCg0xiDptg%2BpJKyBdZDcHEFdhrlL0QcZSZZCDEgTnUwaCFZ0jo0FB3z6YqwwI0vw70qbYRmczeSFOk5W3ZU90wjLGOmQY6hwJyw4FhsAv5y8kr0UQyXMqBB%2B40a0PfPzu1aX0%2BhnXGPkL%2BKJKYRgQ5a3%2F2GebWp5aPjdYfw%2FCT9S9lh%2BJ0wCb0WtZLAyHoKZMNn6H%2BTbfz1x1BSJ7Ockg6R0hHYj6RyD8M8r6qg6%2FGJsaJfaZSMQ7sOJNHV5qBeYR1y%2F7Lqn2aWes0YDIDDucnfczCsMpfOwShVLN6r7NKGQRsxC1uHWJDapoqWuOXgrdPT65Zo6AL%2FyWte9apwO0H7oyPOVk6%2FsBEo2VKA7a01G8wVQbOXGDkRK%2FaCNTOjf9DqfExXKdGceZYsXlnDhlFg3PLcAKTncVNX6%2BrR8jeRTbIUmzNlhlkSKDjrh9y1A%3D%3D&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Date=20220915T215129Z&X-Amz-SignedHeaders=host&X-Amz-Expires=43200&X-Amz-Credential=ASIARD3XUVSEIO3PU6TE%2F20220915%2Fap-southeast-1%2Fs3%2Faws4_request&X-Amz-Signature=289e7460b74d6ff8f9909a33f5a21ee3f5d8aafc33f29a0c65703b3a6b83fc74


ec2-54-254-10-243.ap-southeast-1.compute.amazonaws.com
fu8FP$bMB6=JARuKYSS4jR@M?c-p*O$d


http://mysfits-nlb-37a666f340cc584b.elb.ap-southeast-1.amazonaws.com/mysfits
