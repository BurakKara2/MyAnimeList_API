# MyAnimeList_API
MyAnimeList Creat Collection 
Login the https://myanimelist.net/
Click the account settings
Click the API tab
Click the Create ID
After fill the empty fields, and press the save button
Expected Result: Client ID and Client Secret	were created

Auth Collection:
GET method https://myanimelist.net/v1/oauth2/authorize
Required Params field;
response type : code
client_id : your client id at the myanimelist api field
code_challenge : https://tonyxu-io.github.io/pkce-generator/ (A minimum length of 43 characters and a maximum length of 128 characters.)

after create the URL , go to link from any browser
after click the allow button , creat the code

MyAnimeList Collection:
Post method https://myanimelist.net/v1/oauth2/token
Required Params field;
client_id : your client id at the myanimelist api field
grant_type : authorization_code
code : see the code value at the browser , copy-paste it
code_verifier : https://tonyxu-io.github.io/pkce-generator/ (A minimum length of 43 characters and a maximum length of 128 characters.)
client_secret : your client secret at the myanimelist api field
Expected Result: Get the token successfully
