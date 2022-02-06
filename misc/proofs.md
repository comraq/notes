# Notes on Proofs
1. some difficult definitions have complex structures
  * proving these definitions can be confusing in terms of what can be assumed, and what needs to be actually proven
  * ex: "If a transitive group $G$ is primitive on $A$, prove for each $a\in A$, the only subgroups of $G$ containing $G_a$ are $G_a$ and $G$ (i.e., $G_a$ is a maximal subgroup of $G$)
    * tip:
      * to show a group is primitive, construct a block and show that the block is trivial
      * images of blocks are usually disjoint (ie: partitions) and hence examples of blocks could be cosets (where group elements of the same coset stabilizes the block)
1. work backwards from the desired result:
  * when asked to prove some result, sometimes exploring the result may express it differently, helping to identify which path to take when proving. Sometimes this can help with proof by contraposition as well
1. DFS vs BFS analogy
  * BFS (Breadth First Search) - iterating over all possible paths and slowly diving into each one
  * DFS (Depth First Search) - searching until the end of a path before iterating on the next
  * With proofs, DFS can often shed light faster for the outline of a proof. This is because non-trivial proofs require non-trivial steps to make progress, a BFS approach will appear to be "spinning in circles", never making any significant development in any path, resulting in lack of progress.
  * Whereas with DFS, even if it is a dead end, the depth at which the path is explored may illuminate "adjacent paths" (similar approaches), which may ultimately lead to proving the result. It is difficult to see the correct paths forward without taking a DFS approach.
1. explicitly write down definitions given to help mentally discover what the definitions mean and imply
1. regardless of what to prove, if direct proof does not lead to obvious results, try proving by contradiction
  * even if the proof just involves algebraic manipulation
1. Universal quantifier, `forall`
  * when given a clause with universal quantification in the assumptions, it may be helpful to think of `forall` as a helper function in programming
    * we can invoke a helper function in programming with any input we choose to obtain some result from that input
    * similarily, we can choose any value for the variable scoped by the universal quantifier to give us the desired result
    * this is similar to the concept of pi-types in homotopy type theory
