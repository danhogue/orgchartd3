Name for the Problem:
=====================
Rendering the Org chart

Description of the Problem:
=====================
Read in list of individuals and their managers (an org chart) from a CSV file, and output a file containing the
hierarchy in JSON format. Sound easy? Well it's not hard but here's an extra little kicker: Your algorithm must
be better than O(n^2). Meaning no nested loops.

To make things a bit more fun, once you can output the contacts.json file, fire up the node.js app in the folder and
go to http://localhost:3000 to see it rendered with d3!

Files can be downloaded from:

    https://github.com/chmod740/orgchartd3

Input
====
A CSV file containing a person's name together with their manager's name.

Output
=======
A JSON file containing the node names with child nodes as a tree structure.

Example
========
Input:

    "John", "Sally"
    "Anna", "Sally"
    "Sally",""

Output:

    {
        "node_name": "Sally",
        "children":  [
            {
                "node_name": "John",
                "children": []
            },
            {
                "node_name": "Anna",
                "children": []
            }
        ]
    }






