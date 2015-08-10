People Networks
----------

### To do:
- #def moveEvent(event, newBranch, authorSignature):
- check that msg.sender is one of our function contracts
- investigate https://www.seas.upenn.edu/~hoda/HLPV.pdf
- consider implications of updating data/api contracts & data migration

### Bugs:
- https://github.com/ethereum/wiki/wiki/HPOC_2015#anti-pre-revelation

### Scalability optimizations:
- randomized voter selection? - first x events expiring vote on in one ballot - random selection, then another ballot (V presentation on a similar strat.) - req. rep sort
- ethereum rng:
  - probability 0 1 ... 100
  - prob = probability*2^32
  - if(sha(block.prevhash+block.coinbase+block.timestamp+nonce) mod 2^32<prob):
	   	you got picked / won the rng!
- max number of owners in a branch of rep. issues w/ sending rep etc
- zeroing of array values (e.g. people in the rep index after they have 0 rep left)
- consensus bond mechanism cheaper + reporting on outcome + if not certain onchain as fallback
- possibly enable people to choose their own resolution scripts
- metadata off chain
- https://github.com/ethereum/wiki/wiki/Problems#3-arbitrary-proof-of-computation (to 11)
- reporting / consensus scaling