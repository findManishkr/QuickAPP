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

       
    


