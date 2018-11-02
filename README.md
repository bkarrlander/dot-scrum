# dot-scrum
Scrum explained in DOT notation

### What is Scrum?

![What is Scrum?](https://g.gravizo.com/source/custom_mark?https%3A%2F%2Fraw.githubusercontent.com%2Fbkarrlander%2Fdot-scrum%2Fmaster%2FREADME.md)
<details> 
<summary></summary>
custom_mark
    digraph what_is_scrum {
    
        node [shape=box];

        scrum -> process_framework [label="is a"];
        custom_processes_and_techniques -> process_framework [label="can fit within"];

        scrum -> mgmt_of_complex_work [label="helps"];
        scrum -> efficacy [label="makes\nclear"];

        scrum -> iterative_approach [label="employs an"];
        iterative_approach -> predictability [label="optimizes"]; 
        iterative_approach -> risk [label="minimizes"]; 
        iterative_approach -> feedback [label="maximizes\nopportunity\nfor"]; 

        scrum -> empirical [label="founded on\ntheory of"];
        empirical -> pillars [label="upheld by"];
        pillars -> transparency;
        pillars -> inspection;
        pillars -> adaption;
        pillars -> scrum_values [label="come to\nlife by"];
        scrum_team -> scrum_values [label="lives by"];

        // node labels;
        scrum [label="Scrum"]
        scrum_team [label="Scrum Teams"];
        scrum_values [label="Scrum Values"];
        process_framework [label="process framework"];
        pillars [label="3 pillars of Scrum"];
        empirical [label="empirical \nprocess control"];
        custom_processes_and_techniques [label="custom processes \n& techniques"];
        efficacy [label="efficacy of employed\nmanagement & techniques"];
        mgmt_of_complex_work [label="management of \ncomplex work"];
        iterative_approach [label="iterative & incremental\napproach"];
        
        // layout;
        { rank=same; scrum process_framework }
        { rank=same; pillars scrum_values }
    }
custom_mark
</details>

### Visualization
```<img src='https://g.gravizo.com/svg? digraph g { a -> b }'/>```

NOTE: Ending comments with semi-colon otherwise the graph gets messed up by g.gravizo.com
