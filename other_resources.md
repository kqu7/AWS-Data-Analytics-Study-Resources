## Introduction
---
This section contains various other resources I used when studying for the exam. For details, please check out the table of contents.

## Table of Contents
--- 
- [Official Material](#Official-Materials)
- [Book](#Book)
- [Video Courses](#Video-Courses)
- [Practice Problems](#Practice-Problems)
- [Exam Tips](#Exam-Tips)
- [Big Data and Distributed System Knowledge](#Big-Data-and-Distributed-System-Knowledge)


<div style="text-align: right"> ⬆️  &nbsp; <a href="./README.md">Back to the Main Page</a> </div>

## Official Materials
---
[Official Exam Guide](https://d1.awsstatic.com/training-and-certification/docs-data-analytics-specialty/AWS-Certified-Data-Analytics-Specialty_Exam-Guide.pdf) 

[Offical Sample Questions](https://d1.awsstatic.com/training-and-certification/docs-data-analytics-specialty/AWS-Certified-Data-Analytics-Specialty_Sample-Questions.pdf) 

## Book
--- 
[AWS Certified Data Analytics Study Guide: Specialty (DAS-C01) Exam](https://www.amazon.com/Certified-Data-Analytics-Study-Guide-ebook/dp/B08PJMV9BZ)
- Review: 
    - This is a very comprehensive book that can give you both the overview of AWS data analytics services and the detail of each. I read it twice, the first time for the general introduction, and the second time for details of each services and the integration among them. 


## Video Courses
---
[*Introductory course*] [Udemy’s AWS Certified Data Analytics Specialty 2020](https://www.udemy.com/course/aws-data-analytics/)
- Review
    - A great introductory course that guides you through each AWS data analytics services. If you don't have any previous exposure to data anlaytics, you can use this course as your starting point. It also contains several hands-on labs and practice questions.


[*Advanced course*] [AWS Certified Data Analytics Speciaty](https://www.youtube.com/playlist?list=PLAFY3hrExHFHDiq_mjEXMqFj6ffrWXLR1)
- Review
    - This series of courses contain the best practices and insights for AWS data analytics services.  

## Practice Problems
--- 
[Udemy’s AWS Certified Data Analytics Specialty 2020](https://www.udemy.com/course/aws-data-analytics/)
- Review
    - There are practice questions after you finifsh a section of video course. At the end, there is a practice test with 65 questions. I would say the practice test is a bit simpler than the real-exam. In the real-exam, the differences among choices are more subtle and the wording of question is more delicate. 

[Whizlab: AWS Certified Data Analytics - Specialty](https://www.whizlabs.com/aws-certified-data-analytics-specialty/)
- Review:
    - There are 3 practice tests (65 questions each) and an additional 20 question quiz. Some problems are too technical and are unlikely to be asked in the real-exam. However, the good thing about these practices is that they provide detailed explanation and links to further read, which can help you deepen your understanding toward the service    

[AWS Certified Data Analytics Study Guide: Specialty (DAS-C01) Exam](https://www.amazon.com/Certified-Data-Analytics-Study-Guide-ebook/dp/B08PJMV9BZ)
- Review:
    - There are about 10 practice questions at the end of each chapter and a practice test (65 questions) at the beginning. I would say this practice test is the most similar one to the real exam in terms of question formats and levle of difficulty. 


## Exam Tips
--- 
From Reddit: 
- [Just passed the AWS Data Analytics Specialty Cert](https://www.reddit.com/r/AWSCertifications/comments/hsag0q/just_passed_the_aws_data_analytics_specialty_cert/)


- [AWS Data Analytics certification preparation tips](https://www.reddit.com/r/AWSCertifications/comments/hjhht9/aws_data_analytics_certification_preparation_tips/)

From Medium/Towards Data Science: 
- [The 5-STEP program to get the AWS Data Analytics Certification in three months:](https://medium.com/globant/the-4-steps-program-to-get-the-aws-data-analytics-certification-2020-in-three-months-84733c00bb98)

- [Becoming an AWS Certified Data Analytics — NEW April 2020](https://towardsdatascience.com/becoming-an-aws-certified-data-analytics-new-april-2020-4a3ef0d9f23a)

- [Passed Big Data Specialty Exam](https://acloud.guru/forums/aws-certified-big-data-specialty/discussion/-M2QMFSiD1Gygknha07Z/Passed%20Big%20Data%20Specialty%20Exam!)


- [How did I get certified with AWS Big Data Specialty](https://towardsdatascience.com/how-did-i-get-certified-with-aws-big-data-specialty-)


- [Becoming AWS Certified in Big Data Specialty in 2 Months](https://towardsdatascience.com/becoming-aws-certified-in-big-data-specialty-in-2-months-ecf77d3e06db)

- [My Path to AWS Big Data Speciality Certification](https://simonleewm.medium.com/my-path-to-aws-big-data-speciality-certification-4baff3a8150)

My Thoughts/Tips
- About preparation
    - Most questions in the real exam are about how these data analytic services are applied in the *real-life scenarios* and *integrate* with each other. Thus, it is very important to understand the **_best practices_** of each services and be familiar with some common **_architectural patterns_** used by AWS data analytics for different scenarios. You can accomplish this by doing some hands-on experiments, checking out the best practices, and reading relevant blogs (check out the [*Hands-On Practices and Architectures*](./hands_on_labs_and_architectures.md) Section)  
    - Based on my testing experience, IoT, Step functions, DMS and S3 Glacier did not appear a lot in the test questions. While it is still important to know what they are, you probably do not have to delve too deep into it. In the contrast, there are several topics that occur frequently in the exam:
        -  *Kinesis* appeared a lot in the exam, so you would want to understand its use case, integration with other services, and its limitations as well as common expceptions.  
        - There were a lot of questions related to the best practices of *Redshift* and *Athena*, as well as its integration with S3 and Glue
- For the actual exam
    - There are 65 questions that are needed to complete in 190 minutes, so about 2:45 for each question. If a question is particularly wordy or difficult to understand, you can skip it at first and review later, after you finish the easy ones and can focus on the hard ones.

## Big Data and Distributed System Knowledge
--- 
[Designing Data-Intensive Applications: The Big Ideas Behind Reliable, Scalable, and Maintainable Systems](https://www.amazon.com/Designing-Data-Intensive-Applications-Reliable-Maintainable/dp/1449373321)
- Review
    - A comprehensive book that gives you an introduction of data systems and distributed data
