# Project_DevSec_Clenet

### Secure exchange with the API
I used the fuel library to do HTTP Get request.
The request are done wth the TLS certificate given by the browser (the API website is an https).
I encrypted data given by the API in files saved in the phone, to be abble to acces to the data without internet.

### Hide URL of API
I used the string.xml to hide the URL of API.

### Hide debugging information
I hid the debugging information by adding in proguard-rules.pro file these lines:
-assumenosideeffects class android.util.Log {
    public static *** d(...);
}
So this method analyses the code, and avoid to log debug information for all of its methods.

### Ensure user is the right one
I tried to install the Google SSO to restrict the access, but it doesn't work.
I commmented the code about it.

### Screenshots
![projet_1](https://user-images.githubusercontent.com/64898470/110256955-e85d0200-7f9b-11eb-893b-ab5f30fe6102.JPG)
![projet_2](https://user-images.githubusercontent.com/64898470/110256948-e004c700-7f9b-11eb-9e5d-3a8622720c5d.JPG)
