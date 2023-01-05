# Advanced Node and Express

This is the boilerplate for the Advanced Node and Express lessons. Instructions for the lessons start at https://www.freecodecamp.org/learn/quality-assurance/advanced-node-and-express/

# Running Mongo Locally

1. Install MongoDB ([MacOS](https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/))
2. Run `mongod --config /opt/homebrew/etc/mongod.conf` to run while terminal is open
    - `brew services start mongodb-community@6.0` to start mongo as a service
    - `brew services stop mongodb-community@6.0` to stop the mongo service
3. Set `MONGO_URI='mongodb://localhost:27017/?retryWrites=true&w=majority'` in `.env`
4. Create a database named `database`
5. (optional) Use [Studio 3T Free](https://studio3t.com/free/) as a GUI

# Using Ngrok Locally

1. Sign up for [ngrok](https://ngrok.com/)
2. Set up your [auth token](https://dashboard.ngrok.com/get-started/setup)
3. Spin up the server with `npm run dev`
4. Expose the server to `ngrok` with `ngrok http 3000`
5. Use the `ngrok` url for the [Quality Assurance](https://www.freecodecamp.org/learn/quality-assurance/) lessons
