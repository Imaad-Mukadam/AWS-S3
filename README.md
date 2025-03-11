# AWS-S3 (Bucket/Storage)

## Summary

### **AWS S3 Bucket Configuration Summary**  

1. **Create an S3 Bucket** 🪣  
   - Ensure the bucket name is unique.  
   - Enable public access settings (if needed).  

2. **Upload `index.html` File** 📂  
   - Upload an `index.html` file to the bucket.  

3. **Allow Public Access** 🔓  
   - Create a **Bucket Policy** to allow public read access.  
   - Example policy:  
     ```json
     {
       "Version": "2012-10-17",
       "Statement": [
         {
           "Effect": "Allow",
           "Principal": "*",
           "Action": "s3:GetObject",
           "Resource": "arn:aws:s3:::your-bucket-name/*"
         }
       ]
     }
     ```  

4. **Enable Versioning** 🔄  
   - Turn on **Versioning** in the bucket settings.  
   - Upload an updated `index.html` file to see version history.  

This setup ensures that changes to your website can be tracked and restored if needed! 🚀

# Step - 1

i.Lets create a S3 bucket

![image alt](1.PNG)

ii. Remember to give a unique name for your S3 bucket

![image alt](2.PNG)

iii. Remove block public access and enable Bucket versioning to get the versions of our files, then create the bucket

![image alt](3.PNG)

iv. Now lets upload our static website on bucket

![image alt](4.PNG)

v. Click on upload files or drag and drop your files 

![image alt](5.PNG)

vi. Now click on your uploaded file

![image alt](6.PNG)

vii. Now click on Open

![image alt](7.PNG)

viii. You can see your dummy website is running

![image alt](8.PNG)


# Step - 2

i. To see the versioning , Edit your website

![image alt](9.PNG)

ii. Then again upload your file , then on the show versions button

![image alt](10.PNG)

iii. You can see versions of your files

![image alt](11.PNG)

![image alt](12.PNG)

