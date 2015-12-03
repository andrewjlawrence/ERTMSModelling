The following 3 error scenarios give the expected counter examples.

Scenario 1: Incorrect Control Tables.
-------------------------------------
Remove AC from the Control table completely.
 -- Remove from clear tracks of route 1A.
 -- Remove as a release point and replace with AB.


Scenario 1B: Incorrect Release of Point.
--------------------------------


Scenario 1C: Incorrect Setting of Point.
--------------------------------


Scenario 2: Incorrect RBC Tables.
-------------------------------------
Give Out MA that is too long.
 -- Changed EoA table for route 1A to allo trains to over-shoot onto AD.
 -- Also changed controller so that it does not request route 2,
   meaning that the first train stops on AD, otherwise train speeds
   happen to make the system safe :)



Scenario 3: Incorrect Braking Distance.
-------------------------------------
Modelling incorrect parameters on train weight.
 -- Changed braking distance calculation to be:
(((S * S) + S) div 2) monus 400.
 -- Again also had to change controller not to request route 2, for
    same reasons as scenario 2.
