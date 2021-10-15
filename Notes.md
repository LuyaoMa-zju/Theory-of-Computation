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

