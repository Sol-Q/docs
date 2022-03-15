* Step 1:
Before user gets access to the doxabeta neo, first the user must register. User can register with his email and full name. Please do not forget to select the option “I’m not a robot” This is the link for registration. (http://designer.flexberry.net/#/login-or-register?goto=index) and below is an example of the interface

![A typeusage](/Diagrams/doxabeta-neo-registration.png)

* Step 2:  
After successfully registering. User can log in with the email used for the registration and the password which was automatically sent to your email. This is how the interface looks like when you log in

![A typeusage](/Diagrams/doxabeta-neo-after-login.png)

* Step 3:
You select all projects, then create Project. You fill the field with your project name and then select create project.

![A typeusage](/Diagrams/doxabeta-neo-creating-project.png)

* Step 4:
You click on create diagram and then select the type of diagram you want to use for modelling your subject area. For example, “class diagram”.

![A typeusage](/Diagrams/doxabeta-neo-select-type-diagram.png)

* Step 5:
There are tools available to be used for modelling the subject area. The below diagram shows how the interface appears. After designing your diagram, you need to save your project before proceeding to the next step. It is necessary to enter the diagram name before saving.

![A typeusage](/Diagrams/doxabeta-neo-designing-interface.png)

* Step 6: 
Before proceeding to generate your application, additional metadata should be created that is (a class Diagram for forms, projections for classes of subject area, and an application menu structure). To do this, the user should click on the Navigation menu, then click on "Create projections, forms and application" as shown in the picture below. 
![A typeusage](/Diagrams/doxabeta-neo-navigation.png)

* Step 7:
It is possible for the user after completing step 6, to change the Navigation menu of the application before proceeding to generate.

![A typeusage](/Diagrams/doxabeta-neo-navigation-menu.png)

* Step 8: 
To generate your application, you need to select “Generation” from the menu list. Remember to select the option “Publish to gh-pages” from the Ember JS generation setting.

![A typeusage](/Diagrams/doxabeta-neo-generation.png)

* Step 9: 
On the GitHub account, there will be source code for the backend and frontend. You can clone the repository to your local machine. Flexberry platform also generates a docker file to run your application on a local machine. Example of how the Flexberry platform generates source code for applications on GitHub is like the below picture

![A typeusage](/Diagrams/doxabeta-neo-generation.png)

* Step 10:
The src file contains a Docker file, generated Database (SQL), the backend application and the frontend application.

![A typeusage](/Diagrams/doxabeta-neo-src.png)

**NOTE**: 
When you click on the README.md file, in “Application deployed on GitHub Pages” User can click on this link and deployed application will be open in a new browser tap. Please bear in mind that, Docker is the best way to run generated applications on localhost. This is not a required option, and this option is more suitable for the developers. It is just the simple way to run your generated application using the link the red arrow points to in the picture below. Application deployed on GitHub pages works with IndexedDB to store all data and no use of the backend when the user opens this link.The best option to run an application with the backend is to follow the steps for running the application in Docker and get the application at the available localhost.

![A typeusage](/Diagrams/doxabeta-neo-appnote.png)

* Step 11:
You can now run the application in Docker. The steps to start running docker is shown in the picture below

![A typeusage](/Diagrams/doxabeta-neo-run-docker-files.png)

* Step 12:
After successfully running your application in docker, you can see your application at localhost. You copy the link and paste it into your browser. The below diagram shows an example of a generated application after running in docker. The application frontend running on GitHub Pages (via a link from **note**) is the same that running inside docker and it looks the same way as in the picture below

![A typeusage](/Diagrams/doxabeta-neo-generated-app.png)