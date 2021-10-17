1. Install Amplify CLI using 
    npm i -g @aws-amplify/cli
    
2. Configure AWS Amplify
    amplify configure
    
3. Bootstrap react app 
    npx create-react-app todo-amplify

4. Init BE
    cd todo-amplify
    amplify init
    
5. Setup FE app 
    npm install aws-amplify @aws-amplify/ui-react --save

6. Connect Amplify in FE app
    src/app.js, import Amlify, awsExports, Amplify.configure

7. Create a GraphQL API
    amplify add api
    modify schema at amplify/backend/api/todo-api/schema.graphql
    amplify push

8. Connecting FE to API
    modify crs/app.js
    amplify push

9. Authenticaiting Users
    amplify add auth -- choose Cognito
    amplify push

10. Run locally
    npm start, localhost:3000 in browser.
    
10. Deploying the app
    amplify add hosting
    amplify publish
    
11. Delete all the resources
    amplify delete
    
 
