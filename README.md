# Circular-String-Linearization

## How to Run the project
`gcc project.c -o project` <br>
`./project {input_file} {output_file}`

Note that there are sample inputs in `tests/` that you can use to test the code.

## Project Details
This project considers the problem of finding the smallest lexicographic cyclic rotation in linear time. This achievied by implementing a Suffix Tree data structure, using the Ukkonen’s algorithm, with the given string repeated one time. So if String = "S" the Suffix Tree is built with "SS". Then we traverse the Suffix Tree by the smallest lexicographic rule until we reach a depth that equals the initial String "S" length.

## Input format
- First line contains an integer respective to the size of the target input string
- Then there is a single space character and then the characters of the target input string

## Output format
- A string Letter with the letter being processed
- A string Internal when an internal node is created
- A string Leaf when a leaf is created
- A string Final version which is followed by a representation of each node