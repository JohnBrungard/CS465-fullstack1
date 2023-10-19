# CS465-Full-Stack-Development

<b>Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page application (SPA).</b>

<p>Express is the web framework for node.js that is designed to perform tasks in a well-tested and repeatable way. It sets up a web server for incoming requests and returns relevant responses.
Express also defines a directory structure. Furthermore, Express uses sessions so that you can identify visitors thorugh multiple pages and requests.</p>

<p>JavaScript is the language that makes up the MEAN stack. This allows coding of the frontend and backend with the same language. Furthermore, the use of Angular in our stack is made up of a JavaScript framework for creating interfaces in our application.</p>

<p>A Single Page Application(SPA) dynamically rewrites the current page rather than loading new pages from a server. This means no page reloads and less time wasted refreshing pages. An example of an SPA is Facebook. SPA’s also consume less bandwidth since they only load once.</p>

<b>How is JSON different from Javascript and how does JSON tie together the frontend and backend development pieces?</b>

<p>We use BSON (Binary JSON/JavaScript Serilaized Object Notation) which is how MongoDB stores documents for us to apply CRUD operations with. These documents hold name/value pairs to describe and define data. Through Mongoose, the BSON is exposed as JSON. We also use JSON for our API for transporting data. With this the API will either return JSON Objects or a null reponse for each request between the frontend and backend. </p>

<b>Provide instances in the full stack process when you refactored code to improve functionality and efficiencies, and name the benefits that come from reusable user interface (UI) components.</b>

<p>One instance of refactoring was replacing the static HTML pages with templates using Handlebars, particularly the travel.html file to render each trip without a page reload. This enabled /travel to drive the rendered page dynamically by data passed into the template and reduced the 120 lines of static HTML down to 35 lines.  </p>

<p>We also refactored the Express backend and Angular SPA frontend to include authentication, particularly for CRUD operations involving trips. This made it to where authentication middleware injections are keys to protect the API routes from unauthenticated callers </p>

<b>Methods for request and retrieval necessitate various types of API testing of endpoints, in addition to the difficulties of testing with added layers of security. Explain your understanding of methods, endpoints, and security in a full stack application.</b>

<p>We use API Testing to ensure the SPA is working with the API in which we make requests to the API endpoints and compare their responses with the actual results. For our project, we performed this by checking the backend API by checking MongoDB for data that was added and the data that was retrieved. We also analyzed the powershell for certain codes to determine success such as 200 and 201 for correct actions and 400 and 500 for unintended results.</p> 

<p>On the front end, we checked this by analyzing the view after being updated by the model as we navigated through the application. For example, adding the trip ‘Mega Reef’ through the front end would display a card view with the specified contents. We could also see the path in the url. This is because, in essence, the web browser will take requests from the SPA, secure them with CORS, and forward the request to the secured API.</p>
