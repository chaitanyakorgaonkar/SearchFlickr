SearchFlickr

A web-based UI for finding and viewing images on Flickr.

Before running the webpage 

I have used Express framework for developing the website. Please install Express on Node.js using the following commands: 

npm install -g express 
npm install -g express-generator 

To install flickrapi run the following command: 

npm install -g flickrapi 

and then just to ensure all the required dependencies are installed run the following command: 

npm install 

Running the application

Go to the project folder
Run the following command:

node ./bin/www

Then on the web browser go to the following url:

http://localhost:3000/

User Interface Design Decisions 

Home page 
The home screen allows the user to enter any combinations of the four specified fields. When the user clicks on the Search button he is taken to the 'Flickr Image Search Results' page. 

The following validations are handled on the home screen: 

1. When the user enters none of the four fields and hits Search button, a text saying 'Enter atleast one field' is shown to him. 

2. When the user enters an invalid username and hits Search button, a text saying 'Invalid Username' is shown to him. 

3. When no results are found for the values entered by the user for any of the fields, a text saying 'No results found' is shown to him. 

We can navigate to the home page from any page using the Home button on the top right of the page. 

Flickr Image Search Results page 

The search results are displayed on this page 10 at a time. For more results click on the 'more pics' button at the bottom of the page. 

To open the image url, click on the image. 
To open the user profile of photos owner, click on the link below the photo. 

Click on the home button in the top right corner to go back to home page. 
Validations on this page: 

When the user clicks on 'more pics' and there are no more pics in the result, the more pics button changes to 'No more pics' and is disabled. 

References: 

1. Installations 
http://cwbuecheler.com/web/tutorials/2013/node-express-mongo/
 
2. Convert javascript date to mysql date format 
http://stackoverflow.com/questions/5129624/convert-js-date-time-to-mysql-datetime 

3. Datepicker 
http://jqueryui.com/datepicker/

