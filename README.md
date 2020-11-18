## Starting a Vue project from scratch

1.  Create new folder and change to it

    - `mkdir vue-from-scratch`
    - `cd vue-from-scratch`

2.  Init project and install express

    - `npm init -y`
    - `npm i express`

3.  Create all the files

    - `mkdir public`
    - `touch public/index.html`
    - `touch public/script.js`
    - `touch public/style.css`

4.  Link all the files

    - HTML skeleton in index.html:

      ```html
      <!DOCTYPE html>
      <html lang="en">
        <head>
          <meta charset="UTF-8" />
          <meta
            name="viewport"
            content="width=device-width, initial-scale=1.0"
          />
          <title>Vue from Scratch</title>
        </head>
        <body></body>
      </html>
      ```

    - Get vue CDN link from https://vuejs.org/v2/guide/installation.html

    - Link vue.js in index.html (`<script src="https://cdn.jsdelivr.net/npm/vue@2.6.12/dist/vue.js"></script>`)
    - Link our own js (`<script src="/script.js"></script>`)
    - Link our own css (`<link rel="stylesheet" href="style.css" />`)

5.  Setup static server

    - `touch index.js`
    - setup express server with static middleware to server everything from public folder

6.  Initializing Vue

    - Add main container for vue application in index.html (`<div id="main"></div>`)
    - Initiate vue application in script.js

      ```js
      new Vue({
        el: "#main",
        data: {
          name: "VUE",
        },
      });
      ```

7.  Start Server with `node index.js`

8.  http://localhost:3001
