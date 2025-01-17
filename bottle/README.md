# What is Bottle?

Bottle is a free and open source web application framework, written in Python. A web framework is a set of components that helps you to develop websites faster and easier.

When you're building a website, you always need a similar set of components: a way to handle user authentication (signing up, signing in, signing out), a management panel for your website, forms, a way to upload files, etc.

Luckily for you, other people long ago noticed that web developers face similar problems when building a new site, so they teamed up and created frameworks (Bottle being one of them) that give you ready-made components to use.

Frameworks exist to save you from having to reinvent the wheel and to help alleviate some of the overhead when you’re building a new site.

## Why do you need a framework?

To understand what Bottle is actually for, we need to take a closer look at the servers. The first thing is that the server needs to know that you want it to serve you a web page.

Imagine a mailbox (port) which is monitored for incoming letters (requests). This is done by a web server. The web server reads the letter and then sends a response with a webpage. But when you want to send something, you need to have some content. And Bottle is something that helps you create the content.

## What happens when someone requests a website from your server?

When a request comes to a web server, it's passed to Bottle which tries to figure out what is actually requested. It takes a web page address first and tries to figure out what to do. This part is done by what's called a decorator function.  It will look at the route being requested and match it against a series of functions which are decorated with routes.

Imagine a mail carrier with a letter. She is walking down the street and checks each house number against the one on the letter. If it matches, she puts the letter there. This is how the route decorator works!

In the *view* function, all the interesting things are done: we can look at a database to look for some information. Maybe the user asked to change something in the data? Like a letter saying, "Please change the description of my job."  The *view* can check if you are allowed to do that, then update the job description for you and send back a message: "Done!" Then the *view* generates a response and Bottle can send it to the user's web browser.

Of course, the description above is a little bit simplified, but you don't need to know all the technical things yet. Having a general idea is enough.

So instead of diving too much into details, we will simply start creating something with Bottle and we will learn all the important parts along the way!
