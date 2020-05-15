#### README

### steps

1. Install nodejs
2. Install serverless 'npm install -g serverless'
3. setup credentials 'sls config credentials --provider aws --key 'accessKeyId' --secret 'secretAccessKey''
4. create and redirect to new folder
5. Run 'sls create --template aws-nodejs'
6. open the folder and find files server.yml and handler.js
7. Add your lambda code to handler.js and edit server.yml to deploy
8. Create and verify email for SES access in aws console
9. Create table 'contactForm' with partition key 'id' of 'Number' in dynamodb
10. Run 'sls deploy' and get 'api' for sending emails
    - params : - name - emails - contactNumber - subject - message
