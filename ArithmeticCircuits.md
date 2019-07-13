# From Computations to Polynomials

![By-V](https://miro.medium.com/max/1188/1*YD-ckgBfmmmRBCyVlhp8YQ.png)

> by Vitalik Buterin[1]

...

The steps here can be broken up into two halves.

* First, zk-SNARKs cannot be applied to any computational problem directly;
rather, you have to convert the problem into the right “form” for the problem to operate on.
The form is called a “quadratic arithmetic program” (QAP),
and transforming the code of a function into one of these is itself highly nontrivial.
Along with the process for converting the code of a function into a QAP is another process
that can be run alongside so that if you have an input to the code you can create a corresponding solution
(sometimes called “witness” to the QAP).

* After this, there is another fairly intricate process for creating the actual “zero knowledge proof” for this witness,
and a separate process for verifying a proof that someone else passes along to you,
but these are details that are out of scope for this post.

...

# References

[1] https://medium.com/@VitalikButerin/quadratic-arithmetic-programs-from-zero-to-hero-f6d558cea649   
[2] https://electriccoin.co/blog/snark-explain5/   
