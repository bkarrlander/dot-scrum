# dot-scrum
Scrum explained in DOT notation

### Scrum Theory

![What is Scrum?](https://g.gravizo.com/source/custom_mark?https%3A%2F%2Fraw.githubusercontent.com%2Fbkarrlander%2Fdot-scrum%2Fmaster%2FREADME.md)
<details> 
<summary></summary>
custom_mark
    digraph scrum_theory {
    
        node [shape=box];

        scrum -> process_framework [label="is a"];
        //custom_processes_and_techniques -> process_framework [label="can fit within"];

        scrum -> mgmt_of_complex_work [label="helps"];
        //scrum -> efficacy [label="makes\nclear"];

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

        // TEAM NODES;
        scrum_team -> selforg [label="is"];
        scrum_team -> increments [label="iteratively\ndelivers"];
        increments -> useful_version [label="ensures\navailability of"]
        scrum_team -> flexibility [label="designed to\noptimize"];
          
        
        // ;  
        // node labels;
        // ;
        scrum [label="Scrum"]
        scrum_team [label="The Scrum Team"];
        scrum_values [label="The Scrum Values"];
        process_framework [label="process framework"];
        pillars [label="3 pillars of Scrum"];
        empirical [label="empirical \nprocess control"];
        //custom_processes_and_techniques [label="custom processes \n& techniques"];
        //efficacy [label="efficacy of employed\nmanagement & techniques"];
        mgmt_of_complex_work [label="management of \ncomplex work"];
        iterative_approach [label="iterative & incremental\napproach"];
        
          // ;
          // TEAM LABELS;
          // ;
        selforg [label="self-organizing &\ncross-functional"];
          increments [label="feedback-based increments\nof \"Done\" product"];
        useful_version [label="potentially useful\nversion of product"];
        flexibility [label="flexibility,\ncreativity &\nproductivity"];
          
                   
        // ;  
        // Layout;
        // ;
        { rank=same; scrum process_framework scrum_team }
        { rank=same; pillars scrum_values }
    }
custom_mark
</details>

### Visualization
```<img src='https://g.gravizo.com/svg? digraph g { a -> b }'/>```

NOTE: Ending comments with semi-colon otherwise the graph gets messed up by g.gravizo.com
