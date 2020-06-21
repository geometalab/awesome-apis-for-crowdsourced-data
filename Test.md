Regular **Markdown** here.

<!--
@startuml firstDiagram

Alice -> Bob: Hello
Bob -> Alice: Hi!
	
@enduml
-->

![](firstDiagram.svg)

Some more markdown.

@startuml firstDiagram

Alice -> Bob: Hello
Bob -> Alice: Hi!
	
@enduml

```dot
digraph L {

  node [shape=record fontname=Arial];

  a  [label="one\ltwo three\lfour five six seven\l"]
  b  [label="one\ntwo three\nfour five six seven"]
  c  [label="one\rtwo three\rfour five six seven\r"]

  a -> b -> c

}
```