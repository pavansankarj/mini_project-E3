# mini_project-E3

Here's the proposed method

I proposed a face recognition-based login system for our SMS to ensure security and to reduce human effort for manual entry of details at the login page. This system just tries to 
recognize the faces which it encounters through the webcam and logs into his/her SMS by fetching the details from the database. First, I encode images of all of the students, and store 
them with their respective IDs in the database. We also store the passwords of the students in encrypted format using fernet algorithm. Then at the time of recognition, I to encode the faces of the webcam 
and compare them with the stored encodings. If a match is found I fetch his/her encrypted password and decrypt it using the fernet algorithm which runs in CBC mode of AES. Then I 
open the browser to the SMS site, followed by feeding the username and password to it and then logging into SMS through browser automation i.e., with the help of selenium.

Note: To execute this application and to log in to your SMS, you need to have "chromedriver.exe" downloaded and put in the same folder i.e., where you have this "recognize.exe" file
