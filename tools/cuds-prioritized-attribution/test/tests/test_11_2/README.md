Testcase: 11.2
Criteria: More purchases than CUDs
Note: (L*) means a label set. Note that "project-1: (L1)" does not mean its a project label. 
Its a user label that is attached to a vm thats part of project-1
========


|----COMMITMENTS--|----------BILLING EXPORT-----------------------|----------------------BILLING OUTPUT-----------------------------|
|     Purchases   |     Usage          |BA level|BA level|BA level| Expected CUD      |  Expected SUD        |Expected COST         |
| Projects |Amount|                    |  CUD   |  SUD   | COST   |  allocation       |   allocation         | allocation           |
| ---------|----- |--------------------|-----------------|--------|-------------------|----------------------|----------------------|
|T1:Project-1,    |Project-1(L1):50    |   60  |  100    |  100   |Project-1(L1):5    |Project-1(L1):13.23   |Project-1(L1):8.33    |
|   Project-2:100 |Project-1(L1,L2):50 |                          |Project-1(L1,L2):5 |Project-1(L1,L2):13.23|Project-1(L1,L2):8.33 |
|                 |                    |                          |                   |                      |                      |
|T2:Project-3: 50 |Project-2(L2):100   |                          |Project-2(L2):10   |Project-2(L2):26.47   |Project-2(L2):16.66   |
|                 |Project-2(L1,L2):100|                          |Project-2(L1,L2):10|Project-2(L1,L2):26.47|Project-2(L1,L2):16.66|
|                 |                    |                          |                   |                      |                      |
|                 |Project-3(L2):100   |                          |Project-3(L2):30   |Project-3(L2):20.58   |Project-3(L2):50      |    
|-----------------------------------------------------------------------------------------------------------------------------------|

