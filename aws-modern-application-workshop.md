
#  Build a Modern Application on AWS

https://github.com/aws-samples/aws-modern-application-workshop/tree/java/module-1

 aws s3 mb s3://REPLACE_ME_BUCKET_NAME
  
  aws s3 mb s3://cheungm-MythicalMysfitsIDE-20220914
  
  aws s3 mb s3://cheungm-mythicalmysfits-20220914
  
  aws s3 ls s3://cheungm-mythicalmysfits-20220914
  
  aws s3 cp ~/environment/aws-modern-application-workshop/module-1/web/index.html s3://cheungm-mythicalmysfits-20220914/index.html
  
    
  curl -I "https://cheungm-mythicalmysfits-20220914.s3-ap-southeast-1.amazonaws.com/index.html"
  
  aws s3api put-bucket-policy --bucket cheungm-mythicalmysfits-20220914 --policy file://~/environment/aws-modern-application-workshop/module-1/aws-cli/website-bucket-policy.json
