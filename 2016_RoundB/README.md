SherlockAndParentheses.py: The topology ()()()(.. generates the maximum answer. Let the number of (s be A, let the number of )s be B, let P be min(A,B), we first state that the maximum number of balanced groups will not be more than P*(P+1)/2. Proof: without loss of generality, asssume A<=B. For the i th ( in the arrangement, we know there are at most A-i (s that come after it, thus the maximum number of balanced group that starts from the i th (, is (A-i)\*(A-i+1)/2. Summing up the value for each (, we know the total bound is A\*(A+1)/2, when A<B. Meanwhile, we know this bound is achievable because we can construct it with the topology ()()()(...