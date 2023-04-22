# Test Plan and Results
I will be doing testing the backend components of the software and checking their implementation. I want to make sure the tests can produce the same expected results repeatedly. I will also be testing the front-end components to verify that all components are working properly. These tests will be done in a local version of the program as well as a production deployed version.

## 
1.1 R-AC\
1.2 Tests the response of the recipe API call and the data received.\
1.3 For this test a get call will be made to the MealDB API and the local web console will be checked for JSON data.\
1.4 A recipe string.\
1.5 Returns a JSON of an array of recipes.\
1.6 Normal\
1.7 WhiteBox\
1.8 Functional\
1.9 Unit

##
2.1 AI-AC\
2.2 Tests the response of the OpenAI API call and the data received.\
2.3 For this test a post and get call will be made to the OpenAI API and the local web console will be checked for JSON data.\
2.4 A string requesting a recipe.\
2.5 Returns a response JSON file.\
2.6 Normal\
2.7 BlackBox\
2.8 Performance\
2.9 Unit

##
3.1 FBA-S\
3.2 Tests the firebase account creation process.\
3.3 For this test a post will be made to the Firebase API and the local web console will check for a response code, as well as check the DB to see if it was populated with an account.\
3.4 A username and password user provided.\
3.5 Returns a confirmation that user has signed up as well as updated DB with account.\
3.6 Normal\
3.7 WhiteBox\
3.8 Functional\
3.9 Unit

##
4.1 FBA-L\
4.2 Tests the firebase authentication of an account.\
4.3 For this test a get call will be made to the Firebase API and the local web console will check for a response code, as well as check the URL for login data.\
4.4 A valid username and password that is already present in the database.\
4.5 URL data has valid login information.\
4.6 Normal\
4.7 WhiteBox\
4.8 Functional\
4.9 Unit

##
5.1 Page Navigation\
5.2 Tests the various navigation between pages.\
5.3 This will test the referencing between different files in the project by going through all the links and checking the different pages.\
5.4 None.\
5.5 All pages can be navigated to and from.\
5.6 Normal\
5.7 WhiteBox\
5.8 Functional\
5.9 Integration

##
6.1 Random Dish Generator\
6.2 Tests the generating of a random dish.\
6.3 For this test a get call will be made to the MealDB API and the local web console will be checked for JSON data and repeated multiple times to insure randomness.\
6.4 None.\
6.5 A JSON file with a dishes data, random each time it is called.\
6.6 Normal\
6.7 WhiteBox\
6.8 Functional\
6.9 Unit

##
7.1 Dish Database\
7.2 Tests the ability to search the whole recipe database and generating cards for all of them.\
7.3 For this test a get call with input data to filter will be made to the MealDB API and the output will be returned on screen with all the dishes, this will rely on other tests working first.\
7.4 A random ingredient string.\
7.5 An JSON with an array of Dish data that is then put into individual cards.\
7.6 Normal\
7.7 WhiteBox\
7.8 Functional\
7.9 Unit

##
8.1 Custom Recipe Generator\
8.2 Tests the ability to provide input and receive a custom dish and recipe generated by AI.\
8.3 For this test a post and get call with provided input will be made to the OpenAI API and the output will be returned to the user on screen.\
8.4 A randomly specific recipe request string.\
8.5 A JSON response that is then output to the user.\
8.6 Normal\
8.7 BlackBox\
8.8 Performance\
8.9 Unit

##
9.1 Recipe Card Format\
9.2 Tests to see if data being pulled from recipe API is formatted correctly in custom recipe cards.\
9.3 This test will grab the JSON data and format it into custom recipe cards with two separate views, one concise view and another detailed view.\
9.4 The JSON data from the recipe API.\
9.5 A well formatted recipe card with recipe data pulled.\
9.6 Normal\
9.7 WhiteBox\
9.8 Functional\
9.9 Integration

##
10.1 UI Functionality\
10.2 Tests to see if all buttons and links are properly working and pointing to correct locations.\
10.3 For this test all button or links the user will be interacting with will be tested to see if they all work.\
10.4 None.\
10.5 All buttons and links actions work and provide a response.\
10.6 Normal\
10.7 WhiteBox\
10.8 Functional\
10.9 Integration