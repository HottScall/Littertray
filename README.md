1 - Create client folder

2 - Setup index.html
    2.1 - Create Header

3 - Bring in Skeleton CSS (http://getskeleton.com/)
    3.1 - Create styles.css file
    3.2 Add Skeleton css via link

    <link rel="stylesheet"href="https://cdnjs.cloudflare.com/ajax/libs/skeleton/2.0.4/
    skeleton.min.css">

    3.2 - Add links such as <link rel="stylesheet" href="styles.css">

4 -  Create form
     4.1 - Name
     4.2 - Content
     4.3 - u-full-width to both inputs
     4.4 - Listen for form submit (Javascript, line 5 - 19)
     4.5 - Hide the form
     4.6 - Show loading spinner
     4.7 -  Get data from form and log it

✅ Get user input on the Client
✅ Hide/Show elements on the client

Back-end

 5 - Create server folder
     5.1 - Create server directory
        Terminal - npm init -y (Initializes node.js)

 npm init -y
 npm install express morgan
 Setup index.js
 Add GET / route
 Add POST /mews route
 log out req.body
Front-end
 fetch POST /mews with form data
 See the CORS error and revel in this moment
✅ Send user input from the client with fetch to the server
Back-end
 npm install cors
 Make sure the server is recieving the data
 Add JSON body parser middleware
 Validate name and content
 Must be a string
 Cannot be empty
 If not valid
 Error code 422
 Invalid mew, must contain name and content
 Setup DB Connection
 npm install monk
 connect to db
 create document collection (mews)
 If Valid
 Create mew object with
 name, content, created_date
 Insert into DB
 Respond with created mew object
✅ Store data in a database
Front-end
 Log out created Mew after POST request
 Show the form
 Hide loading spinner
Back-end
 GET /mews
 Respond with mews from DB
✅ Retrieve data from a database on the Server
Front-end
 fetch GET /mews
 Iterate over array
 Append each to page
 Reverse before appending
 Show the form
 Hide loading spinner
 fetch GET /mews after creating a mew
✅ Retrieve data from a server on the client using Fetch
✅ Hide/Show elements on the client
✅ Add elements to the page on the client
Back-end
 npm install bad-words
 Use filter before inserting into DB
 npm install express-rate-limit
 Limit to 1 request every 15 seconds
Deploy
✅ Deploy server with now
 Setup environment variables
 Database connection
process.env.MONGO_URI
✅ Show mlab
 Deploy with environment variable
now -e MONGO_URI=@meower-db
 Add alias
✅ Deploy client folder with now
 Set API_URL based on hostname
# Littertray
# Littertray
