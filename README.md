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
1. Log in to your AWS Console. Ensure that you are on the `ap-southeast-1` region.
2. Navigate to `CloudTrail`, then click `Trails` on the navigation menu.
3. Click the `Create trail` button.

![image](https://github.com/user-attachments/assets/3498a2a0-7c42-4381-bbe5-806ed48e3c47)

4. Use `management-events-yourname` for the Trail Name and choose `Create new S3 bucket` for the Storage Location.
5. Disable `Log file SSE-KMS encryption` and `Log file validation`, then click the `Next` button.

![image](https://github.com/user-attachments/assets/cd3128ad-c96c-4a9f-986f-0083f6b963c5)

6. Tick `Management events` as the event type. Keep everything as is, click `Next`, then `Create trail`.
7. Set aside and you may do various API calls, such as creating instances, buckets, tables, etc. Meanwhile, you may move onto Part 2 first.

## ✒️ Part 2: EC2 - Instance Creation
1. Navigate to `EC2`, then click `Instances` on the navigation menu.
2. Click the `Launch instances` button.

![image](https://github.com/user-attachments/assets/f32c3bbb-6991-44f7-ac64-6984110af65a)

3. Click the `Launch instances' button.
4. Use `cw-yourname` for Instance Name and choose `Windows` under the Quick Start tab. Make sure that your Amazon Machine Image (AMI) is free tier eligible.

![image](https://github.com/user-attachments/assets/4c902637-e575-4aa2-8fec-9ad8adb72738)

5. Select `Proceed without a key pair (not recommended)` under the Key Pair (Login).

![image](https://github.com/user-attachments/assets/0f108ae1-8f38-444b-83ed-cf6eb1c424bf)

6. Leave everything at default and click the `Launch instance` button. Keep this instance running for at least 30 minutes before moving onto Part 3.

## ✒️ Part 3: CloudWatch - Monitoring
1. Navigate to `CloudWatch` and click `All metrics` on the navigation menu.
2. Make sure that you are under the same region as your AWS environment from where you created your previous EC2 instance (`ap-southeast-1`).

![image](https://github.com/user-attachments/assets/39f66657-5c38-48c0-b10e-74227b0df914)

3. Click `EC2` on the namespaces, then click on `Per-Instance Metrics`.
4. Isolate the metrics of your created instance by clicking the `+` button beside the respective Instance ID of your EC2 instance.

![image](https://github.com/user-attachments/assets/44dbe5e7-e4c3-485e-bf69-f36430d1f543)

5. Tick the box of your `CPUUtilization` metric.
6. Change the date-time range of your graph by choosing `1h`.

![image](https://github.com/user-attachments/assets/b4be3b8f-d065-4985-bb30-fbeb9949db77)

7. Try different actions, such as zooming in, zooming out, and ticking multiple metrics at once. Observe what happens. Additionally, you may check out the different `Chart Types` and `Actions` for your graph.
8. Take a screenshot of the whole page and ensure that the graph and your username are visible. Here's an example:

![image](https://github.com/user-attachments/assets/b1c83ecc-71ca-4dd6-b43a-7450cf82065d)

9. Navigate back to `EC2` and choose `Instances` on the navigation menu.
10. Click the `Instance ID` of your created EC2 instance, then click the `Monitoring` tab. Observe the graphs.
11. Take a screenshot of the whole page and ensure that the graphs and your username are visible. Here's an example:

![image](https://github.com/user-attachments/assets/c207b156-a6d1-4698-8ec2-8886eb00ad96)

## ✒️ Part 4: CloudTrail - Log Check
1. 

## ✒️ Part 5: Housekeeping
**This is IMPORTANT.** Once you have finished the activity and obtained the required screenshots, **delete all created services and instances in EC2, CloudWatch, and CloudTrail to avoid incurring costs.**

## 📚 Authors
### Activity and Code Materials
- [Tiny Technical Tutorials](https://www.youtube.com/watch?v=Yxl7e88cTAQ&ab_channel=TinyTechnicalTutorials)
- [SkillCurb](https://www.youtube.com/watch?v=aYhlY9yxeEw)
- [Cloud With Django](https://www.youtube.com/watch?v=P6U89YLJ-ss&ab_channel=CloudWithDjango)
### Learning Material
- Crystal Katherine Parungao ([CKParungao](https://github.com/CKParungao))
