# Assignment - 4
## Shell Scripting

>Name: Aman Narnaware
>
>Roll: 322005
>
>Batch: B1
>
>PRN: 22110404

### 1) What is S3 service of AWS

Amazon Simple Storage Service (S3) is a widely-used object storage service provided by Amazon Web Services (AWS). It's designed to store and retrieve any amount of data from anywhere on the web.

**Object Storage**: S3 is an object storage service. Unlike traditional file storage systems where files are stored in a hierarchical file structure (like folders in a computer), S3 stores data as objects within buckets. Each object consists of data, metadata, and a unique identifier. This approach allows S3 to handle large amounts of unstructured data efficiently.

**Scalability**: S3 is highly scalable. It can store virtually unlimited amounts of data, and AWS automatically handles the scaling of infrastructure as your storage needs grow. This scalability makes it suitable for a wide range of use cases, from small-scale applications to enterprise-level solutions. 

**Durability and Availability**: S3 offers high durability and availability. It stores data redundantly across multiple devices and facilities within a region to ensure durability. This means that even if one or more components fail, your data remains safe and accessible. Additionally, S3 provides high availability, ensuring that your data is accessible whenever you need it.

**Performance**: S3 is designed for high performance. It provides low-latency access to data, allowing applications to retrieve and store data quickly. Additionally, S3 offers features such as byte-range fetches and multi-part uploads to optimize performance for large objects and streaming workloads.

---

### 2) Step-by-step screenshot to upload static web application on the AWS cloud using S3 service

-  Login to AWS console and select S3 Service.
  
    ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/ab7b1146-332e-426a-a0fb-488c1b5f3a9b)

-  Select Create a Bucket.

    ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/57a0af95-009e-4411-9b74-f95e1a1e5c42)

-  Name the bucket and unselect 'Block all public access' and create bucket.

    ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/62ee429b-c4a7-40c8-b68c-294db9ec16c0)

    ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/da4a25b1-0088-454d-99bc-f77f6267de4b)

-  Select the created bucket and in properties find 'Static website hosting' and enable it. Enter the index document (usually "index.html") and error document if you have one.

    ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/d324c7e0-d989-4c10-bb27-a686d7803f3f)

-  Select your created bucket from the bucket list and upload the necessary file(s) for the website. Make sure that the index documnent is in the root directory.

   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/24b82736-c8e0-492a-8ad8-c7c470dd4639)

   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/ebfbccbc-d1d6-482e-8a0b-ad7dbaaea8f2)


-  Next step is to create a bucket policy to allow traffic to the website. You can use [AWS Policy Generator](https://awspolicygen.s3.amazonaws.com/policygen.html) to create policies or visit [Amazon Documentation](https://docs.aws.amazon.com/AmazonS3/latest/userguide/access-policy-language-overview.html?icmpid=docs_amazons3_console).

```
{
	"Version": "2012-10-17",
	"Statement": [
		{
			"Sid": "PublicReadGetObject",
			"Effect": "Allow",
			"Principal": "*",
			"Action": "s3:GetObject",
			"Resource": "arn:aws:s3:::mys3bucketassignment4/*"
		}
	]
}
```
You can get your ARN from the properties in the bucket list.

   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/d5b40989-525c-46df-858a-5048a91ec5a2)

Save Changes.


-  Once you've set up everything, you can access your website using the endpoint provided in the "Static website hosting" in the bucket properties. It will look something like this: http://mys3bucketassignment4.s3-website.ap-south-1.amazonaws.com

   ![image](https://github.com/RealBeazt/Cloud_Assignments/assets/113709187/2c8cf9c3-8f81-4835-820d-1589325547bb)


Your static website is now hosted on Amazon S3 and accessible via the internet !!



