Is a [[Consesus Protocol]] created by [[Leslie Lamport]] in 1989, and it is used in multiple [[Graph Database Systems]] like [[neo4j]]. It is also used in [[📜 Cassandra]] for leader election.

Algorithm:
There are 3 roles:
- **Proposers** - wants to propose value _v_ an wants the system to reach consensus on this value. Sends a _prepare(id)_ to all _acceptors_ and expects a _promise -> value_ response. Upon reception:
	1. If the majority (_quorum_) sends a _promise_ with a null value, the _proposer_ sends an _accept(id, v)_. If he receives again the majority of the responses with the _id_ and _v_, consensus has been achieved for value _v_
	2. If 
	3. If the _proposer_ doesn't get the majority number of _promise_ responses, it will try again with a higher _id_
- **Acceptors**
- **Listeners**