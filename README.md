Companies nowadays are now turning their businesses online to provide their customers a better experience. One of the most popular e-commerce website we hear often is Ebay – an American multinational company running on Node.js . A lot of folks are suggesting that Node.js might be the future of web development. Node.js is a single-threaded event-driven system that runs fast even when handling lots of requests at once, it is also simple compared to traditional multi-threaded frameworks. Node.js is well suited for real-time applications: online games, collaboration tools, chat rooms, or anything where what one user (or robot?) does with the application needs to be seen by other users immediately, without a page refresh. Using a technique known as “long-polling”, you can write an application that sends updates to the user in real time.

## Demo
This simple e-commerce application demonstrates CRUD operations using mongoDB and a simple implementation of a session based user authentication using Passport.js. It also utilizes real time update front-end products using socket.io.  This web app is 100% free to use, you can customize it to build a more sophisticated e-commerce web application. Feel free to submit an issue on GitHub if you found any bug or even better – submit a pull request.

This web application is currently hosted on Heroku, [click here](https://evening-cove-56191.herokuapp.com/) to view the demo. Heroku is for testing only - it does not support file uploads as the filesystem is readonly. Although you can still test the image upload functionality but all images will automatically be deleted after a couple of minutes.

## How do I get setup?
1. Create a folder called "data" in the root directory of our nodejs project. This is where MongoDB documents will be stored.
2. Go to MongoDB installation directory and under the bin folder run this command: `mongod --dbpath C:\Users\Carl\Documents\nodejs-ecommerce\data` This will start the MongoDB server. Leave this CLI  instance open and start another CLI instance.
3. In the new CLI, navigate to where you pulled this repository, ex. `C:\Users\Carl\Documents\nodejs-ecommerce`, then type-in: npm install then wait till it finishes installing all the modules required to run our Node.js Web Application.
4. Once the installation is completed, type in the following command to run our Web Application: npm start  Make sure to keep the CLI opened.
5. Now go to [http://127.0.0.1:3100/](http://127.0.0.1:3100/) using your favorite browser.


## Modules Used
+ async
+ connect-flash
+ cookie-parser
+ crypto-md5
+ express
+ express-session
+ jade
+ mongodb
+ monk
+ multer
+ passport
+ passport-local
+ socket.io