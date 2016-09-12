# AngularJS Architecture
This project has the main objective to present and centralize the ideas of a well defined and solid Architecture for AngularJS. Feel free to contribute, contest or just read :)

# Motivation
The motivation of write a clean code, with well defined resposabilities should not be a motivation of an AngularJS Architecture but for all projects that evolve people working toghether but our main objective is share patterns that worked with us on **real projects**, not only on speaks.

We also would like to listen and improve this guide, we doesn't promisse you an iron bullet but we promisse something that will make you sufer less :D 

# Premises
- This guide supposes that you have a minimum knwoledge of AngularJS, in order to understand the responsabilities of each angular component.

# Introdution
> What's the biggest gap when a new person enter on a on going project?

There are many gaps when we have a new person on our team, but in my point of view, the biggest one is the **BUSINESS GAP**.

It's expected from a person that will work with AngularJS that he/she knows a little about it, but about the client's business is almost impossible.

Based on that, this Architecture is build on the top of the client's **BUSINESS**. The client's business is the most important think on the software, we should put it on evidence.

In comparison with others architectures, that put the **RESOURCES TYPES** as the most important think on the project, this architecture tries to make the thinks simpler for whom are looking at the first time for the project. 

`js/controllers`

`js/services`

`js/directives`

`templates`


You will see above, some comparsion with other project organizations.

#Categories
So, based on our main "rule", that is categorize the projects based on client's business, we thought in a folder division like this:

- Modules
	- Module
		- Scene
			- Resources


###Modules
###Module
###Scene
###Resources

#References
[Angular Style Guide - John Papa](https://github.com/johnpapa/angular-styleguide/blob/master/a1/README.md "Angular Style Guide - John Papa")

[Clean Architecture - Uncle Bob](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html "Clean Architecture - Uncle Bob")