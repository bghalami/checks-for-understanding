## Week Four Recap

### Instructions
Fork or re-pull this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Week 4 Questions

1. What is a cookie?
A piece of data stored locally
2. What’s the difference between a session and a cookie?
A session holds cookies
3. What’s a flash and when do you want to use flashes?
A flash is a little message that pops up telling the user something, you want to use it when something happens but you dont redirect.
4. Why do people say “HTTP is stateless”?
Because it is?
5. What’s authentication? Explain.
Authentication is how we tell our app if someone is logged in or not.
It looks at the session to find a user.
6. What’s the difference between authentication and authorization?
Authorization tells us who our user is and what they can do.
7. What’s a before filter?
It sets an action before another action takes place
8. How do we keep track of a user once they’ve logged in?
With a session!
9. When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?
Namespace when you're using a directory but not referencing something, use a resource when that certain thing is also referenced.
10. At a high level, what tools can you use to implement authorization? How would you use them?
Roles for a user. Set one to be admin, one to user, maybe one to manager
11. What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?
Enum's are methods that let us manipulate data in a very convenient way. We need symbols.
12. What are some strategies you can use to keep your views DRY?
 Using view refrences, like form renders and what not.


### Reviews Questions 
13. Given the following array of hashes, how would I print an alphabetical list of holidays?
```ruby
[
 {holiday: {name: "St Patrick's Day", supplies: ["Corned Beef and Cabbage"]}},
 {holiday: {name: "Halloween", supplies: ["Candy", "Costume"]}},
 {holiday: {name: "Hanukkah", supplies: ["Menorah"]}}
]
```  
array.map do |key, value|
 value[:name]
end.sort

14. How would you clean incoming data to ensure "$300" or "300.00" is stored as 300? 
  "$300" x.gsub("$","").to_i,  "300.00".to_i


### Self Assessment:
Choose One:
* I was able to answer most questions independently, but utilized outside resources for a few\

Choose One:
* I feel comfortable with the content presented this week
