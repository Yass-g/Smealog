# Smealog
An interesting, theory-based, cryptography challenge featured in the FCSC 2021 CTF (French cybersecurity challenge), where the aim was to compute the discrete logarithm with an elliptic curve over a ring. Being more in the theoritical side of cryptography, it had few solves during the challenge, so I'm sharing a solution I came up with during the event.

Smealog.sage and output.txt are the two files provided by the challenge.

The main insight was to transition the problem towards the p-adic field Qp, with finite precision (4 in this case). Once over Qp, we use a result establishing an isomorphism between p-adic integers of absolute value lesser than one, pZp, and E1(Qp), the set of points whose reduced forms are the point at infinity.

For more details : https://core.ac.uk/download/pdf/147902645.pdf
        
            
