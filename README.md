
[Play Blog V Blog here!](https://competent-thompson-123cfb.netlify.com/)

  

Related repos: [Client](https://github.com/Koblinskis/BlogVBlog-client), [Server](https://github.com/Koblinskis/BlogVBlog-server), [MongoDB](https://github.com/Koblinskis/BlogVBlog-mongo)

# Blog V Blog Client

Blog V Blog is a web application that pits two blog titles against each other and the winner is determined by the user. The client is a React application that talks to an ExpressJS API backend, and the server reads and writes to a MongoDB Database. The server selects two random blogs titles from the database and returns them to the client, and then the user picks their favorite. The server records a winning score for the title selected. The highest scoring titles per category can be viewed on the winners page.

  

![Screenshot](https://raw.githubusercontent.com/Koblinskis/BlogVBlog-mongo/master/screenshot.png)

This repo is for the client-side code of the Blog V Blog project. The project is using the React framework to componentize the frontend and to easily handle the application's reactive data. React-router is used to handle routing.

The browser's default CSS is reset using [normalize.css](https://necolas.github.io/normalize.css/). SCSS is used to make styling development easier. The SCSS in this project is following the [BEM](http://getbem.com/) methodology that helps to create reusable components and code sharing in frontend development.

On the winners page [ChartJS](https://www.chartjs.org/) is used to display a bar chart that shows the user which blog is winning in each category and by how many votes.

The brower's built-in Fetch API is used to make GET and POST requests to the [Express API backend](https://github.com/Koblinskis/BlogVBlog-server). 

This is deployed on Netlify.

## How to run the client
Create `.env.development` file in the root of the project. That file needs to contain a reference to a running version of the server. Find out how to run the server by clicking [here](https://github.com/Koblinskis/BlogVBlog-server). 
```
REACT_APP_NODE_SERVER_URL="http://localhost:3001"
```
**Step to run:**

 1. `npm install`
 2. `npm run start`
