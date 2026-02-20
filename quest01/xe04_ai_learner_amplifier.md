Phase 1: Build Foundation (you first)

1. Active reading, self-explanation (close the doc), simple scenario design (5–10 devices) with your justification.


   Scenario: Smart Campus Emergency Network

   (Laptop A)
        |
   (Phone B)
        |
   (Tablet C) ---- (Laptop D)
        |
   (Sensor E)
        |
   (Phone F)
        |
   (Server G)


Devices:

Laptop A = Student laptop

Phone B = Student phone

Tablet C = Campus control tablet (central node)

Laptop D = Lecturer laptop (side node)

Sensor E = Security sensor

Phone F = Security officer phone

Server G = Campus emergency server

All devices communicate wirelessly (no fixed cables).


This is a wireless network of 7 devices where each device can forward data. Laptop A cannot reach Server G directly, so it sends data through intermediate sevices like Phone B, Tablet C, Sensor E, and Phone F.

Laptop A sends an emergency report to Server G.
A connect to B
B connect to C
C sees two options:
Path 1: C → D (Laptop D)
Path 2: C → E 
Routing protocol chooses the path that actually leads to the destination.
Since Laptop D does NOT lead to Server G directly,
C connect to E
E connect to F
F connect to G

A → B → C → E → F → G

My Justification:
Using & devices is ideal because is not too small or too complex to understand and learn.


Phase 2: Strategic AI Use

Test your understanding, explore edge cases with targeted questions, then validate.

Edge case 1: What if Tablet C fails?
scenario: Tablet C suddenly turns Off
New topology:
A → B __ E → F → G

      (C is dead)
Result:
communication breaks because there is no alternative path frome B to E.
Validation: Tablet C is a critical node (single poiunt of failure)

Edge Case 2: What if Sensor E fails?
A → B → C ---- D
              X

              E (offline)
              |
              F → G
can the routing protocol find another path?
if laptop D has a route to F or G then network reroutes through D else data cannot reach G.
validation concept: Tests network reduncy (backup paths)


Edge case 3: what if laptop D become closer to server G?
Scenario: Suppose Laptop D connects directly to server G:
A → B → C → D → G  (shorter path!)

Validation: Routing protocols always choose the optimal path.


Edge Case 4: What If Phone B Moves Out of Range?

New topology:
A   X   B → C → E → F → G
Laptop A becomes isolated.

Result:
A cannot send data to the network
Even though the rest of the network works

Validation Concept: This demonstrates connectivity dependency in wireless networks.



Phase 3: Real Application

Design a small smart-city network (1,000 IoT sensors, 50 traffic lights, 10 emergency vehicles). Decide protocols, justify choices, list failure points, then refine with AI feedback.

