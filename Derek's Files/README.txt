COMP20: Assignment 5
Author: Derek DuPont

Collaborations: Discussed how to set up MongoDb and how to implement the post API with
Tommy Folliard.

Approximately ~15 hr were spent on this project (mostly in learning how to use Mongo and Heroku)

POST API:
	I tested this using:
		curl --data "game_title=...&username=...&score=..." http://localhost:3000/submit.json
	I didn't have time to implement in my frogger problem, but using the curl command,
	I was able to post data into my Mongohq database successfully.
	Unfortunately, I don't have any error checking currently. The essential data fields
	are not enforced.
	
GET API:
	I could not figure out how to appropriately extract the game_title from the URI,
	so this API is not working.
	
INDEX:
	Currently succeeds in displaying all scores. It is not very fancy, just listing them
	in the order they appear.
	
USER SEARCH:
	Has the input box and button, but for some reason, upon calling the form's post
	method, no data is submitted (request.body returns nothing), so this isn't working.
	
Side note: I'm not sure where all my git commit messages have been going...