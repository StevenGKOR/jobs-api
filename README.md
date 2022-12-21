Jobs API is a server-side application, provide a CRUD functionallity, developed with Javascript, Node.js, Express.js and MongoDB.
Extra packages like SwaggerUI and JTW were used.

URL : http://jobs-api-lmgs.onrender.com/
Specific URL for documantation : http://jobs-api-lmgs.onrender.com/api-docs/

For security,packages like helmet cors rate-limiter and xss
JWT used for registration/login, when a user logged in or register to the app a token with genarate. Users cannot access the /jobs 
routes if they have not created an account or are not logged in
Bcryptjs used for hashing passwords
SwaggerUI for a beautifull UI documentation
Http-status-codes for specific status codes at responses depending on the requests of a user and the outcome of the response
Mongoose for database connection and data management
A middleware named error-handler handles the errors 


The API can be used to store an job interviews and the status of those interviews. First a user must create an acoount or login with a existing one
A user must provide a valid e-mail (checking throw regex) and a password bigger than 3 length, the email must be unique

If users logged in or create an account they can create a job interview, update the status of that interview 
between 3 available status (interview, declined and pending). Pending will used as default status. Users can only view, update and delete the 
interviews that belong to them



