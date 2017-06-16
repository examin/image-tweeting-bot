# image-tweeting-bot

Twitter bot that replies(with Node.js and Heroku)

[worker: node bot.js]

This is simply the command Heroku will use to run our script file, bot.js, in Node as soon as it’s deployed.

we’ll be using the twit and node-twitterbot modules in our script file that we installed with NPM


2>??, we have to set up a stream. Fortunately, our 3rd party npm dependency twit provides an API function .stream() to do this task.



     phraseArray = [ "hey twitter",
                    "im tweeting",
                    "tweet tweet",
                    "tweetstorm time... 1/22",
                    "plz RT v important",
                    "delete ur account",
                    "it me",
                    "same",}
                    
                    
3> ??In the followed callback, we pass an event argument which gets the Twitter handle and the screen name of the user. 
In the last line, we invoke a tweetnow() function that replies back to the user who followed our bot.



4>>>  To run this bot, go to your terminal:

$node bot.js

To avoid this monotonous process, you can use npm scripts or nodemon. You can also deploy this app on Heroku for a continuous deployment.

If you are planning to deploy on Heroku, make sure to include a Procfile in the root of your directory structure and add the following line to the file:

worker: node bot.js

If you are using npm scripts, make sure you edit the scripts attribute in the package.json file:

