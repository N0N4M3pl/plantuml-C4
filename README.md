# plantuml-C4

[PlantUML](https://plantuml.com/) is tool for creating diagrams using a simple and intuitive language.

[C4](https://c4model.com/) is model for visualising software architecture.

[plantuml-C4](https://github.com/N0N4M3pl/plantuml-C4) is library for creating C4 diagrams.

![Main example](https://github.com/N0N4M3pl/plantuml-C4/example/contextView/main.png)

## Getting Started

Depending on what diagram you build, you need to include specified file:
* [C4-Context.puml](https://github.com/N0N4M3pl/plantuml-C4/src/C4-Context.puml)
* [C4-Container.puml](https://github.com/N0N4M3pl/plantuml-C4/src/C4-Container.puml)
* [C4-Component.puml](https://github.com/N0N4M3pl/plantuml-C4/src/C4-Component.puml)
* C4-Code.puml (not yet supported)

### Example:

Local file:
`!include /src/C4-Context.puml`

Remote file:
`!include https://github.com/N0N4M3pl/plantuml-C4/src/C4-Context.puml`

## Elements

### 1 - Context

- System
- System_External

### 2 - Container

- Boundary_System
- Container

### 3 - Component

- Boundary_Container
- Component
- Component_Service
- Component_Database
- Component_PubSub
- Component_Storage
- Component_Script
- Component_App_Desktop
- Component_App_Web
- Component_App_Mobile

### Common - for all views

- Boundary
- Person
- Relation
