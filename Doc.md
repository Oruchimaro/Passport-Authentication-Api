### Step 1
    Install Passport package and add it to providers array in config.php

### Step 2
    Run the migrations then we need to We need to install laravel 
    to generate passport encryption keys. This command 
    will create the encryption keys needed to generate secure access tokens. 
    like secret key and secret id.

### Step 3
    Open App/User.php file and put the code on App/User.php File .
    Next Register passport routes in App/Providers/AuthServiceProvider.php,
    Go to App/Providers/AuthServiceProvider.php and 
    put this => Register Passport::routes(); inside of boot method .

### Step 4
    Next, go to config/auth.php and Change the API driver to the session to passport. 
    Put this code ‘driver’ => ‘passport’, in API 

### Step 5
    Add the API routes to api.php  and create the AuthController.
    then add the login, register, and getUser methods in it.


### Step 6
    Make Requests with Postman to test and debug.
    Call login or register apis put $accessToken. 
    ‘headers’ => [
    ‘Accept’ => ‘application/json’,
    ‘Authorization’ => ‘Bearer ‘.$accessToken,
    ]

    Pass Header in login/register rest API, it is necessary to passport
    authentication
    in laravel app.
