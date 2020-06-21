Regular **Markdown** here.

First diagramm as PlantUML:
<!--
@startuml firstDiagram

Alice -> Bob: Hello
Bob -> Alice: Hi!
	
@enduml
-->

![](firstDiagram.svg)

Some more markdown.

Second diagram as GraphViz:
<!--
```dot
digraph L {

  node [shape=record fontname=Arial];

  a  [label="one\ltwo three\lfour five six seven\l"]
  b  [label="one\ntwo three\nfour five six seven"]
  c  [label="one\rtwo three\rfour five six seven\r"]

  a -> b -> c

}
```

![](secondDiagram.svg)

```graphviz
digraph hierarchy {

                nodesep=1.0 // increases the separation between nodes

                node [color=Red,fontname=Courier,shape=box] //All nodes will this shape and colour
                edge [color=Blue, style=dashed] //All the lines look like this

                Headteacher->{Deputy1 Deputy2 BusinessManager}
                Deputy1->{Teacher1 Teacher2}
                BusinessManager->ITManager
                {rank=same;ITManager Teacher1 Teacher2}  // Put them on the same level
}
```
