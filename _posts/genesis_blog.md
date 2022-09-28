---
layout: post
cover: false
navigation: false
title: Superficial thoughts on blockchains and philosophy
date: 2022-09-26 10:18:00
tags: blockchain, layers
subclass: 'post tag-layers'
author: georgy
categories: georgy
---

Sometimes one can hear at conferences or read online that philosophy is needed in the blockchain space. Most of the time, this is a well-meaning suggestion from people deeply appreciative of the multifaceted (and at times very peculiar) nature of blockchain engineering and research. I have some reservations about whether this suggestion should be presented in such a strong modality. After all, this is a very open question if the blockchain field _needs_ philosophy. In fact, many philosophers themselves, from time to time, express doubts about whether anyone really _needs_ philosophy. At the same time, it feels somewhat disheartening to just ignore these well-meaning suggestions. Perhaps we can ask a different question: 'Can philosophy be useful (maybe even a bit) when we build, design, and use blockchain-based applications?'. And intuitively, it seems that it just might be. 

To untangle these intuitions into more specific suggestions, we can try to identify some parallels between classes of problems or areas of interest common to blockchain and philosophy people. Well, for one, both of these fields are deeply permissionless both in spirit and nature. Sure, we have a venerable tradition of academic research relevant to both of these fields, with associated formal and institutional frameworks. And yet there is no single entity or institution in the world with the definite central authority to certify something as 'true blockchain' or 'true philosophy'. 

What we call philosophy historically is a product of consensus between validating parties. Anyone can create their own philosophy, and if enough people are incentivized to maintain and participate, it will achieve liveness and decent adoption. Now the downside of that is, of course, an abundance of completely inconsistent and unworkable philosophies that nevertheless found a significant amount of confused participants throughout history. I will leave it to the reader to find parallels with the blockchain world, but there are plenty. Yet, this permissionless spirit is also a source of endless creativity and ingenuity. Not unlike impactful philosophers of the past, blockchain engineers keep inventing and re-inventing conceptual worlds, design new (sometimes so questionable they would make Plato proud) models of society, and with immense persistence try to solve problems judged to be unsolvable or unimportant by others. 

Thus, there is no surprise that many engineers, researchers, and inventors in blockchain space find themselves dabbling with issues that many philosophers have dealt with (with varying degrees of success).


## Levels of abstraction 


Coders, engineers, and computer scientists love levels of abstraction and layers. To borrow an expression from one of the lectureres from the introductory class to CS students: "We have to use layers; otherwise, our puny human brain would not be able to handle the complexity." Indeed, separating the system under question into different layers is quite a convenient way to grasp different components, functions, or problems in a more meaningful and focused way. OSI and TCP/IP models are well-known examples of conceptual models used to address complexity.

Layering models are no less popular in the context of a blockchain system. At the moment of the writing of this blog, arguments on 'layer three' scalability solutions sound practically mainstream. It is common also to hear expressions like 'this is a governance layer problem' or 'this is a social layer problem.' So it is safe to say that layer thinking is also quite popular in the blockchain space. What is less clear is whether such thinking does help to address complexity or creates more of it. The problem here is that decentralized systems like actual blockchains (some insist on calling them 'permissionless blockchains' for whatever reason) generate emergent properties and emerging complexity. Even a seemingly simple idea of DAO (we just collaborate online) is a compound complexity on top of a Defi complexity, on top of a Smart contract complexity, on top of a consensus protocol complexity, on top of network complexity. This also means that with the increase of scale and application, layering model which once was useful becomes either reductionist or naive or both. 

Case in point: the standard practice of dumping down all non-technical aspects into one 'social layer'. This may sound like a convenient way to deal with everything: a) not important right now; b) other people's problem; c) will resolve itself after the bull market resumes. However, one could argue that avoiding reductionist models is not just an exercise in intellectual honesty but also very pragmatic. Simplifications tend to ignore hidden assumptions and pile up complexity at one layer, e.g. the application layer. For example, trying to address Sybil attacks at the application layer often leads to creating new and inventive ways to degrade the privacy of system users, rather than addressing Sybils at multiple layers. 

To avoid simplification, we could use a more rational approach to the modeling of systems. For instance, we could try to consider different levels of abstraction for a blockchain system not as a technical system with a social layer but rather as a non-trivial socio-technical system. This means that we can consider decomposition into multiple layers where the functioning of each layer and system as a whole depends on the specific behavior of human participants at each layer. Which means that we should carefully consider an appropriate level of abstraction not only for the model as a whole but also for each layer.  

To avoid simplification, we could use a more rational approach to the modelling of systems. For instance, we could try to consider different level of abstraction for a blockchain system not as a technical system with a social layer but rather as a non-trivial socio-technical system. This means that the functioning of each layer and system as a whole critically depends on the specific behavior of human participants at each layer. If we use traditional layering, say borrowed from networking, this gives us only a partial picture. But if we want to analyze blockchain as a socio-technical system, we maybe need to consider the influence of the 'socio' part on different layers and how these layers are related in terms of mutual influence and dependency. For instance, we can consider layers in terms of rules for blockchain protocol: 

