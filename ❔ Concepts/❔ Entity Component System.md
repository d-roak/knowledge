https://github.com/bevyengine/bevy/blob/main/examples/ecs/ecs_guide.rs

Why ECS?
* Data oriented: Functionality is driven by data
* Clean Architecture: Loose coupling of functionality / prevents deeply nested [Inheritance](Knowledge/❔%20Concepts/❔%20Programming/❔%20Object-Oriented%20Programming.md#Inheritance)
* High Performance: Massively parallel and cache friendly

ECS Definitions:

Component: just a normal Rust data type. generally scoped to a single piece of functionality
    Examples: position, velocity, health, color, name

Entity: a collection of components with a unique id
    Examples: Entity1 { Name("Alice"), Position(0, 0) },
              Entity2 { Name("Bill"), Position(10, 5) }

Resource: a shared global piece of data
    Examples: asset storage, events, system state

System: runs logic on entities, components, and resources
    Examples: move system, damage system
