# dot-scrum
Scrum explained in DOT notation

### Scrum Theory

![Scrum Theory](https://g.gravizo.com/source/scrum_theory_mark?https%3A%2F%2Fraw.githubusercontent.com%2Fbkarrlander%2Fdot-scrum%2Fmaster%2FREADME.md)
<details> 
<summary></summary>
scrum_theory_mark
    digraph scrum_theory {
    
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
        pillars -> adaptation;
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
        custom_processes_and_techniques [label="custom processes \n& techniques"];
        efficacy [label="efficacy of employed\nmanagement & techniques"];
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
scrum_theory_mark
</details>

### The Scrum Team

![The Scrum Team](https://g.gravizo.com/source/scrum_team_mark?https%3A%2F%2Fraw.githubusercontent.com%2Fbkarrlander%2Fdot-scrum%2Fmaster%2FREADME.md)
<details> 
<summary></summary>
scrum_team_mark
    digraph scrum_team {
    
    node [shape=box];

    // nodes; 
    
    scrum_team -> product_owner;
    scrum_team -> dev_team;
    scrum_team -> scrum_master;
    
    product_owner -> work_items [label="prioritizes"];
    dev_team -> work_items [label="delivers\n\"Done\""];
    
    dev_team -> work [label="says \"how\" \n& \"how much\""]
        
    product_owner -> business_value [label="maximizes"];
    work_items -> business_value [label="deliver"]
    
    scrum_master -> scrum [label="promotes & provides\nsupport for"];

    // node labels;
    scrum [label="Scrum"];
    scrum_master [label="Scrum Master"]
    product_owner [label="Product Owner"]
    dev_team [label="Dev Team"]
    scrum_team [label="The Scrum Team"]
    work_items [label="work items"]
    business_value [label="business value"]
    
    // layout;
    //{ rank=same; business_value work_items scrum }
    }
scrum_team_mark
</details>

### Graph visualization
```<img src='https://g.gravizo.com/svg? digraph g { a -> b }'/>```

NOTE: Ending comments with semi-colon otherwise the graph gets messed up by g.gravizo.com
