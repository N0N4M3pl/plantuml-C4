# plantuml-C4

[PlantUML](https://plantuml.com/) is tool for creating diagrams using a simple and intuitive language.

[C4](https://c4model.com/) is model for visualising software architecture.

[plantuml-C4](https://github.com/N0N4M3pl/plantuml-C4) is library for creating C4 diagrams.

![Main example](/../master/example/contextView.png?raw=true)

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

- Header_Context
- System
- System_External

![Context example](/../master/example/contextView.png?raw=true)

### 2 - Container

- Header_Container
- Boundary_System
- Container
- Container_Script
- Container_Service
- Container_MicroService
- Container_Database
- Container_PubSub
- Container_Storage
- Application_Web_ServerSide
- Application_Web_ClientSide
- Application_Desktop
- Application_Mobile

![Container example](/../master/example/containerView.png?raw=true)

### 3 - Component

- Header_Component
- Boundary_Container
- Component
- Component_Database
- Component_Storage

![Component example](/../master/example/componentView.png?raw=true)

### 4 - Code

*not yet supported*

### Common - for all views

- Header
- Footer
- Boundary
- Person
- Relation