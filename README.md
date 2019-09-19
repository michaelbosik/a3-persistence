Assignment 3 - Persistence: Two-tier Web Application with Flat File Database, Express server, and CSS template
===

## The Q

http://a3-michaelbosik.glitch.me

Log in credentials were provided via direct message on the class slack to the staff. My slack name is Michael Bosik if there are any questions.

Include a very brief summary of your project here. Images are encouraged, along with concise, high-level text. Be sure to include:

This application is intended to be a way for multiple spotify users to queue up songs and listen to them at the same time.

One of the biggest challenges I faced while creating this application was being able to successfully grab songs from a search using the spotify api.

In the queue.js file you'll see a lot of commented code. This is currently not working but is intended to be the music player that uses the spotify SDK to play songs.

I used passport as an express middleware when creating this application. Passport supports the spotify strategy in order to authenticate users.

I used bootstrap as my CSS framework because the ability to style elements by class was important for my application. Some elements are created by editing the innerHTML of certain elements.

I altered the CSS by putting !important tags on some of the elements to override the styling in bootstrap

The six middleware I used were:
 - passport - authenticates users using the Spotify middleware
 - express-session - used to keep track of sessions
 - bodyParser - used to read request bodies easily
 - querystring - used to concatenate a query string
 - cookie-parser - used to read the cookie in a session
 - lowDB - used as the database for the server

## Technical Achievements
- **Tech Achievement 1**: Created a front-end user interface
for a group spotify queue. Users can search for songs using the
search form submission
- **Tech Achievement 2**: I used OAuth authentication via the Spotify strategy
- **Tech Achievement 3**: I used over five Express middleware packages, enabling me to create a server that parses a request body, can develop a querystring and authorize users using passport. Sessions can also be created and identified with 
cookie-parser.
- **Tech Achievement 4**: Server stores users and queued songs
on a lowDB database. When a user authorizes their account with
spotify, it is saved to the database in a 'users' array. No user
is ever logged twice. When a song is added to the queue, it is
stored in a 'queue' array.
- **Tech Achievement 5**: Songs in the queue can be deleted by
users. The data is removed from the database and the front-end
is updated.
- **Tech Achievement 6**: Server will create a table that is already styled with the rest of the page

### Design/Evaluation Achievements
- **Design Achievement 1**: I tested my application using multiple
sized screens and the pages rearrange orientation accordingly
- **Design Achievement 2**: I utilised the bootstrap CSS framework
to give my website a sound structure and sleek appearance
- **Design Achievement 3**: I used font-awesome and google fonts to give my page a more professional look in terms of text
- **Design Achievement 4**: Each element in my page is labeled by class or by ID for easy access
