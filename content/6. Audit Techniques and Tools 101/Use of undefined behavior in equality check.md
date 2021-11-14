
# 55 - [Use of undefined behavior in equality check](./Use%20of%20undefined%20behavior%20in%20equality%20check.md)

 On the left-hand side of the equality check, there is an assignment of the variable `outputAmt`_. The right-hand side uses the same variable. The Solidity 0.7.3. documentation states that “The evaluation order of expressions is not specified (more formally, the order in which the children of one node in the expression tree are evaluated is not specified, but they are of course evaluated before the node itself). It is only guaranteed that statements are executed in order and short-circuiting for boolean expressions is done” which means that this check constitutes an instance of undefined behavior. As such, the behavior of this code is not specified and could change in a future release of Solidity.


___
## Slide Screenshot
![055.png](../../images/6.Audit%20Techniques%20and%20Tools%20101/055.png)
___
## Slide Text
- 
___
## References
- Youtube Reference
___
## Tags