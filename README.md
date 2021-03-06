# Simplex
## Create your own framework on top of the Symfony2 Components
This repository is based off the tutorial by [Fabien Potencier](https://github.com/fabpot) entitled "Create your own framework... on top of the Symfony2 Components."

The tutorial is broken into 12 parts. Each completed section of the tutorial is tagged using a version number, such as "1.0" for Part 1, "2.0" for Part 2 and so on.

## Set-up
In order to access the exercises, you'll have to check out a copy of the repository...

````
$ git clone git@github.com:coreymcmahon/Simplex.git
````

You can then shift between the different versions of the repository used throughout the 12 part tutorial using the syntax:

````
$ git checkout [version]
````

... where [version] is the tag you'd like to use, such as:

````
$ git checkout 2.0
````

Also, you'll need to install Composer to pull down the dependencies. To do this, execute the following command from within the project directory:

````
$ curl -s http://getcomposer.org/installer | php
$ php composer.phar install
````

Enjoy!


## Part 1 - Installing Composer
In this lesson we learn how to install [Composer](http://getcomposer.org/), a package management tool for PHP projects. We then start building our framework by importing the Symfony2 autoloader and creating the first iteration of our "Hello" application.

[The lesson](http://fabien.potencier.org/article/50/create-your-own-framework-on-top-of-the-symfony2-components-part-1)


## Part 2 - Using the HTTP Foundation classes
Next, we use the Symfony2 HTTP foundation library to provide an abstraction over the HTTP layer.

[The lesson](http://fabien.potencier.org/article/51/create-your-own-framework-on-top-of-the-symfony2-components-part-2)


## Part 3 - Implementing the "Front Controller"
To provide more control over the flow of requests into and throughout our framework, we implement a "front controller." This involves creating a class through which all requests are routed. We also start to use templating to provide more flexibility in the view layer of our framework.

[The lesson](http://fabien.potencier.org/article/52/create-your-own-framework-on-top-of-the-symfony2-components-part-3)


## Part 4 - Introducing the Routing component
Now that we have a front-controller and a method of abstracting the flow of HTTP requests and responses through our application, we can start to decouple the format of URLs from the flow of control. We do this using the Symfony 2 Routing component.

[The lesson](http://fabien.potencier.org/article/53/create-your-own-framework-on-top-of-the-symfony2-components-part-4)


## Part 5 - Adding Controllers
We now have a pretty solid base for our framework. We have an abstraction over the HTTP layer, all requests are handled by our internal application logic via the front controller (as opposed to the web server responding to requests for specific resources) and we have a robust mechanism for handling routing URL requests to relevant response objects. The next step is to break out the logic responsible for creating responses into separate units known as **controllers**. 

Note that the end of the lesson introduces a new application for calculating whether or not the current year is a "leap year" or not. This new application is tagged as "5.1" in the repository (the previous application modified to include controllers as discussed in the previous paragraph is tagged as "5.0").

[The lesson](http://fabien.potencier.org/article/54/create-your-own-framework-on-top-of-the-symfony2-components-part-5)


## Part 6 - Using the Symfony 2 HTTP Kernel
In this lesson the Symfony 2 HTTP Kernel is introduced so that Controllers can be "lazy-loaded" when defining our routes. This means that instead of having to instantiate instances of each controller class when defining routes _just in case_ we need it to service the current request, we can use the HTTP Kernel to work out which controller is going to be used and then create an instance of that single class.

[The lesson](http://fabien.potencier.org/article/55/create-your-own-framework-on-top-of-the-symfony2-components-part-6)


## Part 7 - Moving towards MVC
In part 7 we create our own namespace for our evolving framework and split up the components according to the model view controller design pattern.

[The lesson](http://fabien.potencier.org/article/56/create-your-own-framework-on-top-of-the-symfony2-components-part-7)


## Part 8 - Adding Tests with PHPUnit
At this point we have a fully functioning MVC framework, built using the Symfony 2 components. Before we do any further work on developing the framework, it's time to step back and write some tests for the existing code using the PHPUnit framework.

[The lesson](http://fabien.potencier.org/article/57/create-your-own-framework-on-top-of-the-symfony2-components-part-8)


## Part 9 - Using the Event Dispatcher
In this lesson we learn how to make our framework extensible by adding events throughout the request handling process using the Symfony 2 event dispatcher.

[The lesson](http://fabien.potencier.org/article/58/create-your-own-framework-on-top-of-the-symfony2-components-part-9)


## Part 10 - Caching Requests
For large scale web applications, one of the most important ways we can decrease server load is by caching responses. In Part 10 we learn how to add Caching to our framework.

[The lesson](http://fabien.potencier.org/article/59/create-your-own-framework-on-top-of-the-symfony2-components-part-10)


## Part 11 - Using an Event Driven Architecture
In this lesson we refactor the code to make better use of the HttpKernel component and it's standard implementation which uses events to trigger routing.

[The lesson](http://fabien.potencier.org/article/60/create-your-own-framework-on-top-of-the-symfony2-components-part-11)


## Part 12 - Introducing the Dependency Injection container
In the final lesson we use the Symfony 2 dependency injection component to manage dependencies and configuration between the different components in our application.

[The lesson](http://fabien.potencier.org/article/62/create-your-own-framework-on-top-of-the-symfony2-components-part-12)