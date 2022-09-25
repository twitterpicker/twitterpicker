<img src="https://raw.githubusercontent.com/twitterpicker/twitter-picker/main/public/logo.png" data-canonical-src="https://raw.githubusercontent.com/twitterpicker/twitter-picker/main/public/logo.png" width="200" height="200" style="margin: auto" />

# Picker
## Showcase & Documentation




# Developer Documentation


The product has a cluster of two core backend services running, that rely on one storage layer.

# **Backend Services:** 

 - **Internal API :** 
	 
	  - Endpoint :  `/api/get-winner/${tweetID}`
	  - returns **winner stored in database** or **error object** if no winner found.
	
	  
	

 - **Direct Message server :** 
	 -	
	 - Intercepts user's message to the bot account.
	 - detects the **"tweetID"** from the **"tweet status URL"**
	 - gets the winner from the storage layer, using the **"internal API"**
	 - send message about the winner of the giveaway to the user
	 
