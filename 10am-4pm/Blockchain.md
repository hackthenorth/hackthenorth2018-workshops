## Integrating Blockchain: Intro to Web3
### Presenters: Calvin Chan & Anthony Zhang

**Target Audience:** 
- Software developers with minimal or no prior experience with blockchain technologies, but who are interested in getting started with writing applications that run on top of the blockchain

**Suggested Prerequisites:** 
- Basic data structures, algorithms, and networking
- Basic knowledge of Javascript, CSS, and HTML	
- Basic familiarity with C-family programming languages

**Workshop Goals:**

This workshop will teach you to create a simple distributed application using a popular blockchain platform. Along the way, we’ll cover how the technology works, and how your applications can interact with others within the ecosystem.

**Description:**

This workshop is an introduction to blockchain technology in general, and Ethereum development in particular. In it, we’ll create a distributed application from scratch, and briefly cover important concepts along the way. Live demos and code samples will be provided at the end!

**Content Breakdown:**
- The Impact
    - Showcase the impact blockchain technology has made on modern computing
    - Overview of the components that make up Ethereum as a system
- The Technology
    - An explanation of how blockchains work, in concrete terms, and how it’s applied in Ethereum systems
    - Develop the concepts from first principles and design requirements
- Smart Contracts
    - An introduction to what smart contracts are, what they’re for, and how they work within the Ethereum ecosystem
    - Live demo of deploying a smart contract
- Distributed Applications
    - An overview of what dApps are, how they’re written, and a live demo of writing and deploying a dApp using GitHub pages, Web3.js, and Infura
- Q&A + Try it yourself!
    - Audience questions, plus hands-on help with hackers writing their own smart contracts and dApps

**[Slides](https://docs.google.com/presentation/d/1S4xGjIV7tTWl1gHPl2rbhVs5Ouvirt8nq72Skf0O-JI/edit
)**

--- 

**Key Notes:**
* Ethereum – A really slow, trustless computer
    * Trustless distributed computing is really useful in environments when there are many actors with conflicting interests.
    * Different parties want the computer to give different results, and are willing to sabotage it to get what they want – Ethereum provides a system that forces 	everyone to agree on the true result of the computation, hence “trustless”.
    * The result is a globally distributed computer with roughly the computing power of a old phone.

* Blockchains – An append-only buffer
    * A blockchain implements a Buffer 	ADT, with O(1) append time, O(1) random access, and Ω(2^n) in-place modification.
    * In Ethereum, the blockchain currently limits appends to one per roughly 15 seconds by requiring blocks that are appended to be “mined”.
    * To ensure every node has access 	to every block, a gossip protocol spreads new blocks between peers. Since blocks take 15 seconds on average to mine, there’s plenty of time for peers to get new blocks.
    * When a peer receives multiple conflicting chains, longer one is chosen as canonical – more effort has been put into mining blocks. In other words, to sabotage the blockchain you would need to be able to convince enough people 	to join you in putting in effort that you overpower the other groups.

* Smart contracts – A computer running on the blockchain
    * Within the Buffer exposed by the blockchain, we can store an array of transactions.
    * For blockchain systems like Bitcoin, transactions are a sequence of instructions in a stack machine language. The most common sequence of instructions is one 	that transfers balance from one account to another.
    * For Ethereum, transactions are also a sequence of stack machine instructions (known as EVM bytecode), but with more capabilities, including modifying RAM, 	reading storage, and performing computations.
    * Most people will be writing 	programs using higher-level languages like Solidity, which compile down to the bytecode.
	
* dApps – Interacting with the rest of the world
    * Typically, by dApp people are referring to web applications where the frontend is served via traditional static website hosts (or technologies like IPFS/Swarm), and the backend is some blockchain or other distributed technology.
    * Most commonly, the frontend interacts with the Ethereum blockchain, using libraries such as Web3.js to access the Ethereum network. Services like Infura currently offer hosted nodes for free, and Web3.js users can connect directly to these nodes.
    * Cryptographic secrets are managed either in the frontend Javascript, or via extensions such as Metamask, which perform operations such as signing on the user’s behalf.
