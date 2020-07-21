Today we're going to create the database and models for a simple trail tracker which allow a user to track information about trails they have hiked.

## Migrations
- Create a migration for a Users table.  A User will have a name and email.
- Create a migration for a Trails table. A trail will have a name, location, and length (all strings). A trail will be associated with a user.
- Add a birthdate column to the Users table
- Add a difficulty column to the Trails table
- On the Trails table, change the type of the 'length' column to 'integer'
- Run your migrations
- Where will you check to see if your migrations were successful?

## Models
- Create a User model
- Test your model in console with ActiveRecord methods
- Create a Trail model
- Test your model in console with ActiveRecord methods
- Set up your associations: a User can have many trails, and a Trail _______ __ a ____.
- Add some dummy data to your db.  (Use the Faker gem if you wish.  Create and run a seed file if you're feeling really ambitious!)

- In console, test your associations by getting a User instance and saving it to a variable.  Get a collection of that user's trails.  Use ActiveRecord methods for everything
- Test your association in the other direction using AR methods.  Save an instance of a trail to a variable, and query that trail's user with AR.

- Now you've done Create and Read functions with your database. Time to test Update and Destroy!  Update a record through your model(s).  Delete one.

- We want to display a user's age, so let's create a custom method that will allow us to call `@user.age` on a user instance and will return an integer of their age today.  (Hint: check out `Date.now` in Ruby)

## Association Methods

Let's use more of those methods AR gives us when we define model assocations using macros like `:has_many`

- create a new trail object and create it's association to an existing user instance by chaining ActiveRecord methods

- chain AR methods to find out how many trails belong to an instance of user
- chain AR methods to delete all of the trails the belong to an instance of a user