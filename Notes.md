# Theory of Computation

## Chapter1

- To show that L is regular, we need to find a DFA/NFA M that accepts L. There are two methods to do this:

1. Construct M directly.
2. Let L' = $\Sigma^*$ - L , find M' that accepts L'. Obtain M by exchanging the role of final and non-final states of M'.


## Chapter2
Pumping Theorem: L is regular language. There exists an integer $p \geq1$, for any  $\omega \in L$ and $|\omega|\geq p$, we can pick out a pattern y that can be repeated for arbituary times from $\omega$. (可以从属于regular language的字符串中抽出一个可重复任意多次的pattern y)。

Pumping theorem是regular language的必要条件。

Pumping theorem的证明：设p为L对应DFA的distinct states数。

Usage：可用Pumping theorem来证明non-regular

non-regular的证明还可以用closure property(与一个regular language做与操作等)



Context-free language(CFL): generate from context-free grammar(CFG) 

All regular languages are context-free language.

----------------------------------------------------------------------------------



CFG -> CFL <- PDA

Regular Expression -> Regular Language <- DFA/NFA



CFG: G = (V, $\Sigma$, R, S)

CFL: some CFG generates it.

Build a CFG: Try to observe the special case of CFL, |$\omega$|=0, |$\omega$|=1, ...

​	Then proof L = L(G), that is L $\subseteq$ L(G) and L(G) $\subseteq$ L.

Parse Tree: the path of a CFG generating a string.

- Internal nodes are non-terminals
- Leaves are e or terminals
- Edges form a string

Parse tree of a string is not unique. Example: a + a * a, we can make S -> S+S first, or S-> S*S first.

Ambiguous CFG: for $\omega \in L(G)$, there are two or more parse trees with roots S and yields $\omega$.

⭐We can change the Rules of CFG, to make it not ambiguous. (Make S -> S+S first only)

Inherently ambiguous CFL: every CFG that generates this language is ambiguous.



Proof that every Regular Language is Context-Free Language.

