# BBPlate
My personal boiler plate - Using webpack for React, Redux, Express and Knex

**Creating/Installing basic functionality**
Clone your forked repo down
Run the following commands in your terminal
* npm install
* knex migrate:latest
* knex seed:run
* npm run dev - this will start bundling, watch and nodemon
* npm start - this only runs server, viewable at localhost3000 (setup for heroku).

**Heroku**
* Create app  - with the command heroku create [name]
* Check that the app was added by running heroku apps to view a list of your apps.

**Adding postgres**
* Add postgresql - using the hobby dev option on Heroku
* Check that pg has been added by running heroku addons to ensure the postgresql db is on your app.

**Deploying**
*I have created several npm scripts that will be useful for deploying your app to heroku easily.*

* npm run bb:deploy will push your local master branch to your heroku app
* npm run bb:migrate will run your knex migrations on your deployed heroku app
* npm run bb:seed will run your seeds on your deployed app
* npm run bb:rollback will rollback the seeds.
