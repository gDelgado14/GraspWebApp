#[GraspWebApp](https://grasplock.firebaseapp.com/)

![GraspLogo](http://grasplock.com/images/GraspWhiteSlogan.png)

##Main Stuff

* [index](index.html) contains the login form
* [dashboard](dashboard.html) contains the app itself
* [access](access.html) contains calendaring widget - **in progress**


###Completed

* You are able to log in & log out
* You are able to register & log in simultaneusly
* Redirects: 
	* Dashboard checks if user is logged in - else redirects to index
	* Index redirects to dashboard if already logged in
* app writing to Firebase
	* current JSON tree looks like: 
	
```
grasplock: {
	users: {
		user1: {
			lock: true
		},
		user2: {
			lock: true
		},
		user3: {
			lock: true
		},
		...
}
```

> When a user registers, they get assigned a key value pair of {lock: true} for testing purposes. See [here](index.html#L301).


###To-Do
* Reading data from Firebase
* Add additional pages for each icon


###Attribution:

Using [Bare](http://startbootstrap.com/template-overviews/bare/) HTML starter template for [Bootstrap](http://getbootstrap.com/) created by [Start Bootstrap](http://startbootstrap.com/).

> Copyright 2013-2015 Iron Summit Media Strategies, LLC. Code released under the [Apache 2.0](https://github.com/IronSummitMedia/startbootstrap-bare/blob/gh-pages/LICENSE) license.