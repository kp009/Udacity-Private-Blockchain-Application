# Udacity Private Blockchain Application

#### This application allows to register the stars and it knows who own the star.

#### To run this application
 ```bash
     `node app.js`

    > Server Listening for port: 8000
    ```

#### The application will create a Genesis Block when we run the application.

![Request: http://localhost:8000/block/height/0 ](Screenshots/1 Postman Genesis Block.png)

#### The user will request the application to send a message to be signed using a Wallet and in this way verify the ownership over the wallet address. The message format will be: `<WALLET_ADRESS>:${new Date().getTime().toString().slice(0,-3)}:starRegistry`;

![Request: http://localhost:8000/requestValidation ](Screenshots/2 Request of ownership.png)

#### Sign the message with your Wallet:

![Use the Wallet to sign a message](Screenshots/3 Sign the message.png)

#### Verify the message 

![Verify the message](Screenshots/4 Verify the message.png)

#### Submit the star

![Request: http://localhost:8000/submitstar ](Screenshots/5 Submit my Star1.png)

![Request: http://localhost:8000/submitstar ](Screenshots/6 Submit my Star2.png)

#### Retrieve Stars owned

![Request: http://localhost:8000/blocks/<WALLET_ADDRESS> ](Screenshots/7 Retrieve Stars.png)

#### Output

![Output](Screenshots/8 Output.png)
