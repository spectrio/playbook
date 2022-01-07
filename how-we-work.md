# How we work
We believe in strong opinions, loosly held. If you believe in something, make a case for it. But be reasonable enough to hear all sides, and make the decision that is best for Spectrio and our values.

## Branch Naming Conventions
When spinning up a new branch, please preface it with your initials. i.e.  `git checkout -b as/new-feature`. In this example, 'a' and 's' are my initials (Alex Spencer). And the branch name is whatever I want it to be (so long as it comes after the `/`). This convention gives us a nice foldered look inside of Tower (our default Git GUI), and it makes it dead simple to see who did what.

## Commit Messages
Try to follow [the seven rules of a great Git commit message](https://chris.beams.io/posts/git-commit/#seven-rules)

1. Separate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Use the body to explain what and why vs. how

## Pull Requests
We encourage your workflow for saving progress while you code; however, we don't need to know every step you took to get to the end state. Before submitting a pull request, please squash your commits into one (`git rebase -i` is helpful here). The exception to this is when it would be helpful for the reviewer to logically break up the code with a few more commits.

When merging a pull request, use the "Squash and Merge" option from the drop down; this helps keep the log clean and purposeful.

## PR Peer Review
Unless told otherwise, every bit of code that goes into an app must be done through a pull request. In other words, directly committing to the master, staging, or production branches is a big no-no. In fact, we usually protect branches in Github settings to flat out prevent a direct push to master, but we may forget/miss that step...So just don't do it :).

Once you have submitted a PR, please choose 2 - 3 additional developers on the team and mark them as reviewers in your PR. This will notify all of them that you have a PR in need of review. **NOTE** ANY developer can leave a review on any ANY PR. This request for review process just keeps the wheels moving.

While submitting a PR, please provide a bullet pointed TL;DR list of things that the PR is actually changing. This will help the reviewer quickly identify the stated goal and if you implimentation meets that goal.

Once a PR has had one successful approval, it may be merged by either the approver or the person that submitted the PR.

## Jira and LeSS
You will be added to Jira and assigned to any project boards that your expertise may be valuable on. Each board is groomed weekly. We follow a LeSS style Scrum of development. In other words: 
    * Work your way down the board until you see something you feel comfortable doing.
    * Take work as you need it.
    * Do it right the first time (tested, clean code pls).
    * Then move onto the next job.
    * Deadlines are for journalists. We are developers. Don't waste time and certainly ask for help if you are stuck. But unless told otherwise, just do what needs to be done.

## Standups
We participate in daily standups. A standup is a quick meeting where we can get any company/team announcements from Jeff, then everyone states what they are working on and if they are blocked. That is it. If something that is mentioned kicks up a new conversation, the first person to say: _"We should probably pair on this"_ or _"We should take this offline"_ wins the standup!

## Form creation
HTML forms are everywhere. There isn't an web application on the planet that doesn't have at least one or two. We believe in using the Simple Form gem when the form is truly simple and using good old HTML when the form is more complicated. Examples of complicated forms are those with radio buttons or check boxes tied back to associated models or any nested form in general. If you aren't sure which tool to grab for here, ask.

## Prettier/Rubocop
We believe in convention is a tremendous tool. You will be expected to install the Rubocop (for ruby) and Prettier (for JS)extensions into your IDE. You will be given a config file that tells both of these code formatting tools about our agreed upon conventions. Please do not submit code that hasn't been properly formatted by their respective extensions.

## Bootstrap
Twitter's Bootstrap is our preferred CSS/UI/UX framework. Please use the latest version of it on all new projects.

## HAML over ERB
Our preferred templating language in Rails is HAML. ERB is horrible and ugly.

## Better Errors
Every Rails project we work on needs to have the better errors and binding of caller gems added to the development section of the gem file. This makes debugging code about 1000x easier. If you are unfamiliar with their use, please ask for a demo.

## Byebug
Sometimes we nee to debug something outside of the web. Rake tasks, scripts, etc. For those cases, we use byebug in all of our Ruby applications. To create a breakpoint add `byebug` into the code. Execute the code and it will pause with a live environment command prompt. More info about byebug here: https://github.com/deivid-rodriguez/byebug . If you prefer Pry (a similar gem), we are great with that too!

## ENV Variables
ENV Variables will either be stored in a .env file (using the dot-env gem) if the application is older than Rails 5.2. Any Rails application versioned over 5.2 will use the more modern encrypted credentials protocol. More information for both here:

  * Dot-env: https://github.com/bkeepers/dotenv
  * Encrypted Credentials: https://medium.com/cedarcode/rails-5-2-credentials-9b3324851336

## Markdown
We use markdown in all of our README's, and other technical documents. If you haven't already learned Markdown, please take some time to do so (about half a day is all it takes). Here is the guide: https://daringfireball.net/projects/markdown/syntax. If you have any questions about Markdown, please ask!

