# Photo-GenieV2-Saas-upgrade (Educational Children's Game)

## Photo Genie
# Overview

This project involves the development of an educational game designed for children. The game will prompt the user to take a picture of an object that matches a given prompt. If the user submits a photo of the correct object, they will then be tasked with answering a simple question about it. Points are awarded for correctly submitting the photo and answering the question, while points are deducted for incorrect submissions.

The application will leverage various AWS services to provide its functionality, ensuring a robust and scalable solution.
## AWS Services Used

- **AWS API Gateway:** Invokes a Lambda function upon receiving an API call from the frontend.
- **AWS Lambda:** Calls Rekognition to identify image labels.
- **AWS S3 Storage:** Stores user-submitted images from the frontend for processing.
- **AWS Rekognition:** Identifies and labels user-submitted images.
- **AWS CloudWatch:** Aids in troubleshooting and logging activities.
- **AWS Cloud9:** Provides an integrated development environment (IDE) with multiple SDKs like Python, PHP, and more.
- **AWS DynamoDB (New in v2) :** Serves as the backend database to store users' points within the game.

## Other Services Used

- **HTML:** Serves as a basic frontend where users can submit images.

## Project Architecture V2

<p align="center">
  <img src="https://i.imgur.com/FtFldY3.png" alt="Architecture Diagram" width="80%" height="80%">
  <br>
  <strong><small>Figure 1: Simple Architecture Diagram.</small></strong>
</p>

### 5. Project Video Demo
[View the video demo here](https://youtu.be/VjaLsgd4SuA).
