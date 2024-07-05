

# Firebase Authentication

Upon successful sign-up or sign-in, Firebase creates an _Auth instance_for the user and provides a unique auth token to identify each user. Whenever a user makes a request to a Firebase resource or service, these auth tokens are sent along with the request. Firebase services, respond to these requests and grant access to Firebase services according to users’ permissions. The Auth instance then persists the current user’s state. This prevents the user from logging out if they refresh the browser or page.

# Email and Password Authentication  

Sign up users with de Auth SDK.

The `createUserWithEmailAndPassword` function takes three arguments. The first argument is the `auth` object that represents the initialized `auth`instance. Then, it takes the `email` and `password` values that we obtain from our client-side input fields. This function is asynchronous and takes some time to complete. Therefore, we can attach a JavaScript promise (Text in the key: The Promise object represents the eventual completion (or failure) of an asynchronous operation and its resulting value.) that allows us to handle the function’s success value or failure reason.

