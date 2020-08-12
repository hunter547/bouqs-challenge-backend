# The Bouqs Challenge Online Database

## Sources
Instructions and initial repo cloned from [json-server-heroku](https://github.com/jesperorb/json-server-heroku)
Addional instructions for me to make this work: [json-faker-server](https://github.com/atapas/json-faker-server)
The mock api files using Faker.js came from The Bouqs front end challenge [repository](https://github.com/thebouqs/fe-code-challenge/tree/master/api)

## Setup instructions
1. Clone this repo: `git clone git@github.com:hunter547/bouqs-challenge-backend.git`
2. cd into the project: `cd bouqs-challenge-backend`
3. Run the generate script: `npm run generate`
4. Add your files: `git add .`
5. Commit your files: `git commit -m "yay I have a database."`
6. Create an account on [Heroku](https://heroku.com/).
7. Install the [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) on your computer.
8. Then, log into Heroku from the CLI: `heroku login`
9. Within the bouqs-challenge-backend project folder, create a Heroku project: `heroku create my-cool-app`
10. Then push your commited changes form step 5 to Heroku: `git push heroku master`
11. Open your app once it's finished building: `heroku open`

## Function of `npm run generate`
This script runs the db.js file to generate data using faker.js and outputs the JSON result to a file called db.json. Then when Heroku runs npm start on server.js, server.js uses that file as its source to handle requests and serve data.