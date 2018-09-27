app name : thawing-falls-93934

elena@DESKTOP-1RKFQF4 MINGW64 ~/Desktop/Bootcamp/Homework For Github/Oddly-Enough (master)
$ git remote rename heroku heroku-Oddly-Enough

elena@DESKTOP-1RKFQF4 MINGW64 ~/Desktop/Bootcamp/Homework For Github/Oddly-Enough (master)
$ git remote
heroku-Oddly-Enough
origin

Created mongolab-rectangular-20244 as MONGODB_URI
Use heroku addons:docs mongolab to view documentation



13. When you go to connect your mongo database to mongoose, do so the following way:

// If deployed, use the deployed database. Otherwise use the local mongoHeadlines database
var MONGODB_URI = process.env.MONGODB_URI || "mongodb://localhost/mongoHeadlines";

// Set mongoose to leverage built in JavaScript ES6 Promises
// Connect to the Mongo DB
mongoose.Promise = Promise;
mongoose.connect(MONGODB_URI);