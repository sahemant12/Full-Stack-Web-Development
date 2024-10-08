# Full-Stack-Web-Development
This repo contains the roadmap and the full-stack web development notes along with video link from different YouTube Channel.

## Roadmap
- HTML
- CSS
- JavaScript
- React
- Redux
- Nodejs and ExpressJs
- MongoDB
- Linux
- DevOps
- Tailwind
- TypeScript
# HTML
1. Tag:
   - `<div>,<p>` : block-tag
   - `<span>` : inline-tag
2. Semantic Elements:
   - Examples of non-semantic elements: <div> and <span> - Tells nothing about its content.
   - Examples of semantic elements: `<form>, <table>, and <article>` - Clearly defines its content.
   - More E.g: `<section>, <article>, <header>, <nav>, <main> --> <section>, <footer>, <aside>`
3. Form Elements:
   - For input type use label. E.g: `<lable>Name</lable> <input type="text>`
   - `<button type="button onclick="alert('Hello World!')">Click Me!</button>`
   - `<fieldset>`
# CSS
1. Selector in CSS:
   - Type Selector : h1{ } 
   - Universal Selector : *{ } 
   - Class Selector : *class-name{ }
   - id Selector : #id-name{ } 
   - Attribute Selector : a[href="www.example.com"] { }
   - Pseudo-class Selector : p:first-child { } E.g: hover, visited, 
   - Pseudo-element Selector : p::first-line { }
   - Descendant combinator : article p
   - Child combinator : article>p
   - Adjacent Sibling Combinator : h1+p
   - General Sibling Combinator : h1~p
2. Position
   - static : An element with position: static; is not positioned in any special way; it is always positioned according to the 
            normal flow of the page.
   - relative : An element with position: relative; is positioned relative to its normal position. (E.g: position: relative;
  left: 30px; )
   - fixed : An element with position: fixed; is positioned relative to the viewport, which means it always stays in the same place even if the page is scrolled. (E.g: position: fixed; )
   - absolute : An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed) (E.g: position: absolute;)
   - sticky : The sticky element sticks to the top of the page (top: 0), when you reach its scroll position(One of example).
3. FlexBox
   - flex-direction : (E.g: display: flex; flex-direction: column, row;)
   - flex-wrap : (E.g: display: flex; flex-wrap: wrap, nowrap, wrap-reverse, row wrap;)
   - justify-content : (E.g: display: flex; justify-content: center, flex-start, flex-end, space-around;)
   - align-items : (E.g: display: flex; align-items: center, flex-start, stretch, baseline;)
   - align-content : (E.g: display: flex; align-content: space-between, space-around, stretch, center, flex-start, flex-end;)
   - Definations:
   - justify-content :	Horizontally aligns the flex items when the items do not use all available space on the main-axis.
   - align-items : Vertically aligns the flex items when the items do not use all available space on the cross-axis.
   - align-content : Modifies the behavior of the flex-wrap property. It is similar to align-items, but instead of aligning flex items, it aligns flex lines.
5. Grid Layout (Other Advance Properties later***)
   - gap : (E.g: display: grid; column/row-gap: 50px;)
   - grid-template : (E.g: display: grid; grid-template-columns/row: auto auto auto;)
   - justify-content : justify-content: space-between, start, center, space-evenly;(space-evenly:will give the columns equal amount of space between, and around them)
   - align-content : align-content: center, start, space-evenly; (space-evenly:will give the rows equal amount of space between, and around them)
6. Extra:
  - Overflow : ( overflow: visible, hidden, scroll, auto; ) ( overflow-x: hidden;  overflow-y: scroll; )
  - display : display: none, inline, block, inline-block;

# Tailwind CSS
1. Layout:
   - container
   - box-border-      box-sizing: content-box;
   - block-           display: block; (Take all the block(line))
   - visible-         visibility: visible; ( Show or hide without affecting the layout of the document.)
   - Z-index-
   - position-
