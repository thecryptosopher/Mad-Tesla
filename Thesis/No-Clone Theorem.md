## Quantum Bitcoin: An Anonymous and Distributed Currency
Secured by the No-Cloning Theorem of Quantum Mechanics

The digital currency Bitcoin has had remarkable growth since it was first proposed in
2008. Its distributed nature allows currency transactions without a central authority by
using cryptographic methods and a data structure called the blockchain. 

In this paper we
use the no-cloning theorem of quantum mechanics to introduce Quantum Bitcoin, a Bitcoinlike currency that runs on a quantum computer. We show that our construction of quantum
shards and two blockchains allows untrusted peers to mint quantum money without risking
the integrity of the currency. The Quantum Bitcoin protocol has several advantages over
classical Bitcoin, including immediate local verification of transactions. 

This is a major
improvement since we no longer need the computationally intensive and time-consuming
method Bitcoin uses to record all transactions in the blockchain. Instead, Quantum Bitcoin
only records newly minted currency which drastically reduces the footprint and increases
efficiency. We present formal security proofs for counterfeiting resistance and show that
a quantum bitcoin can be re-used a large number of times before wearing out – just like
ordinary coins and banknotes. Quantum Bitcoin is the first distributed quantum money
system and we show that the lack of a paper trail implies full anonymity for the users. 

**In addition, there are no transaction fees and the system can scale to any transaction volume.**

The laws of quantum mechanics have given rise to interesting applications in computer
science, from the quadratic speedup of unstructured database search due to Grover [1] to the
polynomial-time algorithm for integer factorization by Shor [2].

These “quantum” algorithms are faster than their classical counterparts, showing that some computing problems can be solved
more efficiently if a classical computer is replaced by a quantum one.

 In addition, quantum
states are disturbed when measured, which has given rise to to quantum cryptography protocols
such as BB84 [3] and E91 [4], where the latter uses the quantum phenomena of entanglement.
See Broadbent and Schaffner [5] for a recent survey of quantum cryptography

This begs the question: can quantum mechanics help us design new, improved money systems? The answer is yes. As shown by Wiesner [6], the no-cloning theorem [7] provides an
effective basis for copy protection, although Wiesner’s results predated the actual theorem. See
Section 3 for a more detailed history of quantum money.

This paper introduces Quantum Bitcoin, a new currency that combines the copy-protection
of quantum mechanics with Bitcoin to build a payment system with several advantages over
existing systems.

Bitcoin instead uses cryptography to
distribute this task over a peer-to-peer network of users on the Internet.

Central to Bitcoin is the blockchain, which is a distributed ledger that records all transactions of every user.

Appending new data to the blockchain is the critical part of the Bitcoin protocol, and it
requires authentication of the appended data. Without authentication, a malicious miner could
add invalid transactions to the blockchain, thereby defrauding users. Traditional authentication
methods cannot be used for this purpose, as Bitcoin miners are only loosely organized, anonymous and untrusted.

Here, miners authenticate their verification by proving that they have spent computing power, and therefore energy. This prevents the Sybil attack [11], in which an attacker
can flood a hypothetical voting mechanism. Such an attack becomes prohibitively expensive
since each “vote” must be accompanied by a proof of spent energy.

Bitcoin implements the proof-of-work puzzle by packing a number of transactions into a socalled block. Each block contains, among other things, a timestamp, the nonce, the hash value
of the previous block, and the transactions [9].

Therefore, Bitcoin users are advised to wait until a transaction has been
confirmed by at least six consecutive blocks [12].

According to Nakamoto [8] the probability for a malicious miner to succeed in verifying an
invalid transaction is exponentially small in the number of confirmations as long as a majority
of miners (i.e. computing power) is used for benevolent purposes. This implies that the Bitcoin
protocol is resistant to double-spending attacks. 

As early as around 1970, Wiesner [6] proposed a scheme that uses the quantum mechanics
to produce unforgeable quantum banknotes [5],

 In contrast to quantum banknotes (where
each banknote is unique), quantum coins are all identical.

Until recently,
all quantum money proposals were private-key, however in 2009 Aaronson [22] proposed the
first public-key quantum money system

A novel proposal by Farhi et al.
[24] produced a public-key system using knot theory and superpositions of link diagrams, and
this idea was further developed by Lutomirski [25]. Finally, Aaronson and Christiano [15] based
a public-key quantum money scheme on the hidden-subspace problem.

In this paper we present the inner workings of Quantum Bitcoin, a quantum currency with
no central authority. As with most quantum money schemes the central idea is the no-cloning
theorem [7] which shows that it is impossible to copy an arbitrary quantum state |ψi. Quantum
mechanics therefore provides an excellent basis on which to build a currency, as copy-protection
is “built in”

Quantum Bitcoin uses a classical blockchain, just like the Bitcoin protocol. For the purposes
of this paper, we model the blockchain as a random-access ordered array with timestamped
dictionary entries. Blocks can be added to the end of the chain by solving a proof-of-work
puzzle, and blocks in the chain can be read using a lookup function.

We will now compare Quantum Bitcoin to the classical Bitcoin protocol by Nakamoto [8] and
show that Quantum Bitcoin has several advantages. Bitcoin transactions must be verified by
third-party miners. The time this takes averages on one hour, but as previously mentioned
the waiting time has considerable variance [12]. 

