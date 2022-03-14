## Key concepts
The data structure defines the structure of the application. The systems are based on a data structure expressed by a UML class diagram.

Let's consider the basic concepts based on elementary UML concepts on the example of a class diagram (the concepts of attribute, method, method parameter, type, association role, etc. are not considered, since they are obvious and are entirely borrowed from UML). This [class diagram](fd_class-diagram.html) also illustrates typical situations that arise during design. Any other situations are consequences of this diagram.

![](/Diagrams/examples/uml-example1.jpg) 

The class with respect to which associations are considered in a particular situation is called an internal class, and the rest are external.
By attachment (subobject) is an attribute of a class whose type is another class.

## Master Association

Association similar to the Association between Internal and Master1 called the mechanics, and the outer class from the multiplicity 1 or 0..1 is called Master. A master association can be carried out between classes, each of which is a child, and they have a common cap. An example of this is the Detail2-Detail3 association

## Child compositions, aggregator, header
Aggregation associations or aggregations - compositions similar to Internal-Detail1 are called child, and the external class is child, or simply childish. The inner class in relation to the child is also called an aggregator or header

## Inheritance
Inheritance associations like Internal-InternalChild are called inheritance, the inner class in such an association is the ancestor, and the outer one is the descendant.

## Stereotypes
Classes on the class diagram, the stereotypes attributed to that allows you to specify the appointment of an UML class.

In Doxabeta Neo the following are predefined stereotypes:

* Implementation, the stereotype of default (the chart specify an empty value), the usual UML class implemented in the source code of classes of data objects. Classes can be linked by any associations.
* TypeDef, a stereotype indicating the type of synonym. When generating code synonyms are given to basic types in the target language by the user (the base type gets into the code, but the synonym is not specified in any way)). The diagrams cannot be linked by any associations. 
* Type, a stereotype introducing a new type. When generating code in the target language, this type is declared, and when declaring class members, parameters, etc., it is used. 
* Enumeration,a stereotype introducing an enumerated type. The diagrams cannot be linked by any associations.
* Interface, a stereotype that introduces .Net interface. Interfaces can be linked by any associations.
* BusinessServer, the stereotype corresponding to the business server is .Net class, where the implementation of the business operations of the application system is located;
* EditForm, the stereotype corresponding to the editing form is .Net to the class where the implementation of the form for editing the data object is located;
* ListForm,the stereotype corresponding to the form of the list is .Net to the class where the implementation of the form for displaying a list of data objects is located;
* PrintForm, a stereotype corresponding to the form of printing — .Net class where the implementation of the form for printing is located;
* UserForm, a stereotype corresponding to an empty form;
* EventArg, the stereotype corresponding to the event parameters (event), when generated, the resulting class is inherited from System.EventArgs;
* Application, the stereotype corresponding to the application: the shape of the desktop and the setup class;
* Role, the stereotype corresponding to the role in the system of powers;
* External, a stereotype corresponding to any external (not declared in CASE, language) class.
* ExternalInterface, a stereotype corresponding to any external (undeclared) interface
* User, the user can specify an arbitrary stereotype

## Non-obvious limitations of the object structure (how not to do)
The UML notation describes the purpose of its elements, but does not declare in any way the "correctness" of their use. Therefore, let's consider the main non-obvious limitations that are not described by the notation, cause difficulties in understanding, are impossible to implement, and should be **avoided**

## Cyclic Details
Children of any level cannot be the heir of the cap, because in this case it turns out that the object of the heir must include itself.
![](/Diagrams/examples/uml-example2.jpg) 


## Contradictory aggregation
The heir from the child cannot be the child of the heir of the hat.
![](/Diagrams/examples/uml-example3.png) 

## However
Such a situation is possible:

![](/Diagrams/examples/lookup-as-master.png) 