2. Flexbox & Grid
   - Flex basis-         flex-basis: 0px;(Increase the width of flex item)
   - Flex Wrap-          flex-wrap: wrap;( wrap the flex item )
   - Flex Grow-          flex-grow: 1;( Use grow to allow a flex item to grow to fill any available space )
   - Flex Shrink-        shrink: 1;( Use shrink to allow a flex item to shrink if needed )
   - Order-              order-first( Utilities for controlling the order of flex and grid items.)
   - Justify Content-    justify-content: center;(container's main axis.)
   - Justify Items-      justify-items: start;(inline axis.) almost same Justify Self
   - Place Content-      mixture of justify content and align item.
3. Width & Height
   - width-              min-width: fit-content;(whatever will be the content, the width will fit according to content. other: min-content, max-content
4. Other Concept:
   - 
# React
Video link: [https://www.youtube.com/watch?v=6l8RWV8D-Yo]

1. `CDN(content delivery network)` : The primary purpose of a CDN is to deliver content, such as web pages, images, videos, and other media, to end-users quickly and efficiently.
2. `Jsx(JavaScript syntax extension)` : JSX provides an easy way to write HTML in React and easy to create templates. It is a kind of function that returns a object that React can interpret and used to create actual element. E.g:
      `const element = <h1 className="header">This is JSX</h1>
console.log(element)
/* output
{
    type: "h1", 
    key: null, 
    ref: null, 
    props: {
        className: "header", 
        children: "This is JSX"
    }, 
    _owner: null, 
    _store: {}
}
 */`
3. How to create react app: `npx create-react-app name-of-app` then `cd name-of-app` then `npm start`
4. How to create react app using vite: `npm create vite@latest` then `project name: react-app` then `framework:  react` then run `cd react-app` `npm install` `npm run dev`
5. Things to learn in react:
- Components
- props, passing props/function into component(props is used to pass value from parent to child component)
- states, passing state into component
- .map() method
- Event listener(`onSubmit={}` `onChange={}` `onClick={}`)
- Conditional rendering
- Ternary operator(E.g: `if hemant? "sah": "nayak"`)
- Fetch API
- Local Storage
- lazy initialization [https://kentcdodds.com/blog/use-state-lazy-initialization-and-function-updates#usestate-lazy-initialization]
-  **FORMS (Learn by doing) : What is a controlled form? A controlled form is a form whose input-field values are dictated by the application's state, and the application's state is dictated by the input-field values.
-  axioms
  
6. Extra:
- `npm install nanoid` `import {nanoid} from "nanoid"` `id: nanoid()` : unique nanoid will create and assign its value to id.
- array.unshift() : to put value of array on top.
- arrray.push() : push the element to array.
- event.stopPropagation() :  stops the bubbling of an event to parent elements, preventing any parent event handlers from being executed.
- body.split('\n')[0] : split the body after every whitespaces and return only 1 split.
- array.filter() : to filter array object from array(return desired object from array).
- array.find() : return the value of the first element that pass the test. Otherwise it returns undefined.
- array.findIndex() : return the index of the first element that passes the test. Otherwise -1.
- array.splice(index, howmany, item1, ....., itemX) : method adds and/or removes array elements and method overwrites the original array. [https://www.w3schools.com/jsref/jsref_splice.asp]
- <></> {known as fragment}
- way to write className = {` `dark ${color}` `}
- mockaroo( random data generator website) : [https://www.mockaroo.com/]
- JSON placeholder API : [ https://jsonplaceholder.typicode.com/ ]
- htmlFor(E.g: `<label htmlFor="hello">click me</label> <input type="text" id="hello"/>` )
- Higher Order functions (map, filter, reduce) : [https://www.youtube.com/watch?v=oGpA98nNx6Y]
- array.reduce() : It doesn't return array like map and filter method. It basically return the sum of array(One of E.g)

7. All hooks in React
   ### useState
       - simple and easy to use for managing simple state values that don't require complex updates.
       - const [counter, setCounter] = useState(0)
   ### useEffect
       - It is used when our component needs to do something after render.
       - It have 3 things. (1). Declare and effect (2). dependendies (3). clean up function
       - useEffect(()=>{
         },[])
   ### useReducers
       - It is used to reduce the state. It have 4 things. (1). state (2). dispatch (3) reducer function (4). action
       - const [state, dispatch] = useReducer(reducer, initialState)
       - function reducer(state, action){ return state}
       - onClick={()=>dispatch({type:"PLUS", payload:value})}
       - action => {type:"PLUS", payload:value}
   ### useContext
       - It is used to send the value or function from one component to another without the help of props. It helps to stop props 
         drilling.
       - `Context API` : React Context API allows you to easily access data at different levels of the component tree, without passing props to every level. It has 3 things:
       - (1). `context` : E.g: const person = createContext()
       - (2). 'provider' :  E.g: <person.Provider value={"Hemant"}/>
       - (3). `consumer` : E.g: <person.Consumer>{(name)=>{
           return <h1>My name is {name}</h1>
           }} </person.Consumer>
       - useContext is used to replace the consumer. E.g: const personName = useContext(person)
   ### useRef
       - 1. It creates a mutable variable which will not re-render the components.
       - 2. to access a DOM element directly.
       - E.g: const count= useRef(1) //it always return a object which have current variable(now current =1)
       - See other examples from internet
   ### useMemo
       - It is use to increase the performance of our applications.
       - useEffect hook doesn't return anything but useMemo always return memoized value. AND useCallback return memoized callback.
       - memoized value: Memoization is an optimization feature in React which, when used in the right place, increases the 
         performance of the program.
       - E.g : See from internet
   ### useCallback
       - both useMemo and useCallback increase the performance of our applications.
       - E.g : See from internet

# Redux
1. When we needed redux?
   - When app is moderately complex.
   - Lots of component levels.
   - Lots of changes in state
2. Redux have 5 parts
   - `State`: Global state object of App(E.g: Balance- Rs100)
   - `Action`: {type:'deposit', payload:10}
   - `Reducers`: function receives the current state + action object (state,action)=>newState
   - `Store`: store contains Reducers `getState()`
   - `Dispatch`: only way to update the state is to call `store.dispatch()`

# Nodejs and Expressjs
### Roadmap:
1. Modules, Packages, Npm
2. Server Concepts with Node
3. Web Server(Expressjs)
4. REST API (Expressjs)
5. File Structure MVC
6. MongoDB
7. Mongoose
8. React Integration
9. Deploy MERN App
10. Server-Side rendering
11. JWT, Authentication
12. Streams, Events, Sockets

    
Video link: [ https://www.youtube.com/watch?v=ChVE-JbtYbM ]
1. `Nodejs` : It is runtime environment for javascript. + it have APIs. Jaise Browser js ko run karta hai ussi tarah Node javascript ko run karta hai.
2. HTTP : (HyperText Transfer Protocol): It was designed to communicate between web services and web browsers. http request have no. of components
   - (i) Path(URL): when the client send the request to the server it needs to have a url. OR server is living at specific address and that address is URL.
   - (ii) Request Method(like POST, GET, PUT, DELETE, PATCH, OPTIONS)
   - (iii) BODY(Optional)
   - (iV) HEADER
   - `GET` : It gives us the information that we want from servers.
   - `POST` : sending/adding new data to the server(E.g USERID and PASSWORD).
   - `PUT` : Update the existing data(or replace all current representations).
   - `DELETE` : delete a particular data.
   - `PATCH` : apply partial modications to a data.
4. Things to learn in Nodejs and Expressjs
   - dependencies, devDependencies
   - introduction to Node, NPM, Package.JSON
   - Event loop [ https://www.youtube.com/watch?v=W-HQC_YUGBY ]
5. Importing modules method:
   - const lib = require('./lib.js') (Method1 for importing modules by the help of object)
   - import {sum,diff} from "./lib.js" (Method2 for importing modules by the help of ES module)
6. Reading data from files: const fs = require('fs'); //fetching fs from fileSystem module.
   - const txt = fs.readFileSync('demo.txt','utf-8'); console.log(txt); ('utf-8' is encoding to decode the message into readable format //reading file synchronous but this is not good use. It'll block other file till it is not excuted)
   - fs.readFile('demo.txt','utf-8',(err,txt)=>{ //best way to read files. This is asynchronous
    // console.log(txt); })
   - const t1 = performance.now(); //checking time to execute the code.
7. 3 line for creating server:
   - const express = require('express');
   - const server = express();
   - server.listen(2020); //server struct // we have to close server ownself so we use "ctrl + c" so that new code will run
8. Extra:
   - command: `npm init` //for setting package.json
   - command: `npm install express` //installing express
   - for deleting dependencies we use command: `npm uninstall express` `npm uninstall nodemon`
   - command:`npm install --global nodemon` => `nodemon index.js` => This command will install nodemon globally so that we don't have to restart the server again and again after every modification.

   - `nodemon` is a package for running node server and track live changes to re-start again.
   - Node versions are formatted like 4.1.9 where these are `major.minor.patch` versions.
   - package-lock.json has exact versions installed and link of dependencies of each package.
   - use npm update to update packages safely. npm outdated shows outdated and latets versions of packages installed in your package.json
   - node_modules should not be shared - you can make `.gitignoreto` ignore them to be uploaded.
   - .startsWith()
   - .replace()
   - dotenv : Dotenv is a zero-dependency module that loads environment variables from a .env file into process.env. In process.env we can add our own environment variable. dotenv files are hidden. `npm i dotenv` `require('dotenv').config()` `console.log(process.env)` : Link: [ https://www.npmjs.com/package/dotenv ]
   - cors : (Cross-Origin Resource Sharing)

### A/c RoadMAP
2. Server Concepts with Node:
- 1st we initialise the package.json by command: `npm init -y`
- We can use Server to do 3 things:
- (i) Static file Hosting : Sending normal files without formatting or modifying.
- (ii) Server Side Rendering : Mixing data with templates and rendering dynamic views (dynamic web pages) //This chapter 2 product is dynamic rendering(or Server Side Rendering)
- (iii) Web APIs : Sending data via some APIs/ endpoints.
- Imp. Links: Web Server Concept: [ https://www.youtube.com/watch?v=sfMNI0yLZII ]
- HTTP headers: [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers ]
- HTTP Method: [ https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers ]
- DummyJSON : [ https://dummyjson.com/ ]
3. Expressjs
  - Creating server
  - `const express = require('express');` `const server = express();` `server.listen(8080);`
  - server.get('/demo',(req,res)=>{ res.send('<h>hemant</h>'); })
  - server.get('/',(req,res)=>{ res.json({type:'GET'}) }) //server.get is Application method and res.json is response method
  - Expressjs have 5 method:
  -  1. Application methods : e.g. app.use()
     2. Request methods
     3. Response methods
     4. Middleware methods(means request aaya toh bich mai usko edit, modify etc kiya)
     5. Router methods
     6. for more details check: https://expressjs.com/en/4x/api.html
        
    ### Middleware methods: best link** [ https://expressjs.com/en/guide/using-middleware.html ]
  
     1. Middleware functions are functions that have access to the request object (req), the response object (res), and the next function in the application’s request-response cycle. (MiddleWare is the fn that process the request.)
     2. Middleware functions can perform the following tasks:
       - (i) Execute any code.
       - (ii) Make changes to the request and the response objects.
       - (iii) End the request-response life cycle.
       - (iv) Call the next middleware in the stack (next()).
     3. When request made by client is comes to server then it pass through one or multiple middleware and the request get modified each time. Next in middleware is use to call the next middleware.
     4. MiddleWare either send back the request with response OR send modified req to new middleware.
     5. position of middleware is very important.
     6. Types of middleware:
       - (i) Application level : app.use(middleware)
       - (ii) Router level : app.get('/', middleware, (req,res)=>{})
       - (iii) Built-in middleware : express.json() [ for parsing body data], express.static()[for static hosting]
       - (iv) Third-party middleware - like morgan
       - (v) Error-handling middleware
     7. Body-parser:
        - It allows you to extract data from the request body, which is typically sent in the form of JSON, URL-encoded, or multipart form data.
        - Using body-parser simplifies the process of handling request bodies in Node.js or Express.js applications by providing a convenient way to extract and parse the data from the requests.
      8. (iii) Built-in middleware : //Link for build-in middleware:[ https://www.youtube.com/watch?v=11GeorvleGI ]
          - (a) express.json() : server.use(express.json()); is a built-in middleware in Express.js that parses incoming requests with JSON payloads. It is similar to the body-parser middleware, but it is specifically designed to handle JSON data. (own language) : Whatever we are sending inside the body while requesting, express.json() convert the body data into json.
          - (b) express.urlencoded() : it is used to read the data of form.
          - (c) express.static('public') : The express.static() middleware is a built-in middleware in Express.js that serves static 
                files such as HTML, CSS, JavaScript, images, and more. It allows you to specify a directory on your server that 
                contains static assets, and Express.js will automatically handle the routing and serving of those files.
                //Own words: express.static('public') it go to the public directory and send the file-data available in the public 
                directory, if no files are available then it call the next middleware.
            - (d) express.text() : use to read the text value that is requested
         9. (iv) External Middle-wares:
             - (a) cookieParser(): server.use(cookieParser()); //it is used to read the cookies and through res.send() we can use 
                 that cookies.
            - (b) morgan : morgan('tiny') //morgan is a logger which is used to log(gives the information about request)
                  morgan('default')

# Next ->
  4. REST APIs and CRUD(Easy Done)
     - Router: `const router = express.Router()` for more details: [ https://expressjs.com/en/guide/routing.html ]
     - routes and controller
  5. MVC : It is used to manage the code so that it is not look dirty. It is used for bigger project.
    - Model: The backend that contains all the data logic.
    - View: The frontend or graphical user interface (GUI).
    - Controller: The brains of the application that controls how data is displayed.
   6. MongoDB and Mongoose
     - Mongoose: mongoose is object modeling for node.js Link : [ https://mongoosejs.com/ ].
     - We can connect Atlas with multiple things like : (a) MongoShell (b) MongoDB Compass(connect with local DB) (c) Driver(directly with nodejs) (d) Mongoose 
     - Learn other things by Doing.
   7. Connecting API with React
      - Easy see code or watch video again.
      - `npm run build` : it will build a folder of compile react-app that contains HTML, CSS, Js and other stuff which we will use for backend.
      - `npm i -g http-server` : to install http-server globally.
      - `cd build` `http-server` : to check whether compiled react-app is running or not.
      - `const path = require('path')` : use to specify the path.
   8. Authentication with JWT
      - A JSON web token(JWT) is JSON Object which is used to securely transfer information over the web(between two parties). It can be used for an authentication system 
         and can also be used for information exchange. The token is mainly composed of header, payload, signature. These three parts are separated by dots(.).
      - First we create token : `var token = jwt.sign({ email:req.body.email }, process.env.SECRET)`  `product.token = token` then add that token in product.
      - Second : Get that token `const token = req.get('Authorization').split(' ')[1]` then verify `var decoded = jwt.verify(token,process.env.SECRET)` if verified successfully then call next() middleware.
      - jsonwebtoken(jwt) : [ https://www.npmjs.com/package/jsonwebtoken ]
      - jwt.io : [ https://jwt.io/ ]
      - JWT authorization workflow : [ https://documentation.softwareag.com/webmethods/compendiums/v10-11/C_API_Management/index.html#page/api-mgmt-comp/co-jwt_usecase_workflow.html ]
      - There are many algorithm we follow for authorization. Above alogrithm is : HMAC SHA256
      - Other algorithm: `RS256` : Its key is bigger and have more security. link: [ https://cryptotools.net/rsagen ]. It has two key public and private key.
      - Private Key: by the help of private key we generate token.
      - Public Key: by the help of public key we verify token.
      - password hashing: we use bcrypt to safely store the password. you can use a library like bcrypt to hash password.
      - Installation : `npm install bcrypt`
      - Hashing: `bcrypt.hashSync(userProvidedPassword, saltRounds)`
      - Verifying Password: `bcrypt.compareSync(loginPassword, AlreadyHashedPassword)`, return true of false based on verification of password.
      - use `password.js` for logIn/signUp link: https://www.passportjs.org/

# http status
   1.  '200': 'OK'
   2.  '201': 'Created'
   3.  '202': 'Accepted'
   4.  '400': 'Bad Request'
   5.  '401': 'Unauthorized'
   6.  '404': 'Not Found'
   7.  '500': 'Internal Server Error'
   8.   


          


    

