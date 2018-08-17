## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 1 Questions

1. List the five common HTTP verbs and what the purpose is of each verb.
  GET, POST, PUT, PATCH, DELETE
2. What is Sinatra?
  A web framework built off rake.
3. What is MVC?
  Model View Controller
4. Why do we follow conventions when creating our actions/path names in our Sinatra routes?
  Readibility 
5. What types of variables are accessible in our view templates without explicitly passing them?
  instance variables
6. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template? above the line 'erb :index' add @count = 1

  ```ruby
  get '/horses' do
    erb :index
  end
  ```

7. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?
  locals => { :variable => variable }
8. What's the purpose of ERB?
  We can embed ruby into our html
9. Why do I need a development AND test database?
  One to run our code and save db on, and one to pump controlled data into
10. What is CRUD and why is it important?
  Create Read Update Delete
    It encapsulates everything our methods can do.
11. What does HTTP stand for?
  Hypertext Transfer Protocol
12. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?
  <% %> runs code
  <%= %> prints code
13. What's an ORM? What does it do?
  Object Relational Mapper
  It lets our databses talk to eachother
14. What's the most commonly used ORM in ruby (Sinatra & Rails)?
  ActiveRecord
15. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.
get '/restaurants':display all restaurants
get '/restaurants/edit' :display edit page
put '/restaurants/edit' :makes edit
get '/restaurants/create' :display create page
post '/restaurants/create' :makes creation
get '/restaurants/:id' :shows individual restaurant page'
delete 'restaurants/:id' :deletes the restaurants





16. What's a migration?
  It's the template for the database
17. When you create a migration, does it automatically modify your database?
  No
18. How does a model relate to a database?
  A model is blueprint for the object going into a database
19. What is the difference between `#new` and `#create`?
  #new makes a new model, but doesn't save it to the db.
  #create makes a new model and saves it to the db
20. Given a table named `animals`, What is the SQL query that will return all info from that table?
    `id     name        number_of_legs
    -----   ------      --------------
      1     panda       4
      2     giraffe     4
      3     whale       0
      4     bird        2
    `
  SELECT * FROM animals
  
21. Using the same table, What is the SQL query that will return only the animals that has 4 legs?
SELECT * FROM animals WHERE number_of_legs=4

### Review Questions:  
22. Given a CSV file (“films.csv”) with these headers [id, title, description], how would you load these into your database to create new instances of Film?  
  CSV.foreach("path/to/films.csv") do |row|
    Film.new(row)
  end

23. Given the following hash:
```
activities = {
  hiking: {cost: $0, supplies: ['hiking shoes', 'water', 'compass']},
  karaoke: {cost: $10, supplies: ['courage', 'microphone']},
  brunch: {cost: $35, supplies: ['mimosa flutes']},
  antiquing: {cost: $200, supplies: ['list of antique stores']}
}
```
How would I add 'granola bar' to things you should have when hiking?
activities[:hiking][:supplies] << "granola bar"

24. What are the 4 Principles of OOP? Give a one sentence explanation of each.
   Encapsulation: Keeping your code DRY and following SRP
   Data Abstraction: Keeping methods and classes short as possible.
   Polymorphism: Pretty much inheritance, with some twists...
   Inheritance: Using superclasses to pass qualities to lower classes.

### Self Assessment:
Choose One: (erase the others)
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel comfortable with the content presented this week
