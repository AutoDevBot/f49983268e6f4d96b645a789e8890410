# AutoDevBot
AutoDevBot is an API monitoring service using open source API testing frameworks.  The first REST API testing framework we are supporting is [Frisby.js](http://frisbyjs.com/).  You can also run the same monitors/tests on your local computer for either development purposes or just to make sure it works before letting AutoDevBot run it continuously.

# How To Use AutoDevBot

## 1. Sign up
Sign up : [http://autodevbot.com/signup.html](http://autodevbot.com/signup.html)

## 2. Clone the repository we created you

Login and goto the live dashboard:  [https://api.autodevbot.com/dashboard/login.html](https://api.autodevbot.com/dashboard/login.html)

You can find the URL in your live events dashboard

    git clone https://github.com/AutoDevBot/<YOUR_REPO_URL>.git

## 3. Edit a monitor

Lets edit one of the pre-made working monitor that we created for you.  This monitor is running against our test API server.  Edit this file in your repository

    <REPOSITORY_HOME>/Frisby.js/AutoDevBot.com/UserProfileTest_spec.js

Lets make a simple change to show you how AutoDevBot works.  Change line 20 from "Number" to a "String".  This means that it will be expecting a value of a string instead of a number in that JSON field.  This will produce an error.

    20 | 			"age" : String

## 4. Commit and push

To make AutoDevBot run your new changes you simply just have to commit and push the code back into GitHub.

     git commit -m "my first changes" -a

     git push origin master

## 5. AutoDevBot automatically deploys new code

In your live dashboard, you will see a message that AutoDevBot has seen the changes and is deploying your new code.  Since we just created errors, you will see error messages in your live dashboard now.


# Video Demo
Check out this video demo blog: [http://blog.autodevbot.com/2014/03/11/ive-signed-up-what-now/](http://blog.autodevbot.com/2014/03/11/ive-signed-up-what-now/)

# How to Run Frisby.js Locally

You can got directly to [Frisby.js](http://frisbyjs.com/) site and follow their instructions or read this [blog](http://blog.autodevbot.com/2014/03/13/running-monitors-locally/) we wrote on how to run Frisby locally.

# About This Repository
This repository contains working tests that you can run locally or with the AutoDevBot service.  This is also the repository content that we will put into the repository we create for you when you sign up.  We will continuously add more sample tests in here to make it easy for you to get started and test 3rd party APIs that you might use.  You simply have to copy it over to your repository.
