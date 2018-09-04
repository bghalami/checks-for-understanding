## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Week 3 Questions

1. What is the entry at the command line to create a new rails app?
rails new app
2. What do Models generally inherit from in rails?
Application Record
3. What do Controllers generally inherit from in a rails project?
Application Controller
4. How would I create a route if I wanted to see a specific horse in my routes file assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?
resource :horse, only: [:show]
5. What rake task is useful when looking at routes, and what information does it give you?
rails routes
6. What is an example of a route helper? When would you use them?
  a route helper is shorthand for a route you can use. new_user, edit_admin_user
7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?
  _path is set by the helpers, _url is something we set
8. What are strong params and why are they necessary?
strong params are parameters that can be used only when properly passed in.
9. What role does `form_for` play in helping us create our forms?
it tells our form what it's affecting and where it's going
10. How does `form_for` know where to submit the user's input?
form_for's default method is post and it's based off whatever the form_for is is for
11. Create a form using a `form_for` helper to create a new `Horse`.
<%= form_for Horse.new do |f| %>
12. Why do we want to validate our models?
To make sure they are doing only what we want them to
13. What are the steps of the DNS lookup?
BROWSER TO OS TO ISP TO ROOT TO TLD TO ANS AND BACK

### Review Questions
14. Within a feature test and given the following HTML, write the code necessary to target the following section and check the person's name?

  `<section id="personal-info">
    <h3><%= @person.name%></h3>
   </section>
  `
  within(#personal-info) do
    it {should have_content(@person.name)}
   end 
15. How would you call the method `prance` from within the method `move` on a `Horse` instance?
  def move
    prance
  end 
16. Given the following hash:

```ruby
furniture = {table: {height: 3, color: "red"}, purchased: true}
```
What is the different between how you would return true vs returning 3?  
furniture[:purchased], furniture[:table][:color]
17. What is inheritance?
  It's how a class can use methods from a "parent" class.
### Self Assessment:
Choose One:
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel comfortable with the content presented this week
