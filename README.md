# marybees

An e-commerce website where shoppers can browse and purchase clothing, setup user profiles. 
Shopowners can maintain a backend database of clothing by logging in as a superuser.
The idea for the clothing store came from a colleague of mine who wants to open an online second hand clothes store and join the circular economy.
The target audience is all those interested in buying clothing - from adults to children. 

## User Stories

AS A USER | I WANT TO | SO THAT I CAN
:---------|:-----------|--------:
Shopper | View a list of clothing | Select some to buy
Shopper | Filter to a specific category of clothing | Find what interests means quickly without having to go through every product
Shopper | Filter to a specific brand of clothing | See all products available in that brand category
Shopper | View individual product details | See the price, rating, description, image, sizes
Shopper | Quickly find deals, special offers, clearance items | Find a good bargain
Shopper | Easily see my spending total | Spend even more
Shopper | Search for an item by name or description | Find a specific product 
Shopper | Easily see what I've searched for and the number of results | Quickly decide if the product I want is available
Shopper | Sort a list of available items | Quickly filter to best price, category, rating
Shopper | Sort a specific category of clothing | Find best-priced/rated clothes in a specific category or sort the products in that category by name
Shopper | Sort multiple categories of clothing simultaneously | Find best-priced/rated clothes across broad categories such as homeware or clothing 
Shopper | Easily select size and quantity of an item | Be sure I have the correct size/quantity
Shopper | View items in my bag to be purchased | Identify total cost of items and all items I will receive
Shopper | Adjust the quantity of individual items in my bag | Make changes to my purchases before checkout
Shopper | View an order confirmation after checkout | Verify my order
Site User | Register as an account holder | Have a personal account and be able to view my profile
Site User | Login/Logout | Access personal account info
Site User | Recover my password if forgotten | retrieve account Access
Site User | Receive email confirmation after registering | Verify account registration
Site User | Have a personalised user profile | Store billing info and view order history 
Store Owner | Add a product | Add new products to my store
Store Owner | Edit/Update a product | Change product price, description, images, category, rating
Store Owner | Delete a product | Remove items no longer for sale

## Features

### Existing Features

The website layout is kept as simplistic as possible for ease of use and to be easy on the eye. 
On opening the home page viewers see a header containing the shop name (marybees), a search bar in which to enter search terms contained in a form element
and an unordered list containing an account profile sign in/registration list element along with a shopping bag icon. Shop-name, search bar, my account and shopping bag are all inline.
The navbar is directly below the header and contains dropdown menus for Brands, Clothing and Special Offers. These menuitems allow a certain amount of filtering for specific products or not as the case may be.
Directly below the navbar is a banner containing a free delivery offer on items purchased for more than €50.
These elements are consistent across all pages of the website.
Also to be found on the homepage is a shop now button. Clicking this leads to the products page where all products are displayed.

Colors used on the site are all bootstrap colors. 
The overall theme is white backgound and bootstrap-dark text and button colors. The delivery banner has a background of bootstrap-warning on all pages and also in toasts where free delivery threshold has not yet been reached.
The homepage has a background image but this is hidden on all other pages via the bootstrap overlay class. Bootstrap styling has been used extensively throughout the site.

Product images are displayed in Bootstrap cards. The images can be clicked and on the second clicking instance these open onto a new page.
Stacked on top of one another underneath the images are: the name of the item, its price in bold print its category and its rating.
Categories can be clicked to go to a page of products displaying that specific category ot items. 
As one scrolls down the page a back to top arrow appears in the bottom left corner of the page.

Shoppers can view all clothing products and filter and sort them in a number of ways. 
Products can be filtered by name, price, rating and category. 
The ability to select different categories allows shoppers to filter products for activewear, jeans, essentials, shirts, any clothing deals available and clearance items.
It is also possible to filter for specific brand names items such as Vans, Champion etc. Filtering for ascending/descending price and rating is also possible along with names and categories in alphabetical or inverse alphatbetical order.

Obviously shoppers don't just want to browse items but also add them to a shopping bag and purchase them. 
To select an item simply click on its image which displays this item on its own. On display are an image of the object along with the items name, price, category and rating
as well as a description of the item. A size selector is also visible along with a quantity selector and 2 buttons to either continue browsing products or add this product to the shopping bag.
The "Keep Shopping" button returns the user to the all products page. When "Add to bag" is clicked a toast pops up in the top right corner of the screen with a header saying "Success". Below that a message saying what was added how many items are in the shopping bag, 
widgets containing images of the shopping bag items, the total price ot the purchase and a button leading to the checkout page.
The shopping bag items changes to Bootstrap-success color and the total is displayed so that when the toast is closed the amount is still visible.

Clicking the "Go to secure checkout" button one arrives on the shopping bag page which displays, images of the items, their description, size, quantity, sku number, price quantity, subtotal and the ability to update or remove the item. 
If an item is updated or removed a toast appears again in the top right corner confirming what was done and updating the shopping bag accordingly.
Again on this page the user has the option of returning to the all products page to browse some more if they wish by clicking the "Keep Shopping" button.
Selecting "Go to checkout" on this page leads to the checkout page which contains a form. Info to be filled-in include name, email, delivery address and payment information.
The checkout page also displays a short order summery containing the image, name, size quantity, price of the item and total amount.
There are 2 buttons at the bottom of the page, one to edit the shopping bag if the shopper wants to change anything in their order.
The other button allows the shopper to complete their purchase. Which again shows a toast with a success message all going well or an error message if something goes awry.
The toast success message confirms the order was placed, shows the order number and states an email confirmation will be sent to the email provided.
This page also shows the order information. Order number, order date & time, name of item, quantity and price as well as delivery address provided.
There is a checkbox option that allows the user to save their shipping info also.