- **Sustainability and existence** (system of incentives and infrastructure). Sustains the whole system of rules;
- **Meta-rules** (rules for the EIP proposals and acceptance), rules for the development of codebase, rules for the acceptance of pull requests (loose social consensus); 
- **Rules creation **(Developer meetups, forums, etc.), actual EIPs, implementations, actual pull requests;
- **Application of rules **(Miners), validators;
- **Follow the rules** (Clients, smart contracts).

This type of layering can be helpful to consider when we want to highlight dependencies regarding different participants for instance. Or try to see whether some participants in the system are centralized trusted parties, or what kind of non-technical failures we should expect. But to talk about these and other issues we also need other tools which brings us to the next topic of using good conceptual frameworks.

## Conceptual analysis



Square meters of doodles on a whiteboard for a few days is what it takes to come up with just one reasonably clear model of a system. Describing it coherently and clearly to other people is yet another task. The other problem also is that there is very little agreement on conceptual terminology: is it distributed? Is it decentralized? Which one is which? Well, philosophy is all about conceptual analysis and complex mental abstractions, and yes, not all of it always make sense. Still, a good deal of philosophy can build reasonably coherent and meaningful conceptual models.

One issue which could benefit from such scrutiny is an abundance of interdisciplinary terminology in the blockchain space. As blockchains are not-trivial socio-technical systems, little surprise that concepts from humanities and engineering are often mixed together and conflated. The word 'trust' is easily one of the most problematic examples of that. In itself, it is not a problem if people want to talk about different aspects of such a rich phenomenon. But it may become a problem when we start arguing about different things, as if this is one thing. Not to mention freshly-baked blockchain critics appearing each year with the same argument: 'But no, you still have to trust developers, no Blockchain is not trustless. Check and mate blockchain people!'.The latter argument is, of course, harmless and irrelevant as it fails to grasp specific meaning of 'trust' here. I mean, one can criticize gossip protocol designers that their products fail to spread interesting and fresh gossip, but why should they care. Still, generally speaking, it is helpful to strive for conceptual clarity when engineering complex systems. 


One way to look at this problem through the prism of a conceptual analysis is to consider 'Trust' as a peculiar example of so-called conceptual slippage. This happens when the concept is borrowed from a different field (social studies/game theory) and stuffed with a different meaning (in P2P) or reduced to a very specific meaning (in security). Not to mention that many subfields in computer science also tend to have different conceptions of trust. And when the field (distributed systems) expands to incorporate new contexts (blockchains with human participants), we still keep applying modified/reduced concepts in a broader context with often confusing results. This means that we need to enrich the concept again to make it appropriate for this extended context. 

But of course, there are many more applications for this type of scrutiny. 'Consensus' is another concept that seems to bring a lot of confusion between technical and social interpretations, not only for outsiders but also for some blockchain projects. I.e., when project developers tend to forget that having a running consensus protocol does not address the issues that require social consensus. This is an honest mistake since we still do not completely understand the complexity of layers for blockchain systems. 

And then, of course, there is plenty of overlap and mixture between different terminology. For instance the lack of agreements between industry people and computer scientists on the difference between distributed and decentralized. Academics tend to distinguish between distributed centralized systems (cloud) and decentralized distributed systems (P2P); industry devs sometimes use distributed in the sense of 'super decentralized .' Speaking of which, the concept of decentralization is not only open to various interpretations in different contexts, but it is also what is called an essentially contested concept. This happens when people have a vested interest to insist on a particular definition, maybe because it fits the system they are building or for other reasons. Maybe some of these issues could be properly addressed with some help from a good old conceptual analysis and a dash of scepticism.


## Scepticism

> Philosophy is very good as skepticism: *Do we really know things as they are, are we brains in a vat? What if zoo authorities painted all horses in the local zoo into zebras.* 

And yes, this is a real citation from a respectable philosopher and not a citation of some twitter conspiracy theory. The inevitable consequence of an ever-present skepticism is that philosophers (at least those that are honest with themselves) tend to simultaneously entertain strong beliefs in the correctness of their arguments with constant doubts about the coherence and soundness of these mental constructions. 

Would such skepticism do any good in the blockchain space? There is a lot of circumstantial evidence that it would indeed. It certainly does not hurt to maintain a constant healthy dose of skepticism while engaging in blockchain experimentation, and we are not only talking about 'farm yields' that sound too good to be true, or 'supercycle' promises. Engineering and system modeling for blockchain solutions also benefit from a healthy dose of skepticism. For one, there are a lot of hidden assumptions in blockchain engineering that we tend to ignore or accept uncritically. It is safe to say that a good deal of assumptions on economic incentives or tokenomics falls in the category of hidden and implicit assumptions. Why your Proof-of-history chain has stopped 6 times in one month? Can your algorithmic coin maintain the peg? MEV is not a big deal… the list goes on. Does this mean that we should not try new things? No, of course not, but the point is that it would be helpful to be honest with our assumptions, and try to distinguish between designs and system components that we understand relatively well and those parts that we do not understand yet. 

