## Features of building a class diagram

* The elements used to build class diagrams, described on page class Diagram (Class diagram).
* Working with the editor of class diagrams is given in relevant article

## Features of building classes
![](/Diagrams/structure-of-class.png) 

The General structure of the class is shown in the figure above.

* Renaming classes is presented in Features of the editor class diagram (why this should be done exactly the way explained in this article).
* Used stereotypes with the description given in the article Key concepts of object-oriented structure for applications developed on the Platform Flexberry](fd_key-concepts.html).
* Features of the job methods classes presented in the article class Methods and method parameters .
* Description of class attributes is presented in Attributes data classes .

The need to pay special attention to:

* All names (classes and attributes) are written without spaces. If you want to present in behalf of several words, the words are written together, each with a letter (a description of this style are given here).
* Types that you can use, you can look at card types

## Recommendations for drawing class diagrams
There are recommendations for drawing a class diagram:

* The direction of the relationship 
    * Master associations are drawn "sideways". 
    * Children's compositions are drawn "down".
    * Inheritance is drawn "up” 


* Link Naming 
    * The name of the master is usually the same as the name of the class.
    * The name of the child (the name that the collection will bear in the object model) is usually plural.
    * Associations of the association type must be named on the part of the master, the composition type - on both sides.

* Connection Parameters
    * Classes united by a connection with a multiplicity of "1:1” are combined into one class.
    * Aggregation type relationships are replaced by either Association or Composition




