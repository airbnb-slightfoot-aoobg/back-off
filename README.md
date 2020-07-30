# back-off

EMAIL CONTROLLER

GET https://kmcgeeka-airbnboptimal.herokuapp.com/useremails/useremails
-it works and only data and admin can access
-gets a list of all emails and their associated users 

GET https://kmcgeeka-airbnboptimal.herokuapp.com/useremails/useremail/6
-it works and only data and admin can access
-gets a specific email by the email’s id associated with a specific user 

DELETE https://kmcgeeka-airbnboptimal.herokuapp.com/useremails/useremail/6
-it works and only data and admin can access
-deletes an email associated with a user

PUT https://kmcgeeka-airbnboptimal.herokuapp.com/useremails/useremail/{usermailid}/email/{useremail}
-it works and only data and admin can access
-replaces a specific email associated with a specific user

-POST https://kmcgeeka-airbnboptimal.herokuapp.com/useremails/user/{userid}/email/{useremail}
-it works and only data and admin can access
-adds a new email to a specific user 

USER CONTROLLER
-GET https://kmcgeeka-airbnboptimal.herokuapp.com/users/users
-it works and anyone can access
-gets a list of all users

-GET https://kmcgeeka-airbnboptimal.herokuapp.com/users/user/{userid}
-it works and only admin can access
-gets a specific user by id

-GET https://kmcgeeka-airbnboptimal.herokuapp.com/users/user/name/{username}
-it works and only ADMINs can access
-returns the user with the username 

-GET https://kmcgeeka-airbnboptimal.herokuapp.com/users/myinfo
-This returns the authenticated user’s profile

-GET https://kmcgeeka-airbnboptimal.herokuapp.com/users/user/name/like/{likename}
-send part of a username, and it returns all users with likenames
-only valid for ADMINS

-PATCH https://kmcgeeka-airbnboptimal.herokuapp.com/users/user/{userid}
-only the authenticated user can update a part of their user credentials

-PUT https://kmcgeeka-airbnboptimal.herokuapp.com/users/user/{userid}
-only the authenticated user can update all their credentials at once

-POST https://kmcgeeka-airbnboptimal.herokuapp.com/users/user
-only ADMINs can add a brand new user from this endpoint

-DELETE https://kmcgeeka-airbnboptimal.herokuapp.com/users/user/8
-only the authenticated user can delete themselves 

-POST https://kmcgeeka-airbnboptimal.herokuapp.com/createnewuser
-anyone can access and creates a new user

LISTINGS

GET https://kmcgeeka-airbnboptimal.herokuapp.com/listings/listings
-gets a list of all listings
-anyone can access

GET https://kmcgeeka-airbnboptimal.herokuapp.com/listings/listing/{id}
-gets a specific listing by the listing id
-anyone can access

POST https://kmcgeeka-airbnboptimal.herokuapp.com/listings/user/{userid}
-creates a new full listing to a specific user with the user id passed in
-does not call DS API currently 

POST https://kmcgeeka-airbnboptimal.herokuapp.com/listings/listing/create
-creates a new listing
-only authenticated user can call this and create this
-calls DS backend and creates price

PATCH        https://kmcgeeka-airbnboptimal.herokuapp.com/listings/listing/{listingid}
-updates just a part of a listing by passing the listing id 
-only the user who owns the listing can do this
-calls the DS backend and gets a new price

DELETE 
https://kmcgeeka-airbnboptimal.herokuapp.com/listings/delete/{listingid}
-deletes a listing by its’ id
-only a user who owns the listing can delete a listing

https://kmcgeeka-airbnboptimal.herokuapp.com/login
-Logins in a user
https://kmcgeeka-airbnboptimal.herokuapp.com/logout
logs out a user

Heroku
https://kmcgeeka-airbnboptimal.herokuapp.com/





