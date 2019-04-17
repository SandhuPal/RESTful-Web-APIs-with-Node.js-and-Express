# RESTful-Web-APIs-with-Node.js-and-Express <br>
Building RESTful Web APIs with Node.js and Express<br>


<b>npm init</b> = command to create a package.json<br>
<b>npm i --save express</b>  = Expressjs is a minimal and flexible Node.js web application framework<br>
[install the mongoDB]<br>
<b>npm i --save mongoose</b> = mongodb object modeling for node.js (writing MongoDB validation, casting and business logic boilerplate is a drag. That's why we wrote Mongoose). Mongoose provides a straight-forward, schema-based solution to model your application data. It includes built-in type casting, validation, query building, business logic hooks and more, out of the box.<br>

<b>npm i -save nodemon</b> = nodemon reload, automatically. Automatic restarting of application. Detects default file extension to monitor.<br>

<b>npm i -save-dev babel-cli babel-preset-es2015 babel-preset-stage-0</b> = Babel convert ECMAScript code into a backwards compatible version of JavaScript in current and older browsers or environments.


<b>npm i -save body-parser</b> = extract the entire body portion of an incoming request stream and exposes it on req.body. This body-parser module parses the JSON, buffer, string and URL encoded data submitted using HTTP POST request.


Robomongo (Studio 3T for mongodb) = Like postman for mongodb

//Mongoose connection
mongoose.Promise = global.Promise;
mongoose.connect("mongodb://localhost/CRMdb", {
  useMongoClient: true
});

//Body parser setup
app.use(
  bodyParser.urlencoded({
    extended: true
  })
);
app.use(bodyParser.json());
