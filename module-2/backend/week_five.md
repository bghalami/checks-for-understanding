### Week 5 Questions

Re-pull from this repository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 5 Questions
1. How do we make flash messages display on a page?
flash[:notice] = "You message here!"

2. Where is cart information/temporary information usually stored? sessions[:cart]

3. What might be some reasons not to store a cart in our database? Are there any reasons why we would want to persist that information? if you have an enormous cart that's using up a lot of space, saving 100000 users carts would take up a lot of space. 

4. What is the purpose of the asset pipeline? To make sure our code is working the way we expect it to in production.

5. Why do we precompile our assets? 

6. What do each of the following tags do?

```ruby 
<%= stylesheet_link_tag "application" %>
<%= javascript_include_tag "application" %>
<%= image_tag "rails.png" %>
```
style_sheet references CSS for our program, styling. javascript references any javascript being used on our site. image posts an image on our site.
7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project? version, special gems used, readable in laymens terms. Updating and writing a readme makes your code more likely to be used.

8. What are the top four accessibility issues that we as developers should be aware of? I don't believe we were taught this.

9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`? Callback. We'd put it in somewhere anytime we're saving data but something would need to happen first.

10. Given the following object, how would we create a scope for all users who are active? I don't believe we were taught this.

```ruby 
User.create(name: "Happy", active: true)
```

11. What is the difference between a scope and a class method? I don't believe we were taught this.


### Review Questions:  
12. Given the following hash:  

```ruby
{cart: {"17" => 4, "204" => 52, "29" => 22}}
```

  12a. How would you add item with id of 48 with a quantity of 4?  cart["48"] => 4
  12b. How would you increase the quantity of item 29?  cart["29"] += 1
  12c. How would you find out how many items your user is thinking about purchasing? x = 0, cart.each { |k, v| x += v }, x
  
13. What is polymorphism? How does it relate to duck-typing? What are two ways you use this in everyday Rails applications? Polymorphism is the ability for an inherited method to be used for something sorta different than the original use. You can use it to do things if it works, even if it's not the original intention. ActiveRecord calls and I don't know.  
14. How would you clean the string "(630) 854-5483" to "630.854.5483"?  


### Self Assessment:
Choose One:
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel comfortable with the content presented this week
