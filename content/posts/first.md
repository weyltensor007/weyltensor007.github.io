+++
title = 'First'
date = 2024-08-19T14:33:47+08:00
tags = ["first_tag"]
series = ["first_series"]
categories = ["first_cats"]
+++


Hello, this is some code block

```python
print("hello world!")
```


```mermaid
stateDiagram
    direction LR
    [*] --> A
    A --> B
    B --> C
    state B {
      direction LR
      a --> b
    }
    B --> D
```


```mermaid
---
title: Centered Mermaid Diagram
config:
  theme: dark
  flowchart:
    curve: linear
---
flowchart
    A --> B
    B --> C
```