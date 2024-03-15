
Anonymous credentials: attributes vs functions



We discuss the privacy and policy implications for some different reusable anonymous credential technologies.

Attribute based anonymous credentials like "I Reveal My Attributes" (IRMA) received considerable press over the recent years.  In these, users reveal requested parts of an identity document, like gender, without revealing other parts.  IRMA also permits proving diverse attributes from multiple linked credentials. 

As discussed by the W3C verifiable claims WG, attribute based credentials use-cases risk abuse or unnecessary disclosure of personal information.  At one extreme, services might collect unnecessary attributes merely to prevent sock puppets, Sybil attacks, etc.  We think this risks becoming the typical use case even.

Anonymous credentials could handle this typical use case better by never revealing any personal information, but instead proving the output of a secret pseudo-random function tied to the user.  An example is proof-of-person-hood parties by Bryan Ford's DEDIS group at EPFL

We discuss both applications like rate limiting, spam defense, and games, as well as strategies for authenticating function inputs so services only know their users represent distinct people, but cannot link users between services.

We also discuss the differences between basing a credential upon an anonymized certificate scheme or upon a ring signature.


I'll briefly cover a mathematical trick which I discussed in https://www.youtube.com/watch?v=0i_5RW3tkVM&list=PLj80z0cJm8QFnY6VLVa84nr-21DNvjWH7&index=9 but overall keep the talk not too technical. 

