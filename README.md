# Playing with UML Diagrams

## Class Diagram

Single block:

```
----------------------------
CLASS NAME
----------------------------

ATTRIBUTES
----------------------------


FUNCTIONS
----------------------------
```

Access Modifier or Class Visibility notations:

```bash
+ Public
- Private
# Protected
~ Package Local
```

Params in methods can be decribed in terms of its direction wrt to the caller:

```
MethodA(in a: int): int => takes in a, does not modify it
MethodB(out a: str): int => returns a after modification
MethodC(inout a: bool): str => takes in a, and modifies it
```

Class Diagrams can represent 3 different level of specification or perspective

> Conceptual Perspective:

>> Diagrams that represent concepts that implement the classes and is language independent

> Specification Perspective:

>> High level software specification, but not their implementation

> Implementation Perspective:

>> Depict actual software implementation


Relationship between classes

[Notations](https://en.wikipedia.org/wiki/Class_diagram#/media/File:Uml_classes_en.svg)

![class-relationship-connectors](https://user-images.githubusercontent.com/12943990/139782678-f07a5ac6-9e57-4e16-a5f2-85427e379d4a.png)

> Association:

- Connects classes
- Can specify verb describing association
- Muliplicity: number of obejcts taking part in the relationship. Eg: 1 to 1, 1 to many, many to many

> Inheretence/Genrealization:

- Schematic relationship between parent class and its descendants
- Hollow arrow directed towards parent class
- Convention: Abstract classes names are written in italics

> Realization:

- Relationship between interface and objects that implement this interface
- Special case of association of two classes

> Dependency:

- When object of one class is used by another class, without being stored in a field

> Aggregation:

- One class is a composite part of another
- If aggregate class deleted, the composite classes exist, but do not form the aggregate class

> Composition:

- Once the classes forming the aggregator class are dropped, the aggregator class is also dropped


