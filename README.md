# ☁️ CloudWatch and CloudTrail 101: Logging and Monitoring with AWS ☁️

Amazon Relational Database Service (Amazon RDS) is an easy-to-manage relational database service optimized for total cost of ownership. It is simple to set up, operate, and scale with demand. In this activity, you will learn how to create, manage, and scale your own database in the cloud using Amazon RDS.

**Disclaimer:** This activity is based on Sanjeev Thiyagarajan's [tutorial](https://youtu.be/ylmwaDUMV9c?si=jGnEN8NObwqD8-jc&t=421).

## 📋 Requirements
1. **Browser** (Google Chrome, Microsoft Edge, Opera GX, etc.)
2. **AWS Account**
3. [**pgAdmin 4**](https://www.postgresql.org/ftp/pgadmin/pgadmin4/v9.0/windows/)

## 🎯 Objectives
1. **Create an RDS Instance** and configure security for access.
2. **Define Database schemas and tables.**
3. **Launch an EC2 Instance** for hosting the app.
4. **Connect the App to RDS** using the connection string.

## ✒️ Part 3: Housekeeping
1. Once you have finished the activity and obtained the required screenshots, delete all created services and instances in RDS and in the pgAdmin app to avoid incurring costs.
2. Select the radio button of `my-first-db`, then click on `Actions`->`Delete`.

![image](https://github.com/user-attachments/assets/fc5113c2-19f8-4a9f-a703-b47d2580551c)

3. Deselect the ticked boxes `Create final snapshot` and `Retain automated backups`.
4. Tick on the deletion acknowledgment box then type `delete me` as a confirmation.

![image](https://github.com/user-attachments/assets/fa759fc9-fe12-46be-a5cd-3b0d6f711961)

5. Disconnect and delete the databases `myapp` and `aws-rds` then remove the PostgreSQL server in the pgAdmin application.

## 📚 Authors
### Activity and Code Materials
- Sanjeev Thiyagarajan ([KodeKloud](https://youtu.be/ylmwaDUMV9c?si=jGnEN8NObwqD8-jc&t=421))
### Learning Material
- Crystal Katherine Parungao ([CKParungao](https://github.com/CKParungao))
