# Chat_Service-gRPC

## Project Description

-This project involves a messaging service where a user can send and receive messages from a specific user.

-A graphical user interface is available to facilitate the use of the application.

-Upon execution, an interface will appear where the user must enter their username and password, then choose to log in or sign up.

-Once logged in, they can enter the username of the user they wish to message and the message itself, then use the "Send" button to send the message.

-Once the message is sent, it will immediately appear on the recipient's interface.

-All accounts will remain as long as the server is running.

-Connections are well managed, so no problems can arise.

### Notes

-Case sensitive

-A username must contain only letters, numbers, and the "_" character, and it must start with a letter.

-A password must be at least 8 characters long and must contain an uppercase letter, a number, and a special character.

#### Example

##### username: adem

##### password: Adem123*

-Two users cannot log in to the same account at the same time.

-A username is unique.

-A user can only send messages to a connected user; otherwise, an error will appear.

-All messages are private between the sender and the recipient.

-In the login interface, the user can close the application normally. But in the chat interface, the user must press the "Close" button to close the application for management reasons.

### Deployment

##### First Method:

You can take all the files and simply run MessagingServer.java, then MessagingClient.java (as many times as needed).

##### Second Method:

1. Create a Maven project.

2. Copy the pom.xml file and run it with mvn install.

3. Copy the messaging.proto file into the resources folder and run the command mvn clean compile.

4. Create a folder under java and call it Messaging, then copy the MessagingServiceImpl.java file into it.

5. Copy the MessagingServer.java and MessagingClient.java files under java, then run them respectively.
