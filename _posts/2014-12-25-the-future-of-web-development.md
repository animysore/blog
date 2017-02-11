---
layout: post
title: The Future of Web Development
description: What changes I (and a ton of other people) expect to see in the next generation of web development
modified: null
tags:
  - web development
  - crosspublished
image:
  feature: "abstract-13.jpg"
comments: true
share: true
published: true
---
<figure>  
    <a href="/images/2014-12-25-the-future-of-web-development/future-polymer-logo.svg">
        <img src="/images/2014-12-25-the-future-of-web-development/future-polymer-logo.svg" alt="">
    </a>
</figure>
>***The stuff that dreams of are made of*** " ~ The Maltese Falcon

Web Development is a fast paced, highly competitive and creative field. Commonly, there are two big parts to any web-based thingy. The front end, where the pretty stuff is. This falls under web design. Then we have the back end, where all the heavy machinery nestle. Technically only the back end falls under web development, but one cannot describe a house, without showing where the front door is.  In this article I have tried to collect the views of the people working behind in the concepts discussed, from many web posts. At the bottom, are a few resources you can look at if you are interested.

I wrote this article originally for the [**KHMD blog**](https://kumaranhmd.blogspot.in)
{: .notice}

Going a little into the annals of computer history, we find that the Internet, despite growing rapidly, did not grow in chaos. It was developed layer by layer, each step taken in a logical sequence. The development of the internet, began with the creation of efficient data transfer systems. With the creation of the World Wide Web, came the key components of our present internet - the web browser and the web page.

Sir Tim Berners Lee (All Hail!) also created the Hypertext Markup Language - HTML - along with the web. The first few versions of HTML were, to put it in a nice way, severely lacking. If it weren't for CSS, the Internet would be ugly.

### Web Apps will dominate the market

Across the world, there is great belief that web based applications will be the future - of not just the web - but also smartphone and desktop apps. The arguments put forth for proclaiming web apps as the next conquerors are quite simple. Web-browser based applications are easy create - they primarily use the languages and technologies used to build regular websites - and will run on a multitude of platforms with just some minor adjustments. Today, with the rise of several mobile and desktop operating systems, each with their own system type, each with their own specific set of programming languages to develop with, more and more people (developers to be precise) are clamoring for a unified technology that allows one to build an app once, and get it to work everywhere.

Putting it all together, the general idea, is that why not make applications which are run by a web browser as opposed to them being run directly by an operating sywww.polymer-project.org/images/logos/p-logo.svgstem - To create what is quintessentially an operating system which is run on top of another operating system.

>***Oh if it were only so simple*** ~ Aleksandr Solzhenitsyn

Unfortunately, the world functions in mysterious ways. Or in this case, in very clearly defined, but still mind-numbing ways. There are a host of problems in such a model. If one were to make a list, of all the hurdles we would need to cross to implement this idea *fully*, topping that list would be Performance. Native apps (Normal apps run by the operating system directly) are able change a variety of system settings in order to fit in exactly, so as to utilize as less system resources as possible, and yet function smoothly and give a rich user experience. Currently while it is possible to some degree to create an app that can run on a particular browser, with some effort on all browsers, and maybe with a lot more effort on all browsers on all mobile and desktop OS's (The time, human drudgery and expertise required will be high), such an app, will not be able to run nearly as well as a native app.

Google is spearheading the effort to integrate web and system apps, into a hybrid environment where BOTH native and web apps are treated on an equal level. It has designed an entire javascript based framework called Polymer (Explained later in this article) for the development of web apps, as well as another javascript based framework, Angular.js for the front end of web applications.

Here is a more detailed and well explained article regarding Google and Web applications : [The future of the web according to Google](https://divshot.com/blog/opinion/the-future-of-the-web-according-to-google)

### Flash of Death

One thing anyone can say for sure, looking at the present scenario, is that Flash will be driven to extinction. In 2010, Apple sounded the death knell for Flash by making iPad's and iPhone's incompatible with Flash. Google followed, and all versions of Android past ICS, do not offer any native Flash support. However HTML 5 is not replacing Flash at a rate which would be expected. Presently most browsers offer only limited compatibility with HTML 5, despite it being having more performance benefits. The vast majority of video streaming sites use Flash player, rather than HTML 5 based solutions. Even Youtube, still uses Flash Player, although it's rapidly going HTML. It looks like Flash is not going to go down without a fight.

<figure>  
    <a href="/images/2014-12-25-the-future-of-web-development/future-flash-gravestone.jpeg">
        <img src="/images/2014-12-25-the-future-of-web-development/future-flash-gravestone.jpeg" alt="RIP Flash">
    </a>
</figure>

### Javascript is the Future - JQuery, Node.js, Angular.js, Polymer.js

It looks like Javascript will be the Most-Wanted-Language of the next phase of the Internet. Javascript is currently the most used client-side scripting language. JQuery, a javascript library, is widely used for interaction and animation. Now, with the rise of several pioneer projects all based on javascript, javascript is set to be the true programming laionguage of the web.

I will go a bit into scripting languages here. All interactive, motile parts of a website or web app (barring hyperlinks and css effects) are powered by scripts. There is more than way to skin the proverbial cat, and web-developers use mainly two different techniques to run scripts.

`<Warning> Textbook definitions up ahead!`

Scripts can be run client-side, meaning your device takes instructions from a piece of code, and processes data accordingly. Client-side scripting languages mainly include javascript, javascript, and flash - Honestly flash is just for games - a measly 12% according to [w3techs](w3techs.com).  The other way of running scripts is from the server, where everything you feed to a website or app (location, clicks, hovers, text-entry) is sent to a server, where a server-side language, such as php or asp.net (by Microsoft) or python processes it, and sends data back to your device. The vast majority of websites use client-side and server-side scripts in tandem for maximum efficiency, security and speed.  


#### Node.js

In 2009, we witnessed the birth of Node.js, a server side scripting language based on Javascript. Node.js is being showcased as the successor the world's most widely used server side language php. It is possible to dismiss this as an absurd notion if we consider the vastness of php in terms of market-share, but we must keep in mind that Node.js is a very new language, and very efficient and light as compared to php. Linkedin does the backend of it's mobile apps using Node.js. Paypal (Gasp!) uses Node.js, and so do all [these guys](https://github.com/joyent/node/wiki/Projects,-Applications,-and-Companies-Using-Node). What is most important of all, is that Node.js is getting developers hooked.

<figure>  
    <a href="/images/2014-12-25-the-future-of-web-development/future-node-logo.png">
        <img src="/images/2014-12-25-the-future-of-web-development/future-node-logo.png" alt="Node.js">
    </a>
</figure>

#### Angular.js

Let me start off the introduction to Angular.js with this picture :

<figure>  
    <a href="/images/2014-12-25-the-future-of-web-development/future-angularjs-logo.png">
        <img src="/images/2014-12-25-the-future-of-web-development/future-angularjs-logo.png" alt="Angular in 4 words">
    </a>
</figure>

That's the story, in a nutshell. Angular is designed for dynamic views, the way HTML was designed for static pages. Angular is already insanely popular. Just head over to the homepage to start a simple tutorial right within your browser (Link below). Angular depends completely on your knowledge of javascript and HTML, and it allows for the creation of remarkable interfaces and functions for web apps. Angular provides pretty much the best framework  for developing web apps right now, be it interfaces, services or communication with servers.  

#### Polymer.js

Polymer is another project by Google, and it is, I have mentioned before, made for building web application components. Polymer is a new language that is still very much in development - I forgot to mention earlier, that it was launched in 2013. Polymer basically helps in building components, which together work to form a web app, or can directly be used in websites as modules for extra functionality.  While Polymer is a great concept, it is still looks like it's way ahead of it's time.

An article sounding alarm bells for Polymer : [Is Polymer.js the future of web application development?](http://www.toptal.com/front-end/polymer-js-the-future-of-web-application-development)

On a final note, I would like to remind you that Polymer's dependencies, although non-existent in the present, are already being made and standardized. Polymer uses several powerful features of HTML 5 not yet approved by the W3C, but hopefully, Polymer will succeed.

#### Back to Javascript

So I just listed three amazing javascript-based projects, all of which seem set to play a big part in next-gen web development. Now javascript-based here means a keen background knowledge of javascript, along with HTML and CSS will be required to do anything serious.

One last thing about javascript -  Khan Academy's programming tracks are largely javascript-centred too. The Hour of Code movement teaches js (A skinned version)
along with a few other languages.

### CMS (Content-Management Systems) on the rise

A rather small, but interesting thing to note is that the use of content management systems is on the rise. A CMS is generally used when there are large amounts of data to be posted on a website, or a large number of users post data to a website. Most blogging platforms like WordPress, Weebly and Blogger use CMS, along with e-commerce sites which use specialized CMS's such as Magento. If you want to use a CMS for your website (not one that is on a blogging platform) Drupal is highly recommended, as it is open source.

<figure>  
    <a href="/images/2014-12-25-the-future-of-web-development/future-cms-graph.png">
        <img src="/images/2014-12-25-the-future-of-web-development/future-thumb-cms-graph.jpg" alt="Angular in 4 words">
    </a>
</figure>

## Conclusion

The Web is now a shining beacon for all other fields of computer technology. Some of the greatest people in the field of technology and programming are developing for the web. There is a lot of room for ideas, and is a great area to point one's computer skills at. If you are interested web development, now is a great time to get creative. Check out the resources page of the KHMD blog for some general resources pertaining to web development. Below are some resources *specifically* regarding the technologies discussed in this article.

Thanks to  [**Gautam Padiyar**](https://plus.google.com/+GautamPadiyar)  for the ideas.

## Resources

***Before you start anything, head over to the homepages of these great projects. They give links to great learning resources, as well as lots of info concerning how why that project is really useful***  

Polymer - [polymer-project.org](http://polymer-project.org)

Node.js - [nodejs.org](http://nodejs.org)

Angular.js - [angularjs.org](https://angularjs.org)

***Enlightening posts***

Rey Bango's [Post](http://code.tutsplus.com/tutorials/using-polymer-to-create-web-components--cms-20475) on how to create basic elements in Polymer.

Angular and Polymer are very very similar. Here's a post laying out the differences : [Polymer vs. Angular](http://www.binpress.com/blog/2014/06/26/polymer-vs-angular/)

***Here are a few links to detailed lists of great goodies***  

[Node Cloud](http://www.nodecloud.org/) This website contains all the possible resources you will ever need to get started with Node.js, including details of different frameworks and IDE's.

[Udemy's Node.js tutorial](https://blog.udemy.com/node-js-tutorial/) Udemy has a beginners' course for learning MongoDB in Node.js. Great for someone who wants to launch themselves into a database-intensive NodeJS project.

[Github list of Angular JS Resources](https://github.com/jmcunningham/AngularJS-Learning) From what I infer after opening a fraction of the links to resources provided here - and they are great ones too - is if you want to begin with Angular Js, visit this page.
