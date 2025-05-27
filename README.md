# Serverless Event Feedback System Using AWS

## Project Description

The **Serverless Event Feedback System** is a cloud-native application designed to automate feedback collection for seminars, workshops, and similar events. Leveraging AWS services like API Gateway, Lambda, DynamoDB, and SES, this system eliminates the need for traditional server infrastructure. It ensures real-time feedback processing, secure data handling, and automated email notifications to event organizers.

## Features

- Responsive web-based feedback form
- Real-time feedback submission and processing
- Backend logic with AWS Lambda (Python)
- Secure and scalable data storage using Amazon DynamoDB
- Automated email alerts using Amazon SES
- Secure access control using IAM roles and policies
- CloudWatch integration for monitoring and debugging
- Fully serverless, scalable, and cost-efficient design

## Technologies Used

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: AWS Lambda (Python)
- **Cloud Services**: 
  - Amazon API Gateway
  - AWS Lambda
  - Amazon DynamoDB
  - Amazon Simple Email Service (SES)
  - IAM (Identity and Access Management)
  - CloudWatch (for logs and monitoring)

## Screenshots

### Feedback Form
![Feedback Form](#)
![Screenshot 2025-05-14 165519](https://github.com/user-attachments/assets/935f8476-0578-4685-a037-b2c5c809b271)

*Clean and responsive form with fields for name, email, event type, ratings, and comments.*

### Submission Confirmation
![Success Popup](#)  
![Screenshot 2025-05-14 165637](https://github.com/user-attachments/assets/2a94705b-612a-4cfa-a6d6-2cd3e44e83fe)

*Confirmation alert indicating successful feedback submission.*

### Email Notification
![Email Screenshot](#)  
![Screenshot 2025-05-14 165727](https://github.com/user-attachments/assets/39f491ff-5314-4354-87ba-d8929306846b)


*Automated email with submitted feedback details received by the event organizer.*

## Installation & Deployment

> ⚠️ This project requires an AWS account with access to API Gateway, Lambda, DynamoDB, and SES.

1. **Clone this repository**
   ```bash
   git clone https://github.com/Niki654/Serverless-Event-Feedback-System.git
   cd Serverless-Event-Feedback-System
   ```
   
2. **Set Up AWS CLI**
   ```bash
   aws configure
   ```
   
3. **Create DynamoDB Table**
  - Go to **AWS Console → DynamoDB**.
  - Create a new table named **EventFeedback**.
  - Set `feedback_id` (or a similar field) as the **Primary Key**.

4. **Deploy Lambda Function**
  - Go to **AWS Console → Lambda**.
  - Create a new function (e.g., `processFeedback`).
  - Upload the backend code from this repository.
  - Attach necessary **IAM permissions** to allow access to **DynamoDB** and **SES**.

5. **Configure API Gateway**
  - Create a new **HTTP API** or **REST API** in the **API Gateway** console.
  - Set up a **POST** method and link it to your Lambda function.
  - **Deploy** the API and **copy the endpoint URL** for use in the frontend.

6. **Set Up Amazon SES**
  - Go to **Amazon SES Console**.
  - **Verify your sender email address**.
  - Update your Lambda function code to use the verified email and correct SES **region**.

7. **Set Up Frontend**
  - Open or host `index.html` using a local browser or **S3 static website hosting**.
  - Update the form's `action` or JavaScript code to include your **API Gateway URL**.

8. **Test the System**
  - Fill out and submit the feedback form.
  - Check **DynamoDB** to confirm that the feedback has been stored.
  - Verify that the **notification email** is received by the event organizer.
    
9. **Project Completed**
  

