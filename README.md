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
*Clean and responsive form with fields for name, email, event type, ratings, and comments.*

### Submission Confirmation
![Success Popup](#)  
*Confirmation alert indicating successful feedback submission.*

### Email Notification
![Email Screenshot](#)  
*Automated email with submitted feedback details received by the event organizer.*

## Installation & Deployment

> ⚠️ This project requires an AWS account with access to API Gateway, Lambda, DynamoDB, and SES.

1. **Clone this repository**
   ```bash
   git clone https://github.com/yourusername/serverless-feedback-system.git
   cd serverless-feedback-system
