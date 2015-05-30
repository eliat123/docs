#Authentication
The default authentication setup for Backand applications relies on [OAuth2](http://oauth.net/2/) to provide tokenize authentication. By logging in with your username (your email address), your password, and your app name, you receive an authentication token that is valid for 24 hours. This token is required for all communication with Backand, and as such we highly recommend that you use Backand's angular infrastructure to help you save the access token. Using the [ngCookies](https://docs.angularjs.org/api/ngCookies) wrapper, you can adjust the default request header to include your current access token, greatly easing the process of securing your API communications. Backand also offers Anonymous Access, which allows you to access your application without the need to authenticate via username and password.