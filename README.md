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

7. All hooks in React
   ##useState
   ##useEffect
   ##useReducers
   ##useContext
   ##useRef
   ##useMemo
   ##useCallback

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
   
