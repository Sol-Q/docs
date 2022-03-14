## Creating basic types of diagrams. Basics of Information Systems design

## The order of Information system design 
The first step of an algorithm for designing an information systems is a problem statement, which should be defined:

+ characteristics of the automation object
+ define the main task to be implemented by the application
+ describe the business processes that will be implemented in the application

Next is to create a diagram of Use Cases, which is the most common representation of functional requirements of the system. It allows to describe the main processes that is needed to be implemented. It is useful to make an activity diagram, which is a flowchart that shows the flow of control passes from one activity to another. Once the functional requirements for the system and its boundaries is defined, user should examine the subject area with the aim of building class diagram. Further, it is useful to describe scenarios that is needed to be implemented in the application using sequence diagram. Scenarios can be described using chart cooperation, allowing to describe the interaction of objects and focuses primarily on the organization of the objects. State diagram determines the sequence of States of an object caused a sequence of events. This diagram may help to clarify the subject area, supplemented, if necessary, a class diagram. Chart deployment is a physical diagram in the UML. It displays the physical relationship between hardware and software components of the designed system.

* The problem statement for the design 
    - For example described problem Statement.

* Create entity relationship diagram
    - For example described entity relationship diagram.

* Charting activities
    - An example is to described diagram Construction chart activities.

* The construction of class diagrams
    - An example is to describe diagram classes.

## The Model menu of the application
In order to create a new class open the project. The default open menu item Application Model, which is a list of all classes in the project. Then you press the button Create class. 


## Sterotypes of classes 
+ Entities (implemtation) - This is the class that represent real object whose instaces will be stored in the appplication database. Create pair.
+ Enumeration (enumeration) - Is a datatype which is defined as an identifiers. Create pair.
+ Business server(businessserver) - This is a class whose code is invoked in the process of changing instances of related entities.
+ Type (type) – This is a complex data type or a real object whose instances will be stored in the application database. It is advisable to create, if necessary in code, secondary business objects that do not need to be stored in the database.
+ Typedef (typedef) - This is a type of data that can be mapped manually generated to the database or application data types. Needed if there are not enough default types.
+ Interface (interface) - This contract in the form of a list of public properties and methods that must be implemented in the related entities or types.
+ Application (application) - A class that stores general information about the generated application.
+ User forms (userform) – class representing an empty form of application (all markup and logic for it to be done fully manually by the developer), which can also be added to the menu structure (in “container” class with the stereotype “application”). It can be used in the case when the level of the application model required special forms, which are neither list nor edit forms (so that looking at the model it can be seen which forms are in the application)
+ Geo-server layer (geolayer) - Class which configures the layer GIS subsystem.
+ Geo-server layer styles (geolayerstyle) - class which configures the layer GIS subsystem.
+ External entities (external) – a class that is not explicitly declared in the model but will be available in the source code, including an entity from a different project. When generating code level, it is assumed that the declaration of this class is contained in an external or system library.  In a particular case, it is implied that you can specify for an external class a reference to a class from another project (stage) in Doxabeta Neo. In this particular case, it is assumed that the class at the code level is declared in another solution (addon), which must be connected by developers to the main project manually (for example, through a NuGet package created on the basis of another solution; the connection of "external" libraries at the generation level is not implied). When it is used: a reference to a class from other projects (i.e. stages) is indicated when there are some common libraries for several projects, and classes from it are reused in different projects. Another option is that the corresponding external class is a class from the system library or any external library (addon). Then, at the model level, it is possible to link to an external class and include it in the base class representation, and at the code level, after generation, the data type for the corresponding property will be the class that is declared in this "external" library (it must be connected manually by the developer to the project; if it is a class from a system assembly, for example, then it can already be automatically connected as an option at the first generation of the project).
+ Entities with user stereotypes with user-defined (custom) - class with arbitrary semantics, which it code is not generated to the application.

The list of diagrams contains automatically created diagrams for each class. In the search field on the Application Model form enter the name (or part of it) of the class from the list. Select the class (or several classes) that meets the specified condition displayed. In the All types field, select any of the created types. Only classes of the selcted type are displayed.

## Filtering and searching charts
The diagram menu contains all diagrams created within the project. They differ in types and have unique names. If the list is long, it is convenient to use search or filtering. To search for diagrams, you can type part of the diagram name in the search field. The list will be edited in accordance with the specified condition. You can also filter the diagram by type. For this drop down list, select the desired diagram type.