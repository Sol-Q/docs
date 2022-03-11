## Activity Diagram
The activity diagram is like the state diagram. It reflects the dynamic aspects of the system behavior. Essentially, this diagram is a flowchart that clearly shows how the flow of control moves from one activity to another.

As an example, it is proposed to consider an enlarged activity diagram to describe the process of selling products to a client. This will allow you to better understand the actions taking place.
[Example](/Diagrams/Activity-diagram.png)

Activity on the chart are “scattered” on the treadmill, each of which corresponds to the behavior of one of the objects (e.g. client, Manager, web server, database server, etc.). It makes it easy to identify which object performs each of the activities. Lane - the area of the activity diagram, which shows only the activities under the responsibility of a specific object. The lane is designed to split the chart in accordance with the allocation of responsibility for actions. The title of lanes may indicate the role or object to which it corresponds. 

## The main elements of activities diagram
In the diagram of activities you can display the following elements of UML notation that are available in the Toolbox:

Element/Notation | Purpose
:------------------------------------------------------------------|:--------------------------------------------
![Example](/Diagrams/decision.jpg) | decision (Decision)
![Example](/Diagrams/activeobject1.jpg) | Active state (Active state)
![Example](/Diagrams/startstate.jpg) | Initial state (Start state)
![Example](/Diagrams/finalstate.jpg) | End state (Final state)
![Primer](/Diagrams/complextransition.jpg)![Primer](/Diagrams/complextransition_ver.jpg) | Synchronizer/splitter (Complex transition)
![Example](/Diagrams/objinstate.jpg) | Object in the state (in Object state)
![Primer](/Diagrams/signalreceipt-l.jpg)![Primer](/Diagrams/signalreceipt-r.jpg) | Receive signal (Signal receipt)
![Primer](/Diagrams/signalsend-l.jpg)![Primer](/Diagrams/signalsend-r.jpg) | Sending signal (sending Signal)
![Example](/Diagrams/transition.jpg) | Transition (Transition) (in Object state)
![Example](/Diagrams/objectflow.jpg) | Modify (object flow)
![Example](/Diagrams/partition.jpg) | Partition (Partition)
![Primer](/Diagrams/swlane-h.jpg)![Primer](/Diagrams/swlane-v.jpg) | Separator swimming lanes (Swimlane separator)
![Example](/Diagrams/note.jpg) | Comment (Note)
![Example](/Diagrams/noteconn.jpg) | Connector review (Note the connector)
