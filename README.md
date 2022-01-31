# Udacity Private Blockchain Application

#### This application allows to register the stars and it knows who own the star.

#### 1. To run this application
 ```bash
     `node app.js`

    > Server Listening for port: 8000
 ```

#### 2. The application will create a Genesis Block when we run the application.

![Request: http://localhost:8000/block/height/0](Screenshots/1%20Postman%20Genesis%20Block.png)


#### 3. The user will request the application to send a message to be signed using a Wallet and verify the ownership. 
The message format will be: `<WALLET_ADRESS>:${new Date().getTime().toString().slice(0,-3)}:starRegistry`;

![Request: http://localhost:8000/requestValidation](Screenshots/2%20Request%20of%20ownership.png)

#### 4. Sign the message with your Wallet:

![Use the Wallet to sign a message](Screenshots/3%20Sign%20the%20message.png)

#### 5. Verify the message 

![Verify the message](Screenshots/4%20Verify%20the%20message.png)

#### 6. Submit the star

![Request: http://localhost:8000/submitstar](Screenshots/5%20Submit%20my%20Star1.png)

![Request: http://localhost:8000/submitstar](Screenshots/6%20Submit%20my%20Star2.png)

#### 7. Retrieve Stars owned

![Request: http://localhost:8000/blocks/<WALLET_ADDRESS>](Screenshots/7%20Retrieve%20Stars.png)


