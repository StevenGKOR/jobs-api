The Jobs API is a server-side application that provides CRUD functionality and was developed using JavaScript, Node.js, Express.js, and MongoDB. The API features various packages, including SwaggerUI and JWT for added security.

To access the Jobs API, users must visit the following URL: http://jobs-api-lmgs.onrender.com/. Additionally, there is a specific URL for documentation, which can be found here: http://jobs-api-lmgs.onrender.com/api-docs/.

For security purposes, packages such as helmet, cors, rate-limiter, xss, and bcryptjs were implemented. Users must register and log in with a valid email and password (which must be longer than three characters) to access the /jobs routes. Once a user is authenticated, a token is generated and stored to allow access to the API.

To handle database management and connections, Mongoose is used. Additionally, HTTP status codes are implemented to provide specific responses depending on user requests and outcomes. In the event of an error, an error-handler middleware is implemented.

The Jobs API allows users to store job interviews and their respective statuses. After registering or logging in, a user can create, view, update, or delete interviews. Interviews can be updated to one of three available statuses: interview, declined, or pending. Pending is the default status for any newly created interviews. It's important to note that users can only view, update, and delete interviews that belong to them.


