# ai powered blog app


* we will create the `fronted` in react ;
-> to create a react project we'll use `react + vite package`

```
 npm create vite@latest  

 // this command creates a new fronted project with `vite` as the project tool.
 // it is used to quickly set up project with minimal configuration


```

* navigate to the `client` directory and run the command `npm install ` it will install all required
dependencies listed in the package .json file



` npm run dev `:-> this command used in Node.js project to 'start the development' server.

`package.json` contains this script

```
"scripts":{
    "dev":"vite"
}

```
so when you type `npm run dev ` you're telling npm "run the script named 'dev' which is basically 
the command `vite` ".



### add color theme to whole web app

```
`index.css` -> 

@theme{
    --color-primary :#5044E5;
}


````







* to hide scroll bar , use the below command

```
::-webkit-scrollbar {
    display: none
}

```








### time to add tailwind css in the 

* to install tailwind , use command

`npm install tailwindcss @tailwindcss/vite`:-> this intalls various requirements of tailwind in react app




### install one more package 

* `in our web app we will create different pages,`
*  `and we will navigate the user from one page to other page`

for that we need to add `react-router-dom pacage`

```
 npm install react-router-dom                     // [in client folder]


```

- after this we have to set up `route`

->### open main.jsx file

* import `BrowserRouter` from `react-router-dom` package
```
import {BrowserRouter} from `react-router-dom`

```

### now its time for figma design of our blog app

- here we will design different pages of the website

-- before that will create folder structre for compontent and pages

```
 client/
|-src/
     |-> creat `component ` folder



     |-> create `pages ` folder
                   * open pages folder
                |-> create `Home.jsx` file
                    * add   <h1>Home </h1>

                |-> creat `Blog.jsx` file
                    * add < h1> Blog</h1>    
     


```






### underdstanding the meaning of basic react program

```

 import react from 'react'

 const Home = () => {
       
       return (
          <div> 
          
          </div>


       )


 } 


 // above program defines->
   *  a basic react component named Home that currently renders an empty <div> to the page


```



### how to create routes

* -> `ex`:-> `http://localhost:5173/blog`, `http://localhost:5173/home`


```

import React from 'react'
import {Route, Routes } from 'react-router-dom'
import Blog from './pages/Blog'
import Home from './pages/Home'

const App = () =>{
    return (
      <div>
       <Routes>
        <Route  path = '/'  element = { <Home/>} />
        <Route  path = '/blog' element = {<Blog/>}/>
       </Routes>
      </div>
    )
}

export default App;

`this simply sets different routes`




```