# POST a Gift

![puppy mail](https://media.giphy.com/media/hTsAAaYV5nRjq/giphy.gif)


You'll be working with the [holiday shopping API](http://localhost:3001/items) from Day Three. This time, you'll focus on writing some POST requests!

You'll be writing the functionality of this gift list adding application. The HTML and CSS have been written for you, so that you can focus on the functionality, but you will need to add a little bit for your messages. 

**User stories for the functionality to build**
* As a user, when I fill out the form to add a new gift, I should see a message indicating that it was successful. 
* As a user, I am not able to submit the form unless I have provided a recipient, name of gift and price. 
* As a user, I can submit the form without providing an optional link. 

_Make sure to consider the user experience! For every step, think about what information the user would want to see!_

** The API **
You'll need to use this [Holiday Shopping API](https://github.com/turingschool-examples/holiday-shopping-api) to complete your tasks. Please follow the instructions in the Holiday Shopping API README to run the API locally. You'll need to have this running while you're working. 

## Endpoints

| Description | URL | Method | Required Headers | Required Properties for Request | Sample Successful Response |
|----------|-----|--------|---------------------|-----------------|
| Get all items |`http://localhost:3001/items`| GET  | none | none | An array containing all items |
| Add item |`http://localhost:3001/items` | POST  |  'Content-Type': 'application/json' | `{ id: <number>, recipient: <string>, name: <string>, priceInDollars: <number> }` | "Item #<id number here> has been added!" 
| Delete an item | `http://localhost:3001/items/<id number here>` | DELETE | none | none | "Item #<id number here> has been deleted" 
  
_Hint: Check out the POST request lesson for more details - find it in the lessons list or calendar._
_Note:  Make sure you are using unique id numbers for each POST, and you might want to experiement with DELETE._

**BONUS**
* You don't _need_ to have a class to achieve the above functionality, but try adding one anyway. Make sure you're writing tests for it too. What benefit does this give you to use a class vs. storing everything in `script.js`?
* Submitting the gift form could be a bit more exciting. Try implementing this [canvas-confetti npm package](https://www.npmjs.com/package/canvas-confetti) to set off some confetti when the submit button is clicked. Thanks to Tony for finding this cool package!
* Get some more practice with GET requests, and design a way to display the list of all the gifts. Remember to focus on clean CSS, and make sure this matches with the overall theme of the application. 
