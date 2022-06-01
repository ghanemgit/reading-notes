# GraphQL @connection

## Relationships
#### Without relationships, your type definitions are simply a collection of disconnected nodes, with little value. Adding relationships into your data model gives your data the context that it needs to run complex queries across wide sections of your graph. This section will run through writing some type definitions for a simple connected model, inserting some data through the schema, and then querying it.

### Example graph
#### The following graph will be used in this example, where a Person type has two different relationship types which can connect it to a Movie type.
![image](https://user-images.githubusercontent.com/97638932/168908636-197841dc-81df-4f8c-9cdd-faf1f02d46d8.png)

Figure 1. Example graph

### Type definitions
First, to define the nodes, you should define the two distinct types in this model:


```
type Person {
    name: String!
    born: Int!
}
type Movie {
    title: String!
    released: Int!
}
```
#### You can then connect these two types together using @relationship directives:

```
type Person {
    name: String!
    born: Int!
    actedInMovies: [Movie!]! @relationship(type: "ACTED_IN", direction: OUT)
    directedMovies: [Movie!]! @relationship(type: "DIRECTED", direction: OUT)
}

type Movie {
    title: String!
    released: Int!
    actors: [Person!]! @relationship(type: "ACTED_IN", direction: IN)
    director: Person! @relationship(type: "DIRECTED", direction: IN)
}
```
#### The following should be noted about the fields you just added:

- A Person can act in or direct multiple movies, and a Movie can have multiple actors. However, it is exceedingly rare for a Movie to have more than one director, and you can model this cardinality in your type definitions, to ensure accuracy of your data.

- A Movie isn’t really a Movie without a director, and this has been signified by marking the director field as non-nullable, meaning that a Movie must have a DIRECTED relationship coming into it.

- To figure out whether the direction argument of the @relationship directive should be IN or OUT, visualise your relationships like in the diagram above, and model out the direction of the arrows.

- The @relationship directive is a reference to Neo4j relationships, whereas in the schema, the phrase edge(s) is used to be consistent with the general API language used by Relay.
