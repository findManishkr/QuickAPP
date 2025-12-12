# backend of the project 

```
 QuickApp/
      * create a folder server
    |-> server/
          * create a file `server.js` [-main file of our backend server]
          |-> server.js
         
```

* now, initialize a node.js project  inside `server folder` project using command `npm init -y`,after this
  a `package.json` file will be created


## now its time to install some dependencies that will be used in our backend


 `npm install <packages>`: adds the specified libraries to :
   * `node_modules` / directlory
   * `dependencies` section in `package.json` ( unless you use --save-dev )


   `npm install express mongoose cors dotenv jsonwebtocken multer`:

    - what each package is used for 

     ### 'express'
      - express is used to build server and api endpoints
      - it is fast and minimal web framework for Node.js

      ### 'mongoose'
      - An ODM( object data modelling ) library for `mongodb`
      - it provides `schemas`, `modals`, `validation`, `middleware` and simplified database operations
      - Mongoose connects you `Node.js` App to `mongodb` and lets you create `schemas` and `modals`

       
     ### cors
      - Used to allow fronted(React,Angular etc) to access you backend api ie enables cross-origin resource sharing
      - Useful when you frontend and backend run on different domain/ports. It controls which domain 
        can access your api.


     ### dotenv
      - loads `environment variables` from a `.env` file to `process.env`
      - used for configuration :`database urls`, `secrets`, `keys` etc

     ### jsonwebtocken(JWT)
      - used to create and verify json Webtockens for authonetcation and authorization.
      - ie used for login authontication : generate and verigy JWT tockens.


     ### multer
      - it is a middleware , primarily used for file uploads( image, documents , videos,etc )   
     



`npm install nodemon --save-dev`:-> nodemon is a developers tool,
  that automatically restarts your Node.js Server whenever you save changes in your code


  `--save-dev`-> stores the nodemon in `devDependencies section` in `package.json` file
      not in normal dependencies, as nodemon is needed during development,
      not in production
