# AUTHENTICATION

> Amazon Cognito: Amazon Cognito is a robust user directory service that handles user registration, authentication, account recovery & other operations.

- The Amplify Framework uses Amazon Cognito as the main authentication provider.
- The Amplify Auth category provides an interface for authenticating a user.

- Configure Auth Category: To start provisioning auth resources in the backend, go to your project directory and execute the command:
`amplify add auth`.
Then push the changes to the backend. by: `amplify push`

- The Auth category can be used to register a user, confirm attributes like email/phone, and sign in with optional multi-factor authentication.

- The next step in the *sign up* flow is to confirm the user. A confirmation code will be sent to the email id provided during sign up. Enter the confirmation code received via email in the `confirmSignUp` call.

### Resources
- [Amazon Cognito](https://aws-amplify.github.io/docs/android/authentication)