Another cool part about skepticism is that it can help to distinguish between relevant and irrelevant critical arguments and highlight constructive criticism. For instance, in order to evaluate these arguments, we can consider whether these arguments are using a valid conceptual framework and level of abstraction that corresponds to the subject of criticism. E.g., Saying that smart contracts do not have the same qualities as legal contracts and thus should be done differently is not relevant or constructive criticism. On the other hand, saying that smart contract development driven primarily by gas-optimization strategies does not align well with good software engineering practices is a constructive criticism. 

Finally, healthy skepticism is a must-have in a space dominated by information asymmetries. This, in other words, means that the distribution of expert and accurate knowledge (sometimes referred to as 'alfa') is very, very, very uneven. One can say that blockchain space is not just characterized but defined by information asymmetries both of intentional and unintentional nature. Asymmetries are unfortunately incentivized because information advantage is often easily monetizable in this space. Then, there are also objective asymmetries rooted in the complexity of blockchain systems that require some very particular expert knowledge like cryptography of distributed systems engineering. And, of course, the constantly increasing number of new projects and more specialized solutions makes it quite challenging to navigate the space for anybody, including blockchain researchers. Here again, correct terminology and the correct level of abstraction can do wonders. Not to mention a good habit of verifying as much as possible in a true spirit of healthy skepticism, which is one of the original values of blockchain space if you think about it.  

## Evaluation

Finally, even after we have a good understanding of problems and solutions at different levels and from different angles, there is always this small question of which solution we actually choose and why. Even when we can seemingly agree (within the group of interested participants) with something, for instance, that decentralization is good, it opens up another bottomless jar of conflicting opinions. How to measure it? What is the threshold for sufficient decentralization? 

And it gets worse once we get to the point of considering different trade-offs, often without even talking about them explicitly. For example, often, there is the implicit assumption that it is OK to sacrifice a bit of decentralization for the sake of, say, the performance of ease of bootstrap at some stage of development. Which is interestingly enough sometimes turns out to be not true at all; some protocols sacrifice decentralization without gaining any wins in performance (Gromit reference). 

Coincidentally, one of the oldest subfields of philosophy deals with normative reasoning and normative judgments, that is, trying to come up with good arguments for why something is better than other and even arguments on what 'better' even means. This subfield is a moral philosophy, and contrary to popular opinion, this is not an exercise in dispatching condescending judgments about the sins of other people. In fact, some of the moral philosophy does the opposite, just search for the 'strong moral relativism'. Thus, even if we hypothetically do not care about the moral impact of blockchain applications (though I sincerely hope that more than a few people do), normative reasoning can help make relevant judgments on design choices. 

We can borrow a set of different approaches for normative reasoning: - formulating values (in a broad sense), choosing or finding a way to measure them, and then trying to compare them. And the latter can be a proper challenge. For example, what are the values or criteria of a working blockchain? Liveness, throughput, availability, fault-tolerance, censorship-resistance? Some are theoretical, abstract measurements of distributed systems, and some are more vague and loaded metrics. Even if we focus on the first three measurements, we need to ensure that when comparing the metrics and associated trade-offs, we use the same framework of evaluation, say a unified method of measurements context (light transactions vs read/write heavy smart contracts), environment context (p2p network vs cloud settings). 

Imagine multilayer systems where we have to consider social components and associated values. Here, it is quite easy to run into a situation where we try to compare values and metrics that are simply incommensurable.  On a high level, we do not even know what is a good or desirable threshold of efficiency for a consensus protocol since we do not have agreed and accurate metrics of such properties as decentralization and censorship resistance is. 

Maybe ee may measure them in the future and confidently say that some other types of consensus protocols deliver exactly the same properties as the Nakamoto consensus (for some specific use case) while say consuming less energy. But at the moment, we probably can not even start comparing (and no, Bitcoin and Ethereum are two different things used for different things). Luckily, resolving normative conflicts, tackling incommensurability of values, and constructing reasonable arguments against the background of a complete conceptual mess, are well-known activities in philosophy. Maybe some of the available methods and approaches could also be used in the blockchain space.  


## To sum up…. 

Maybe some philosophy could be used in blockchain research and engineering as well. Inspired by this thought, this blog will keep presenting and elaborating on some of these and other intuitions on blockchains and philosophy. All presented thoughts are superficial conjectures at best, and you should not expect profound insights from these posts. However, the blog's authors hope that the blockchain research and development field is still at that level of maturity when naive ideas can still be somewhat valuable; after all, "we are still early"™. 


