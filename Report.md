Assignment 6 Solution
---------------------

# Team Members

- Joey Lau
- Lorena Raichle

# GitHub link to your (forked) repository

https://github.com/LorenaRaichle/Assignment6

# Task 1

1. WebIDs of the group members

Ans:
https://solid.interactions.ics.unisg.ch/LorenaRaichle/profile/card#me
https://solid.interactions.ics.unisg.ch/Joey-Lau/profile/card#me


2. Group profile

Ans: https://solid.interactions.unisg.ch/LorenaRaichle/TeamJoeyLorena


# Task 2

1. What command did you perform to get the group name from the WebId?

Ans:

'SELECT ?group WHERE { ?group foaf:member <https://solid.interactions.ics.unisg.ch/TeamJoeyLorena/profile/card#me> . }'



2. Which command did you perform to get the group members from the WebId?

Ans:

PREFIX foaf: <http://xmlns.com/foaf/0.1/>
SELECT ?memberName
WHERE {
<https://solid.interactions.ics.unisg.ch/TeamJoeyLorena/sample-team> foaf:member ?member .
?member foaf:name ?memberName .
}


[
{"memberName":"\"LorenaRaichle\""}
]


SELECT ?memberName WHERE { ?s ?p ?memberName }

[
{"memberName":"http://xmlns.com/foaf/0.1/Group"},
{"memberName":"https://solid.interactions.ics.unisg.ch/LorenaRaichle/profile/card#me"},
{"memberName":"https://solid.interactions.ics.unisg.ch/Joey-Lau/profile/card#me"},
]


3. Which command did you performed to get the group members from the WebId without link traversal? Which result did you get? Is it correct?

Ans:


