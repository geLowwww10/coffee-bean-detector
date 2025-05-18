# Coffee Bean Detector Web Application

A web application for detecting and analyzing coffee beans using computer vision and machine learning.

## Deployment to Render

1. Create a new account on [Render](https://render.com)

2. Create a new Web Service:
   - Connect your GitHub repository
   - Choose the branch to deploy
   - Select "Node" as the runtime
   - Set the build command: `npm install`
   - Set the start command: `node server.js`

3. Set up Environment Variables in Render:
   ```
   NODE_ENV=production
   PORT=8080
   DB_USER=coffebean
   DB_PASSWORD=coffeebean
   DB_HOST=localhost
   DB_PORT=5432
   DB_DATABASE=coffeebean_scanner_db
   ```

4. Create a PostgreSQL database in Render:
   - Go to "New +" and select "PostgreSQL"
   - Name it "coffee_bean_db"
   - The database credentials will be provided by Render

5. Update the environment variables with the database credentials provided by Render

## Local Development

1. Install dependencies:
   ```bash
   npm install
   ```

2. Create a `.env` file with:
   ```
   NODE_ENV=development
   PORT=5000
   DB_USER=postgres
   DB_PASSWORD=postgres
   DB_HOST=localhost
   DB_PORT=5432
   DB_DATABASE=coffee_bean_db
   ```

3. Start the server:
   ```bash
   npm start
   ```

## Features

- User authentication
- Coffee bean detection and analysis
- Quality metrics calculation
- Scan history tracking
- User profile management 