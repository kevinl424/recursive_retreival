# Recursive Retrieval Cyphers

## Getting Subraph Based on Entity ID
    MATCH p = (:Entity { id: "Harry" })-[*]->()
    RETURN p;

- the  `*` means traversing all paths
- adding a number, `x`, after `*` means a max hop distance of only that many nodes 
- can search labels by replacing `Entity` with labels