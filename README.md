Lab Test 1 - Stefan Kepinski - 101356431

I could only fit so much in every screenshot in terms of code. I wanted to make a video but my OBS was giving me trouble. 

Overall notes: most functionality present. could not figure out retrieving older messages in socket. Did not know how to do private messages.
Did not have time to make it look nice with CSS.

What does work: Signup, login (both save to mongoDB). messages are displayed in chat room pages and shown in console. did not make username dynamic based on user though.
Tried to deploy my project as a page on github, but got a 404 error. Did not have time to troubleshoot.

Below is a portion of my server.js. I implemented the various socket methods that were shown to us in the lab. The server is set up and called when ran.

I created get method for the messges that were saved in the database, but I did not end up figuring out how to implement the retrieval in socket.io
![serverjs](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/f58a50bb-3012-4eca-9408-58e855d4a72c)

Various HTML pages for displaying web pages:

chat.html
just contains buttons that take you to the chat rooms
![chathtml](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/6484cf5a-f267-4db0-8d81-06983d257a03)

chatroom.html
this page contains the front end deployments of the socket.io. I mostly only was able to implement the ones that we went over in class.
I was not sure how to do "user typing...."
![chatRoomhtml](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/b40ea6af-2792-42b5-88bd-6ceb362eaf8a)

login.html
Not much to say about this. Form for login
![loginhtml](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/abcfd1b5-dd11-430c-be4f-2c8984469de6)

login.js
attempt at doing local storatge for user info from the login. I honestly got too focused on trying to make socket.io work that I didn't really implement it further 
after trying to pass it to chat.html
![loginjs](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/cb5dd149-0777-4b07-ac64-5b188fe9de12)

signup.html
Form for signup
![signuphtml](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/ec1bfa2a-45dc-4609-abb3-b9cd3ac5e65c)

signup.js

backend for html form. takes user info and saves it to the mongoDB. if everything is good it passes the user to login
![signupjs](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/3736999b-da0e-4ae3-8650-e15da155fed4)

I think I forgot to upload this one in the submitted folder, but this is the packend post route for the signup.js
![image](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/df01b8d2-c08d-4491-8ba6-11edea556df0)

Model for user:
![mongoUser](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/de5cceb1-a8b8-4610-9fbb-c90aaed17fba)

Model for messages:
![mongoMessagesCode](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/2432c96c-09e0-493d-bcef-8dc927fbdac4)

Output Examples:

![roomExample](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/e8e91230-d5ac-4093-9c72-6c44068db957)
![roomExample2](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/e9233feb-8cf1-4de0-8413-e64696d206d2)
![consoleLogRoomActivity](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/a4a0b910-1a1d-4ba2-a878-4c88c5816f5b)
![homepage](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/5471fe5a-ab42-4421-8fa4-ecb45d4270fc)
![signup](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/067c1cbe-b6f2-48da-9ebc-067b71caab5a)
![mongoValidationExample](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/9d8c0c76-e590-45f4-b33e-1628497d98fd)
![login](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/9a20cdb9-9850-4ed4-bed1-59a0f4103cce)
![mongoUsers](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/4b372a29-6947-4b56-8b7a-4940e4498657)
![mongoMessages](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/013dc33b-5868-42f8-a08c-99b199c4b52d)
![attemptedPageDeployment](https://github.com/stefk13/101356431_lab_test1_chat_app/assets/123743947/ebfad7d4-00db-4951-a812-287bb56f6846)
