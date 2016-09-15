# AngularJS Architecture
This project has the main objective to present and centralize the ideas of a well defined and solid Architecture for AngularJS. Feel free to contribute, contest or just read :)

# Motivation
This idea began from some experiences that we had while working with JS applications, where we wasted time with solutions that could be much better if we had a simple and organized file structure.

Therefore, we are developing this architecture to provide a start point for a scalable, simple and quick web application. This solution is based on our experience with web applications and desire to create something that can be helpful to the community.

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

###Module
A module is the biggest possible categorization of the client's business, it represents something very important for client, that certanily will have sub-divisions (flows) and also specific resources for that. 
Something very important is that a module is not a folder for only scenes, we will also put **shared resouces** inside of it. For example, if I have specifics constants for for that module, the file will be on module's folder.

A good example of modules for a bank application should be:

`investments`

`cards`

`transfers`

`ui-components`

###Scene
A Scene is a flow that we will have on our application, if for example, inside the `investments` module, I will problably have a page that list all investments so a good scene will problably be `listAll`. Each scene should have a folder, for group your resources.

Only remembering... If we have a resource that will be shared by another scenes of that module that resource belongs to the **MODULE** not to the **SCENE**.

###Resources
The resources are the files, they can be putted on the module folders, if they are shared between the scenes, or inside the scene folder, if they are specifics for that flow.

But... what resources could be?

- **Services**: login.service.js
- **Factories**: login.factory.js
- **Controllers**: login.controller.js
- **Views**: login.html
- **Templates**: loginHeader.tmpl.html
- **Directives**: keyboard.directive.js
- **Constants**: httpStatus.constants.js


#Conclusion
Pretty simple hum? The real thing is that is no more than a folder division!
Every time that you have a doubt about if something deserves to be a module, or if a resource is from module or from scene, discuss with your collegues! This is very important because discussing we can reach all the possibilities of non-covered cases by this architecture.

#Examples
[Example Folder](https://github.com/johnpapa/angular-styleguide/blob/master/a1/README.md "Angular Style Guide - John Papa")

#Getting startted!
[Yoman Plugin](https://github.com/johnpapa/angular-styleguide/blob/master/a1/README.md "Angular Style Guide - John Papa")

#References
[Angular Style Guide - John Papa](https://github.com/johnpapa/angular-styleguide/blob/master/a1/README.md "Angular Style Guide - John Papa")

[Clean Architecture - Uncle Bob](https://8thlight.com/blog/uncle-bob/2012/08/13/the-clean-architecture.html "Clean Architecture - Uncle Bob")