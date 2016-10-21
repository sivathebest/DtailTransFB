# DtailTransFB
Its latest Facbook Loing App.

###### Updated to Android API Level 24
###### Min Android API Level 15
###### Facebook API 'com.facebook.android:facebook-android-sdk:4.16.1'

This Application is simple Facebook Login Application. This uses Facebook API to get user information from facebook. Its easy way to login and signup.It updated to the latest version in both Facebook API and Android API. The current app will get only the access token from facebook with username. You can get more information about the user by adding permission and code in the below part of MainActiviy. 

            ```
            @Override
            public void onSuccess(LoginResult loginResult) {
                // App code
                info.setText(
                        "User ID: "
                                + loginResult.getAccessToken().getUserId()
                                + "\n" +
                                "Auth Token: "
                                + loginResult.getAccessToken().getToken()
                );
                
                // Your extra code goes here to get more information about the user. 
            }
            ```
