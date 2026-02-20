Computer Architecture is the theory to learn how computers work. It is based on pure mathematics and electronics. Computers only know two digits - 1's and 0's.They do not know anything else. But, it is very hard for humans to understand and design these systems by writing equations, which describes the movement of electrons in a wire, then to a transistor, then it builds certain logic that lets you run Minecraft. This is very hard for us humans to do this . So here we will use a technique called 'Abstraction'.
## Abstraction

The critical technique for managing complexity is abstraction: hiding details when they are not important. For example, A country contains multiple states and a state contains many districts and a district contains multiple cities.
Similarly, in case of computers, at the lowest level of abstraction is the 'Physics', the motion of electrons. The behavior of electrons is described by quantum mechanics and Maxwell’s equations. Our system is constructed from electronic devices such as transistors. By abstracting to this device level, we can ignore the individual electrons.
The next level of abstraction is 'Digital circuits' such as logic gates restrict the voltages to discrete ranges, which we will use to indicate 0 and 1. In logic design, we build more complex structures, such as adders or memories, from digital circuits.[^1]
Then comes microarchitecture, which takes these logic and gives us a thing called CPU. But to work with this, we need to define its specific instructions which in turn lets us use the registers that we will 'program' when we write code.
Then there is the software realm, that uses these logics and gives us the operating systems that lets us use the computer like we do currently like write documents, surf the web, play games etc. But this is out of scope for this stage.
[^1]: There are also Analog Circuits, but we do not need it mostly while learning computer architecture.
## Modules
Before building something, we need to set up some rules.
Since digital circuits work with discrete voltages (i.e. specific voltages for a certain operation), they are very much weaker than analog circuits that use continuous voltages. And when we use these circuits to build 'modules' and then our systems, there should not be anything that are unknown to us (this is called 'undefined behavior'). A unknown behavior in a certain module can cause a larger problem or possibly danger to us when thousands to millions of these modules are going to be used in our systems.

So the rules are - 
	1. Abstraction: Dividing the whole system into modules, then further subdividing it, so that the pieces are easier to understand.
	2. Modularity: Modules should have well-defined functions and no unanticipated behavior.
	3. Regularity: There should be uniformity as we will not going to make different types of modules for same task with any real benefit.