Some shoppers like to create profiles with companies to speed up the checkout experience as well as keep track of their order history and billing info.
It is possible for shoppers to create a profile and save their personal and order histories for future reference. Reset passwords as needed.

Store owners can have administrative access to the database to add, edit and delete entries as necessary 


### Features Left to Implement

Add webhook handlers to checkout logic.

Add shipping address info to checkout flow if shipping address differs from billing address.

Send confirmation emails.

The ability to add sizes to items in the backend django database.

Improve sizing across product range.

Set up a review page.

## Technologies Used

[IDE](https://www.gitpod.io/) 
Gitpod is an online IDE which can be launched from any GitHub page. 
Gitpod provides a fully working development environment, including a VS Code-powered IDE and a cloud-based Linux container configured specifically for the project at hand.

[HTML5](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5) is a markup language used for structuring and presenting content on the World Wide Web. 

[CSS3](https://developer.mozilla.org/en-US/docs/Archive/CSS3) 
Cascading Style Sheets is a style sheet language used for describing the presentation of a document written in a markup language such as HTML. 
CSS is a cornerstone technology of the World Wide Web.

[Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript) is a scripting or programming language that allows you to implement complex features on web pages — 
every time a web page does more than just sit there and display static information for you to look at — displaying timely content updates, interactive maps, animated 2D/3D graphics, scrolling video jukeboxes, etc. — 
you can bet that JavaScript is probably involved. 
It is the third layer of the layer cake of standard web technologies, the other 2 being HTML and CSS.

[Bootstrap4](https://getbootstrap.com/) is a free front-end framework for faster and easier web development.
Bootstrap includes HTML and CSS based design templates for typography, forms, buttons, tables, navigation, modals, image carousels and many other, as well as optional JavaScript plugins.
Bootstrap also gives you the ability to easily create responsive designs.

[Django](https://www.djangoproject.com/) is a Python-based free and open-source web framework that follows the model-template-views architectural pattern. 
It encourages rapid development and clean, pragmatic design.

[Python](https://www.python.org/) is an interpreted, object-oriented, high-level programming language with dynamic semantics. 
Its simple, easy to learn syntax emphasizes readability and therefore reduces the cost of program maintenance. 
Python supports modules and packages, which encourages program modularity and code reuse.

[Postgres](https://www.postgresql.org/) is a powerful, open source object-relational database system that uses and extends the SQL language combined with many features that safely store and scale the most complicated data workloads.

[Stripe](https://stripe.com/)
Online payment processing for internet businesses. 
Stripe is a suite of payment APIs that powers commerce for online businesses of all sizes.

[AWS](https://aws.amazon.com/)
Amazon Web Services is a subsidiary of Amazon providing on-demand cloud computing platforms and APIs to individuals, companies, and governments, on a metered pay-as-you-go basis.

[Heroku](https://www.heroku.com/) is a platform as a service (PaaS) that enables developers to build, run, and operate applications entirely in the cloud.

### Testing

[HTML Validator](https://validator.w3.org/)

[CSS Validator](https://jigsaw.w3.org/css-validator/)

[Javascript Validator](http://beautifytools.com/javascript-validator.php)

Extensive testing on chromebook during development. Heroku app tested on iPhone11, One Plus 7T Pro mobile phones and Ipad 2 tablet.
Responsiveness was slower on the apple products in terms of website loading and page loading. 
Functionality as expected and described above. 

Bugs:

* Checkout form styling - form fieldsets not adhering to bootstrap styling i.e should have a dark border and no border-radius on both phones. Same for some of the buttons.

* Resolved: Brand name querying - ampersand (&) is a special character in querying so company brandnames containing  (&) - the & must be replaced or the query doesn't return any result. Here it is replaced with the word 'and.

### Deployment

Project level settings file connects the Django database, AWS S3 file store with the Heroku app. Environment variables are stored both in the IDE and Heroku app Config vars.

[Heroku](https://www.heroku.com/)-to deploy to Heroku firstly create a new app then in the resources tab provision a heroku postgres database. 
To use Postgres dj_database_url and  psycopg2-binary must be installed. Comment out the default database in settings.py and instead provde the database URL from Heroku so that original database settings are not in version control.
Then run migrations. Write an if statement so that if the app is running on heroku where the database URL environment will be defined connect to Postgres otherwise sqlite. 
Install the gunicorn webserver. Create a Procfile to tell Heroku to create a web dyno which will run gunicorn. Temporarily disable collectstatic so heroku won't try to collect static files on deploying. 
Add host name of Heroku app to allowed hosts in project level settings. Push to github then git push heroku master.


[AWS](https://aws.amazon.com/) - hosts static files and image files. Create a group. Attach a policy that allows full S3 access to the bucket.
Create a user who is part of the group and who has their own special access keys

## Credits

### Contents

[Backgound Image](https://www.pinterest.de/pin/362187995028110882/)

Product images downloaded from [kaggle](https://www.kaggle.com)

### Acknowledgements

Thank you to Chris at Code Institute Dublin for putting an ecommerce website together so we students can learn what 
Full Stack Development really means and potentially start our own online stores. I would never have come close to this without you!