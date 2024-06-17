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

## Updated Saas User points implementation and Highscores

In the original Photo Genie project, the application simply told users what the image they submitted was. In version 2, I had the idea of transforming that base concept into an educational children's game. Instead of merely identifying the submitted photo, the application now instructs the user to take a photo of a specific object and then prompts them to answer a question about it. This exciting approach encourages children to take photos of objects around the house or outside, helping them learn through interactive quizzes. This also allowed me to set up a simple high scores function so users worldwide can see the amount of points other users have accumulated.

To support this functionality, I integrated DynamoDB into the architecture to store user data and points. In version 3, I plan to add Amazon Cognito to provide login functionality for the application. Currently, users are prompted to input their name before submitting their photo, so their data can be stored in the database. Once the login functionality is implemented in version 3, this step will no longer be necessary, as user sessions will be linked to their login information.

<p align="center">
  <img src="https://i.imgur.com/FJyDnBd.png" alt="Architecture Diagram" width="80%" height="80%">
  <br>
  <strong><small>Figure 2: Users promoted with an object to take a photo of.</small></strong>
</p>

<p align="center">
  <img src="https://i.imgur.com/85piamJ.png" alt="Architecture Diagram" width="80%" height="80%">
  <br>
  <strong><small>Figure 3: DynamoDB implementation.</small></strong>
</p>


### Project Video Demo V2
[View the video demo here](https://youtu.be/VjaLsgd4SuA).
