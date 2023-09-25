# Full-Stack-Web-Development
This repo contains the roadmap and the full-stack web development notes along with video link from different YouTube Channel.

## Roadmap
- HTML
- CSS
- JavaScript
- React
- Nodejs and ExpressJs
- MongoDB
- Linux
- DevOps
- Tailwind
- TypeScript
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
   
