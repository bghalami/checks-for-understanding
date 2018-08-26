## Week Two - Module 2 Recap

Fork or re-pull this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!). 

Note: When you're done, submit a PR.


### Week 2 Questions

1. At a high level, what is ActiveRecord? What does it do/allow you to do?
Active record translates multiple database languages in one easy to use package. It lets you create queries and query accessories.
2. Assume you have the following model:

```ruby
class Team << ActiveRecord::Base
end
```

What are some methods you can call on `Team`? If these methods aren't defined in the class, how do you have access to them?
Team.all, Team.find, Team.where. We inherit them from ActiveRecord

3. Assume that in your database, a team has the following attributes: "id", "name", owner_id". How would you find the name of a team with an id of 4? Assuming your class only included the code from question 2, how could you find the owner of the same team? Team.find(4). Owner.find(Team.find(4).owner_id)

4. Assume that you added a line to your `Team` class as follows:

```ruby
class Team << ActiveRecord::Base
  belongs_to :owner
end
```

Now how would you find the owner of the team with an id of 4?
???Team.find(4).owner???

5. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.
Teacher has_many Students, Student belongs_to Teacher
6. Define foreign key, primary key, and schema.
Foreign key is the id matching up to a row of a different table.
Primary key represents a row of data.
Schema is a blueprint for your database.
7. Describe the relationship between a foreign key on one table and a primary key on another table.
A foreign key represents data that can be called from a row on another table.
8. What are the parts of an HTTP response?
Status line, status code?

### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.
#find - because I'm always looking for stuff.
#where - because I need to know where things are.
#find_by - because these are really the only three methods I have memorized
#avg/sum - because, like the 80/90s barbie said, math is hard.

2. Name your three favorite ActiveRecord rake tasks and describe what they do.
3. What two columns does `t.timestamps null: false` create in our database?
created_at, updated_at
4. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?
ONE school to MANY teachers
5. In the same database, what will you need to do to create this relationship (draw a schema diagram)?
6. Give an example of when you might want to store information besides ids on a join table.
7. Describe and diagram the relationship between patients and doctors.
8. Describe and diagram the relationship between museums and original_paintings.
9. What could you see in your code that would make you think you might want to create a partial?

### Self Assessment:
Choose One:
* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:
* I feel comfortable with the content presented this week
* I'm somewhere in the middle of here... mostly comfortable.
* I feel overwhelmed by the content presented this week
