
## 1- Who is Roy Fielding?
-  He helped write the first web servers, that sent documents across the internet

## 2- Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world?
- Machines don't have a universal noun - that's why they suck. Every programming language, database, or other kind of system has a different way of talking about nouns.

## 3- What is the HTTP protocol that Fielding and his friends created?
- is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a web page.

## 4- What does a GET do?
- The web page just specifies the URLs to the images and the browser goes and does more GETs using the HTTP protocol on them until all the resources are obtained and the web page is displayed. 

## 5- What does a POST do?
> - If one system needs to add something to another system, it would use an HTTP verb of POST.

## 6- What does PUT do?
> - If a system wants to replace something in another system, it uses an HTTP verb of PUT

## 7- What does PATCH do?
> * If a system wants to do partial updates to something in another system, it'll hopefully use PATCH.

## Resorces : 
- https://gist.github.com/brookr/5977550