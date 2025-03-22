# ☁️ CloudWatch and CloudTrail 101: Logging and Monitoring with AWS ☁️

**Amazon CloudWatch** and **AWS CloudTrail** provide unified monitoring and auditing for your AWS resources. CloudWatch tracks performance, while CloudTrail logs API activity. In this activity, you will learn the fundamental practices of monitoring and auditing your AWS environment using CloudWatch and CloudTrail.

**Disclaimer:** This activity is based on [Tiny Technical Tutorials'](https://www.youtube.com/watch?v=Yxl7e88cTAQ&ab_channel=TinyTechnicalTutorials), [SkillCurb's](https://www.youtube.com/watch?v=aYhlY9yxeEw), and [Cloud With Django's](https://www.youtube.com/watch?v=P6U89YLJ-ss&ab_channel=CloudWithDjango) tutorials.

## 📋 Requirements
1. **Browser** (Google Chrome, Microsoft Edge, Opera GX, etc.)
2. **AWS Account**

## 🎯 Objectives
1. **Enable CloudTrail** to log API requests and events.
2. **Configure CloudWatch Alarms** for EC2 metrics.
3. **Set Up Log Streams** in CloudWatch for app logs.
4. **Analyze Logs** to monitor system performance.

## ✒️ Part 1: CloudTrail - Trail Creation
1. Log in to your AWS Console.
2. Navigate to `CloudTrail` then click `Trails` on the navigation menu.
3. Click the `Create trail` button.

![image](https://github.com/user-attachments/assets/3498a2a0-7c42-4381-bbe5-806ed48e3c47)

4. Use `management-events-yourname` for the Trail Name and choose `Create new S3 bucket` for the Storage Location.
5. Disable `Log file SSE-KMS encryption` and `Log file validation` then click the `Next` button.

![image](https://github.com/user-attachments/assets/cd3128ad-c96c-4a9f-986f-0083f6b963c5)

6. Tick `Management events` as the event type. Keep everything as is, click `Next` then `Create trail`.
7. Set aside and you may do various API calls, such as creating instances, buckets, tables, etc. Meanwhile, you may move onto CloudWatch first.

## ✒️ Part 2: CloudWatch
1. 

## ✒️ Part 3: CloudTrail - Log Check
1. 

## ✒️ Part 4: Housekeeping
**This is IMPORTANT.** Once you have finished the activity and obtained the required screenshots, **delete all created services and instances in EC2, CloudWatch, and CloudTrail to avoid incurring costs.**

## 📚 Authors
### Activity and Code Materials
- [Tiny Technical Tutorials](https://www.youtube.com/watch?v=Yxl7e88cTAQ&ab_channel=TinyTechnicalTutorials)
- [SkillCurb](https://www.youtube.com/watch?v=aYhlY9yxeEw)
- [Cloud With Django](https://www.youtube.com/watch?v=P6U89YLJ-ss&ab_channel=CloudWithDjango)
### Learning Material
- Crystal Katherine Parungao ([CKParungao](https://github.com/CKParungao))
