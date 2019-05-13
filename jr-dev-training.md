# Jr Developer Training Schedule

Welcome to the team! We are very happy to work with you! We want you to feel comfortable coming to any of us with questions. Remember one of the dev team values is: **SHOUT for help**. Don't spend hours turmoiling over an issue. Bubble it up quickly and loudly. That said, it may be hard to know what you don't know. This guide exists to help train you up quickly.

You will go through each of these sections with your work buddy. Each day will consist of:

* 1 hour of lecture
* 3 - 4 hours of self study


The rest of your day should be spent contributing to live code. After all, the best way to learn is to dive in and do it! Your work buddy will get you into our Jira system, find some good tickets for you to work, and assign them to you.

## Training Schedule

### Day 1
#### Routes, MVC, Rails, and Heroku

1. Web requests, REST, and routes
1. Error driven development
1. Building Controllers from scratch
1. Generators vs Scaffolds
1. Building Views from scratch
1. ERB is gross. Lets learn HAML!
1. Deploying to Heroku
1. Common Heroku commands/debugging

##### Homework/Self Study
Spin up a new rails app to blog about your first few days here! The app should have a Posts Table with `title:string` and `body:text` attributes. It should also have a Comments Table with references to the posts tale _(a post can have many comments)_.

**Do NOT** use scaffolding/generators for your routes, views, or controllers. You can generate your models because we want the timestamped migration files built for us, but that is it!

Deploy this application to Heroku. Write up a small blog post about what you learned today (repeat this every day for the next five days). Post a link daily in Glip to let the rest of the team comment/cheer you on!


### Day 2
#### Ruby Classes, OOP, and Gems

1. Classes, Instances, and Modules
1. Namespacing
1. Inheritance
1. Undefined method for nilclass
1. Common Gems we use
    * Better Errors/Binding of Caller
    * Devise
    * Bullet

##### Homework/Self Study
Add Devise to your blog (so users have to sign up and sign in/out to write posts or comments). Update your relationships/models so a User can have many posts and many comments.

Add Better Errors and Binding of Caller to your Blog

Add Bullet to your Blog. Fix any N+1 errors it detects

Get a membership to GoRails.com from Jeff (our VP of Technology). Sign in and watch the training videos on some of the gems we use most often: Devise, Pundit, Doorkeeper/JWTs, etc. Keep coming back to this place anytime you are faced with a new gem or feature we need to implement. A few minutes of training can greatly accelerate your code!

### Day 3
#### Testing with RSpec, Capybara, and Faker

1. Model testing
1. Faker all the things!
1. Rules of testing
1. Setup, execute, expect
1. Controller testing
1. Integration/regression/feature testing

##### Homework/Self Study
Add unit tests for your models (using shoulda_matchers mostly) and integration tests using Capybara to your blog. Use the simplecov gem to determine what level of coverage you have as you go. Once you hit better than 75% coverage, you are good to move on.


### Day 4
#### ActiveRecord, SQL, and the DB

1. ActiveRecord common methods: `.new, .create, .save, .persisted, .valid, .errors`
1. Writing native SQL
    * SELECT
    * FROM
    * LIMIT/DISTINCT
    * JOIN
1. Outputting ActiveRecord SQL queries
1. Blazer

##### Homework/Self Study
Install Blazer on your blog. Write some queries to show each users Posts and each users Comments (using dynamic variables).

### Day 5
#### The state of Spectrio

This section will really vary depending on the current state of each application and what we need to focus on. But the gist is this:

1. Cover all the current applications we support
1. Go over as much vocabulary as possible:
    * 1Portal/Cloud
    * 905x/Purple Box
    * Spectrio Connect
    * CMS/Engage CMS
    * FeedServer/Proxy Server
    * Codigo
    * Overhead Music/GRRID

##### Homework/Self Study
You've drank enough from the firehose this week ;) . Enjoy the day! Take it all in! Ask questions! Keep moving forward!
