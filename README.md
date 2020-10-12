## README

Dear colleague

In order for this to run you need to have a .env file in the following format

```
DATABASE_URL_DEVELOPMENT=<your url here>
```

- Install dependencies
  - sequelize, sequelize-cli, pg, dotenv
- Create a .env file
  - Add the url to the file
- Put the .env in gitignore
- require('dotenv').config()
  - config/config.json
    - turn config/config.json into config.js
    - add module.exports
    - in models/index.js turn config.json into config.js
    - require('dotenv').config() at the top
    - change url in config to `process.env.<WHATEVER_YOU_CALLED_YOUR_VARIABLE>`
  - index.js (where you start a server)
    - require('dotenv').config() at the top

For CRA:

- https://create-react-app.dev/docs/adding-custom-environment-variables/
