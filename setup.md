# Setup
Its time to setup your laptop! This can be a bit of a process, but fret not; we are here to help!

## IDE
Feel free to use your IDE of choice. Vim, Sublime, Atom, VS Code, whatever. Use whichever tool you feel most comfortable with. Currently the majority of the team use VS Code. We like its ease of entry, extensibility, and built in terminal. 

## Setapp
You will be invited to Setapp by Jeff. Think of Setapp as the "Netflix for Mac Applications". Some of the applications you will need from Setapp are PAW (Postman on steroids), CleanMyMac, and whichever SQL GUIs you find a need for. Be sure to run CleanMyMac once every couple weeks to keep your laptop's HDD clean and its OS well maintained.

## Tower
Tower is our defacto Git GUI. Feel free to contintue to use Git's CLI, but there are times when Tower can be an absolute lifesaver! Things like cherry-picking, soft/hard resets, and commit squashing are so much easier in Tower than in the CLI. You will get an invite to install Tower with a CAL in your email on your first day.

## Slack/Glip
This is our default chat application. Communication is vital in our world. Especially if you are remote. Be sure to sign in daily, keep an eye on the important channels, and communicate early/often if you are working remotely.

## 1Password
You will be invited to join 1Password on your first day. This is where we store all of our shared credentials for the applications, tools, etc. In general, letting 1Password generate a password and storing it for you is the safest way to keep all of your logins secure. Ask someone for help if you are unsure how to use this tool properly.

## Node, Ruby, Rbenv/RVM, Homebrew, etc.
Many of our applications run on Ruby/Ruby on Rails. Rails is a full feature framework with a good number of dependancies. And well...Node is everywhere. So at a bare minimum, you will need Node, a Ruby Version Manger, Ruby, the Bundler Gem, the Rails Gem, and a host of other tools. Here are a couple ways to do this:

1. Thoughtbot's Laptop Script - https://github.com/thoughtbot/laptop
    * Pros: It is a quick/easy thing to do
    * Cons: It is opinionated and installs a few extra things that you probably don't need/want
2. Follow these steps
    * Install Node - Installer app from https://nodejs.org/en/
    * Install Homebrew - `/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`
    * Use Homebrew to install Postgresql - `brew update && brew install postgresql`
    * Use Homebrew to install Rbenv - `brew install rbenv`
    * Use Rbenv to install the Ruby versions you need - `rbenv install <RUBY VERSION>` - Pay attention to the post install here. You will probably need to update your bash/zsh profile to get rbenv into your PATH. You can then use `rbenv local <RUBY VERSION>` to set the ruby version for that folder/subfolders or `rbenv global <RUBY VERSION>` to set the system wide default ruby version. More info here: https://github.com/rbenv/rbenv
    * Install the Bundler gem to each of those ruby versions - `gem install bundler`
    * Install Rails `gem install rails -v <RAILS VERSION>`
    