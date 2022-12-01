# Static-Website-Hosting-AWS-S3
1- Goto S3 service in AWS console.
2- Create a Bucket, give a name (Apha-Website -Name must be unique)
3- Select Region that suits your location.
4- We do not need to change any of these configuration. Standartly it creates BlockPublicAccess Bucket.Click Create Bucket.
5- Uplooad your website files. You can use files from this repo or you can use https://github.com/zce/html5up
6- Click on index.html (it is access denied)
7- Click again on your bucket (alpha-static-website) and goto Properties tab. At the bottow Edit Static WebHosting. Enable it.
8- Host Static Website , select index and error documents.
9- Try to reach index.html it is still access denied.
10- Click your bucket again goto Permissins tab and Edit Block Public Access (deselect all selections) and SAVE it.
11- Goto Permissins tab, Bucket Policy edit it.
12- Paste this Json code there and change "arn:aws:s3:::" with your own ARN and Save changes.
13- Go and try to reach index.html. No it is accessible.