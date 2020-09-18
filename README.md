# Task
This file creates a result from tasks based on dependencies.

you need to enter text values as below:
Enter tasks as a string
Enter dependencies as a string

EXAMPLES

tasks : []
dependencies: []
result: []

tasks: [a,b]
dependencies: []
result: [a,b]

tasks: [a,b]
dependencies: [a => b]
result: [b,a]

tasks: [a,b,c,d]
dependencies: [a => b,c => d]
result: [b,a,d,c]

tasks: [a,b,c]
dependencies: [a => b,b => c]
result: [c,b,a]

tasks: [a,b,c,d]
dependencies: [a => b,b => c,c => a]
result: Error - this is a cyclic dependency


function that does the job:
items_as_per_order(tasks,dependencies)
