The general Way of showing Hello on a page is 
```
    var rootHandle = document.getElementById('root')
    var belgiumHandle = document.createElement('belgium-area')
    belgiumHandle.appendChild(document.createTextNode('Hello'))
    rootHandle.append(belgiumHandle)
```


This could be boiled down to 2 lines of code By the Syntactical sugar provided by react
```
   var belgiumElement = React.createElement('div', {class: "belgium-area"}, 'Hello')
   ReactDOM.render(belgiumElement, document.getElementById('root'))
```

Display an Anchor Tag In the Browser

```
  var anchorElement = React.createElement('a', {href: "https://www.google.com", id: "anchor_google"},"Visit Google")
```

Displaying of the Ul having a lot of the lis
```
  var ulElement = React.createElment('ul', {class: "product_listings"},
    React.createElement('li', {id: 'product_1'}, 'NodeJs'),
    React.createElement('li', {id: 'product_2'}, 'Javascript'),
    React.createElement('li', {id: 'product_3'}, 'React')
  )
```


```
JSX --> Stands for JAvascript XML
 - JSX is the syntax of the html elements being assigned to the variables for the sake of the usage on to the Browser .
 - For doing this we basically need the support of the Babeljs package
 - Babeljs is used for converting the [JSX] ---> [React] and once it is converted to the React level then reactDom does the operation of rendering the react elements into the web page .
 - We load the Library of the Babel 
  using <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
  - Generally babel is used to convert the ES6 syntax to the ES5 for the browser to understand and it also does the Job of converting JSX to the React Html
  - When we write the JSX syntax script type="text/babel"
```


```
  What is embeedding string in JSX?
  const place = 'Bengaluru'
  const h1 = <h1> We are currently in {place}</h1>
```

```
 We learn how to embed function in the JSX
 We learn how to embed an Object information into the Html page
```