# plantuml-C4

[PlantUML](https://plantuml.com/) is tool for creating diagrams using a simple and intuitive language.

[C4](https://c4model.com/) is model for visualising software architecture.

[plantuml-C4](https://github.com/N0N4M3pl/plantuml-C4) is library for creating C4 diagrams.

![Main example](/../master/example/diagrams/example.container.png?raw=true)

## Getting Started

Depending on what diagram you build, you need to include specified file:
* [C4-Context.puml](https://raw.githubusercontent.com/N0N4M3pl/plantuml-C4/master/src/C4-Context.puml)
* [C4-Container.puml](https://raw.githubusercontent.com/N0N4M3pl/plantuml-C4/master/src/C4-Container.puml)
* [C4-Component.puml](https://raw.githubusercontent.com/N0N4M3pl/plantuml-C4/master/src/C4-Component.puml)
* C4-Code.puml (not yet supported)

If you need, you can use many of them in one file (you can mix them together).
Its depend what you want to show on diagram.

### Example:

Local file:
`!include /src/C4-Context.puml`

Remote file:
`!include https://raw.githubusercontent.com/N0N4M3pl/plantuml-C4/master/src/C4-Context.puml`

## Elements

### 1 - Context

- Header_Context(text)
- Footer_Context()
- System(alias, label, description=" ", link="")
- System_External(alias, label, description=" ", link="")

![Context example](/../master/example/diagrams/example.context.png?raw=true)

### 2 - Container

- Header_Container(text, link)
- Footer_Container()
- System_Boundary(alias, label)
- System_Package(alias, label)
- Container(alias, label, description=" ", technology="", link="")
- Container_Script(alias, label, description=" ", technology="", link="")
- Container_Service(alias, label, description=" ", technology="", link="")
- Container_MicroService(alias, label, description=" ", technology="", link="")
- Container_PubSub(alias, label, description=" ", technology="", link="")
- Container_Database(alias, label, description=" ", technology="", link="")
- Container_Storage(alias, label, description=" ", technology="", link="")
- Container_Config(alias, label, description=" ", technology="", link="")
- Application_WebServer(alias, label, description=" ", technology="", link="")
- Application_Web(alias, label, description=" ", technology="", link="")
- Application_Desktop(alias, label, description=" ", technology="", link="")
- Application_Mobile(alias, label, description=" ", technology="", link="")

![Container example](/../master/example/diagrams/example.container.png?raw=true)

### 3 - Component

- Header_Component(text, link)
- Container_Boundary(alias, label)
- Container_Package(alias, label)
- Component(alias, label, description=" ", technology="", link="")
- Component_PubSub(alias, label, description=" ", technology="", link="")
- Component_Database(alias, label, description=" ", technology="", link="")
- Component_Storage(alias, label, description=" ", technology="", link="")
- Component_Config(alias, label, description=" ", technology="", link="")

![Component example](/../master/example/diagrams/example.component.png?raw=true)

### 4 - Code

*not yet supported*

### Common - for all views

- Header(text)
- Footer()
- Note(alias, text, side="right")
- Person(alias, label, description=" ")
- Relation(fromAlias, toAlias, direction="--", label="")
