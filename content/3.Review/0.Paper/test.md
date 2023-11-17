---
title: Test paper
---

테스트 페이지 입니다.

## Example

{{< columns >}}
```tpl
{{</*/* mermaid [class="text-center"]*/*/>}}
stateDiagram-v2
    State1: The state with a note
    note right of State1
        Important information! You can write
        notes.
    end note
    State1 --> State2
    note left of State2 : This is the note to the left.
{{</*/* /mermaid */*/>}}
```

<--->

{{< mermaid >}}
stateDiagram-v2
    State1: The state with a note
    note right of State1
        Important information! You can write
        notes.
    end note
    State1 --> State2
    note left of State2 : This is the note to the left.
{{< /mermaid >}}

{{< /columns >}}