Bitcoin transactions are therefore slow; too
slow for ma customer to wait in the check-out line. In contrast, Quantum Bitcoin transactions
are immediate and only requires the receiver to have read-only access to a reasonably recent
9
copy of the blockchain. We also note that Quantum Bitcoin transactions are local, so that no
blockchain must be updated, nor does it require a third party to know of the transaction.
These local transactions are independent of network access. Bitcoin requires two-way communication with the Internet, while Quantum Bitcoin transactions can be performed in remote
areas, including in space. 

The read-only blockchain access requirement makes it possible to
store a local off-line blockchain copy in, for example, a book. To receive Quantum Bitcoin
transaction, the user simply needs to read from this book, given that the quantum bitcoin to
be verified is older than the book in question.


Another performance advantage is scalability. According to Garzik [26], Bitcoin as originally
proposed by Nakamoto [8] has an estimated global limit of seven transactions per second. In
comparison, the local transactions of Quantum Bitcoin implies that there is no upper limit
to the transaction rate. It should be noted, however, that the minting rate is limited by the
capacity of the Quantum Shard and Quantum Bitcoin blockchains. By placing the performance
restriction only in the minting procedure, the bottleneck should be much less noticeable than
if it were in the transaction rate as well.

Local transactions also mean anonymity, since only the sender and receiver are aware of
the transaction even occurring. No record, and therefore no paper trail, is created. In essence,
a Quantum Bitcoin transaction is similar to that of ordinary banknotes and coins, except no
central point of authority has to be trusted. Bitcoin, on the other hand, records all transactions
in the blockchain which allows anybody with a copy to trace transaction flows, even well after
the fact. This has been used by several authors [27–32] to de-anonymize Bitcoin users.
Another advantage of Quantum Bitcoin is that transactions are free. 

Classical Bitcoin
transactions usually require a small fee [8] to be paid to miners in order to prevent transaction
spam and provide additional incentives for miners. It is also believed that these fees will allow
mining to continue past the year 2140, when the last new bitcoin is expected to be mined. In
Bitcoin, mining is required for transactions to work, but this is not the case in Quantum Bitcoin,
again due to local transactions. 

Even better, if Quantum Bitcoin adopts an inflation control
scheme similar to that of Bitcoin, there will be no need for Quantum Bitcoin mining when the
21 million quantum bitcoin have been found. Users will still be able to perform transactions
even though mining has stopped. When this occurs, it is realistic to publish a “final version” of
the Quantum Bitcoin blockchain in a book which then would contain descriptors of all quantum
bitcoin that will ever exist.

Quantum Bitcoin is a tangible application of quantum mechanics where we construct the ideal
distributed, publicly-verifiable payment system. The currency works on its own without a
central authority, and can start to work as soon as it is experimentally possible to prepare,
store, measure and reconstruct quantum states with low enough noise. The no-cloning theorem
provides the foundation of copy-protection, and the addition of a blockchain allows us to produce
10
currency in a distributed and democratic fashion. Quantum Bitcoin is the first example of a
secure, distributed payment system with local transactions and can provide the basis for a new
paradigm for money, just like Bitcoin did in 2008.

Two parties can transfer quantum bitcoin by transferring the Quantum Bitcoin state over
a suitable channel and reading off a publicly-available blockchain. 

Transactions are settled
immediately without having to wait for confirmation from miners, and the Quantum Bitcoin
can be used and re-constructed an exponential number of times before they wear out. There is
no transaction fee, yet the system can scale to allow an unlimited transaction rate.
Note that while Quantum Bitcoin is secure against any counterfeiter with access to a quantum computer, the protocol is not unconditionally secure. The corresponding security proofs
must therefore place the standard complexity assumptions on the attacker. See Appendix A for
the complete security analysis.

We invite further study of our proposal and welcome attempts at attacking this novel protocol. There are also some challenges that should be addressed in future work: quantum bitcoin
are atomic and there is currently no way to subdivide quantum bitcoin into smaller denominations, or merge them into larger ones. A practical payment system would benefit greatly
from such mechanisms as it otherwise becomes impossible to give change in a transaction. The
security proofs in this paper should also be extended to the non-ideal case with the addition of
noise, decoherence and other experimental effects.

G. Brassard. “Brief history of quantum cryptography: A personal perspective”. In: Theory
and Practice in Information-Theoretic Security, 2005. IEEE Information Theory Workshop on. IEEE, 2005, pp. 19–23.

C. H. Bennett, G. Brassard, S. Breidbart, and S. Wiesner. “Quantum Cryptography, or
Unforgeable Subway Tokens”

F. Pastawski, N. Y. Yao, L. Jiang, M. D. Lukin, and J. I. Cirac. “Unforgeable NoiseTolerant Quantum Tokens

A. Lutomirski, S. Aaronson, E. Farhi, D. Gosset, A. Hassidim, J. Kelner, and P. Shor.
“Breaking and making quantum money: toward a new quantum cryptographic protocol”.
In: (Dec. 20, 2009). arXiv:0912.3825.

“BitIodine: Extracting Intelligence from the Bitcoin Network”. en. PhD thesis. Aug. 2013

