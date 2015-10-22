---
title: DAVIDSON'S TEST
subtitle: Donald Davidson's Critique of the Turing Test as an Expression of his Theory of Intellectual and Linguistic Competence
author: Tobias Lohse
date: \today

mainfont: regular.otf
mainfontoptions: BoldFont = bold.otf,ItalicFont = regular-italic.otf,BoldItalicFont = bold-italic.otf
geometry: top=1.5cm, bottom=2cm, left=1.5cm, right=1.5cm
papersize: a4paper

toc: true
toc-depth: 2
numbersections: true

bibliography: references.bib
link-citations: true
citation-style: style.csl
reference-section-title: References
nocite: '@*'

template: style.tex
linkcolor: black
citecolor: black
toccolor: black
urlcolor: black


abstract: |
  In his essay 'Turing's Test' [-@Davidson:1990tt], Donal Davidson discusses Alan Turing's famous proposal how to define the goal of Artificial General Intelligence and proposes a modified version that fixes the weaknesses of the original proposal. Davidson's Test illustrates his theory about the essence of linguistic and intellectual competence very well.

  Davidson's idea of triangular Epistemology

keywords: Donald\ Davidson, Philosophy\ of\ Mind, Philosophy\ of\ Language, Epistemology, Interpretation, Turing\ Test, Artificial\ Intelligence

---

<!-- Turing’s famous test aims to specify sufficient condition for intelligence on the basis of linguistic abilities. Therefore it is of natural interest to philosophy of language and philosophy of mind. Donald Davidson (1917–2003) has arguably been one of the most interesting contemporary philosophers in these areas. His thoughts are concerned with defining the essence of our ability to interpret the linguistic behaviors of others and for him too this is a condition for our ability to think. However in Turing's Test (1990) Davidson criticizes Turing’s test and tracks its insufficiency down to Turing's premise that physical and intellectual capacities can be separated clearly. For Davidson meaning can not be analyzed independent of world knowledge and the ability to interpret utterances only emerges holistically through interaction with other about experiences in a shared world. He proposes a modified test that allows the judge to observe a history of three-way engagement between the object, a shared world, and other agents in which the object develops its semantics for previously unknown occurrences. I aim to clarify the conditions of this modified test and argue why Davidson would hold these conditions not only as sufficient for intelligence but also as necessary and thus as providing a definition of intelligence. For this I will clarify why Davidson localizes the essence of intelligence in the ability to interpret utterances that can not be interpreted based on a previously acquired set of rules, practices, or conventions; and how Davidson thinks the essence of this ability can nevertheless be formally captured in an empirical unified theory of thought, meaning, and action. -->

# Introduction



### Historic background to of Davidson's Philosophy

- Vienna Circle and Empiricism
- Wittgenstein and the social aspect of language
- Quine and the new non-empiricist analytical philosophy
- semantic vs. foundational theories of meaning
- brief overview of players







### Overview of Paper

- What is the Turing Test and why is it still interesting
- How can we understand Davidson's Critique of the Turing Test
- How is Davidson's proposal for a modified test related to his Unified Theory
- How well does Davidson's Test hold up against objections?
- What can Computer Linguistics and Artificial Intelligence learn from Davidson's Test







# The Turing Test and Its Relevance





<!--
### Description of the Test

- the imitation game
- establishing a baseline
-->

First we will have to explore what the Turing Test is. Alan Turing (1912-1954) proposed his famous test first in 'Computing Machinery and Intelligence' [-@Turing:1950cm] as a replacement for the question *"Can machines think?"* --- which he deemed to vague to deserve discussion. The test is described as a game: the imitation game.

The imitation game consists of an interrogator that can communicate via a real-time text chat interface with two players. One player is a computer the other a human. The interrogator’s task is to identify the human after a given time. The computer's task is to pretend to be a human[^no-sexism] and the human's task is to help the interrogator identify him correctly. If many interrogators consistently can't tell the computer apart from the human --- as measured against an established baseline[^baseline] --- we ought to take this as an indication that the computer can think. [@Turing:1950cm, p. 433--434]



[^no-sexism]: I think it is pretty clear that Davidson misinterprets Turing on the sexist aspect of the test [see @Davidson:1990tt, p. 78]. Turing didn't mean that the interrogator's task would be to decide on the gender, and the computers task to imitate a woman. This becomes pretty clear when Turing says: *"If the man were to try and pretend to be the machine [...]"* [-@Turing:1950cm, p. 435] and from all his examples that are focused on how the machine can imitate being a human not a woman. [See also  @Copeland:2000tt, p. 526.]

[^baseline]: Turing's idea is that a baseline is established by the traditional imitation game, in which a man tries to imitate a woman and the interrogator has to decide on the gender. While this might not be the best way to establish a baseline it means that Davidson's critique that *"Turing does not say what he would make of a computer that was consistently chosen over the [...human] to be the [...human]"* [-@Davidson:1990tt, p. 78], is ill conceived, as the computer will always unambiguously fall over or under the baseline within a margin of error.

## Interpretations and Versions of the Turing Test



<!--
### Different Interpretations of the Turing Test

- Interpretation as definition, sufficient conditions, just framework to gather evidence
- two or one player?
- definition of intelligence uninteresting. Focus on application of intelligence
-->

But the interpretations are not as straight forward, as it might seem. The main question is what the Turing Test is supposed to be. There are three main interpretations:

1. The Turing Test is taken as an operational definition --- a sufficient and necessary condition --- of intelligence: Something is intelligent[^intelligence] if and only if it passes the Turing Test. [For example see @Millar:1973pi.]
2. The Turing Test is taken as a sufficient condition of intelligence: Something is intelligent if it passes the Turing Test. But it is not necessary for something to pass the Turing test in order to be intelligent.
3. The Turing Test is taken *"as a potential source of good inductive evidence for"* intelligence: If Something passed the Turing Test one would be justified for inductively inferring that it is intelligent. [See @Moor:1976at, pp. 249, 251]

The first interpretation and any reading of intelligence in a broader sense are clearly not in line with Turing's ideas, but the interpretation of the imitation game as a test clearly is. This becomes clear from the following section of a radio interview [-@Turing:1952ca], which represents Turing's simplest expression of the test:

> *“I don’t want to give a definition of thinking [...] I don’t really see that we need to agree on a definition at all. The important thing is to try to draw a line between the properties of a brain, or of a man, that we want to discuss, and those that we don’t. […] I would like to suggest a particular kind of test that one might apply to a machine. You might call it a test to see whether the machine thinks, but it would be better to avoid begging the question, and say that the machines that pass are (let’s say) ‘Grade A’ machines. The idea of the test is that the machine has to try and pretend to be a man, by answering questions put to it, and it will only pass if the pretence is reasonably convincing.”* [@Turing:1952ca, p. 466]

In this simplified version of the test there is no second human player. While this might be limiting for a quantitative analysis, it ensures the focuses on the main question and removes any undue emphasis on strategy. The simplified version that Davidson proposes for discussion is basically identical except for the fact that Davidson proposes that *"the interrogator [...should] be asked to decide whether or not the object is thinking."* [-@Davidson:1990tt, p. 81] If we assume that any bias against the object's ability to think can be removed, this seems to be the clearest expression of Turing's idea and is therefore the version we will refer to in the following.

It also becomes fairly clear that a reading in Moor's third sense does Turing most justice. But where does that leave the relevance of the Turing Test?



[^intelligence]: The term intelligence is adopted here purely in reference to Artificial Intelligence. Davidson [-@Davidson:1995ct] mostly uses the term rationality to refer to the concept that this thesis is concerned with and I will introduce and explicate the term intellectual competence for this in [section 4.1][The Distinction between Linguistic Competence and Performance].

## Relevance of the Test and the Turing Principle



<!--
### Relevance of the Test

- the challenge of AGI
- How the TT solves the definitonary problem of AGI
- other tests
- Why the TT is a good test
-->

The main challenge of the field of so called *Artificial General Intelligence* (AGI) is to give a clear definition of its topic. Unlike other propositions for an operational definition[^agi-tests] of AGI, the Turing Tests provides a clear and well justified empiric goal.

> *"there are two strong arguments why the Turing test is a good format for gathering inductive evidence. First, the Turing test permits direct or indirect testing of virtually all of the activities one would count as evidence for thinking. Secondly, the Turing test encourages severe testing. […] the computer would be tested in detail over a wide range of subjects […and] the interrogator's goal is to find a refuting instance which gives the computer away.”* [@Moor:1976at, pp. 251-252]

Critics of the Turing Test as a goal for AGI mostly fall into two camps. The first point Moor provides is aimed against the first type of critics that suggests the test sets the wrong goal. As Moor argues, communication is a very clear framework to investigate all kinds of thinking. A further pragmatic reason for the relevance of the Turing Test --- that I would add --- is: Natural language communication provides a good gold standard for completely general and seamless interfaces. Many of those critics mistake the question as philosophic while it is best treated definitional. Computer Scientists ought not to be concerned with defining intelligence in general but with a good definition for *"Grade A"* computers --- to use Turing's terminology. In this regard the interpretation of the Turing Test as a framework to gather empiric evidence can be set as a clear definition of the goal of AGI.


The other type of critics questions the adequacy of the test to determine wether its goal is reached. Moor's second point is aimed against that by pointing out how well the test encourages thorough testing. The critics sometimes mistake Turing's predictions as a specification that the Test ought to take only 5 minutes and limited implementations of the Turing Test that favor engineering tricks like the Loebner Prize[^loebner-critique] discredit Turing's intentions. I agree with Copeland's interpretation of Turing: The goal the test sets is a computer that *"plays the imitation game successfully come what may, with no field of human endeavour barred, and for any length of time commensurate with the human lifespan."* [@Copeland:2000tt, p. 530]



[^agi-tests]: See @Muehlhauser:2013wa for a brief overview of operational definitions of AGI, including the coffe-brewing and college test. From a philosophical perspective all those seem rather random and dubious --- certainly much further away from clearly capturing necessary conditions of human-like intellectual competences.

[^loebner-critique]: Shieber [-@Shieber:1994lr] criticizes the Loebner prize for its inappropriateness to award advances in natural-language-processing techniques instead of engineering tricks oriented to the exigencies of the restricted task like parrying and insertion of random typing errors. But the setup of the scoring system alone shows how pointless it is to even judge current systems by a direct Turing Test.

<!--
### Turing's Three Main Claims about Artificial Intelligence

- Turing supports the fact that a universal computer can simulate every physical process including the brain. (also known as the Turing Principle, Wikipedia)
- Turing believes that communication is a suitable means to expose the relevant intellectual abilities that determine wether a machine can think.
- Turing thinks the imitation game specifically is suited to test the communicative abilities of the computer.
-->

### Turing's three main claims {-}

We have established that:

1. Turing sees communication as suitable to expose the relevant intellectual abilities that determine wether a computer can perform tasks on paar with a human being.
2. Turing thinks that his test specifically can determine wether a computer possesses such communicative abilities.

But there further is a third claim. [@Copeland:2000tt, p. 530]  Which is known as the Turing Principle[^turing-thesis]:

3. Turing believes that universal computers can simulate any physical process including the brain.

This is implicit in @Turing:1950cm and most clearly expressed in @Turing:1951cd, p. 463: *"If it is accepted that real brains, as found in animals, and in particular in men, are a sort of machine it will follow that our digital computer suitably programmed will behave like a brain."*

This is a much more controversial claim of course and --- as Turing is well aware --- he has few arguments and less evidence for it. It is important however to realize this as a separate and fully independent claim from the others.



[^turing-thesis]: This is also known as the Church–Turing–Deutsch principle and represents an extension of the well known Church-Turing thesis to artificial intelligence.

## Turing on Machine Learning

<!--
### State of Passing the Test

- Move from AGI to AI and Machine Learning
- Turing's (wrong) predictions
- Loebner Prize state
- 1952 predictions
- success through NN scale
-->

Unlike the obsession in popular culture with human-like artificial intelligence might suggest, the interest of Computer Scientists in the last years has been more focused on domain specific intelligence for specific applications (most notably: image recognition, domain specific language processing, and robotics). The field that is concerned which such *weak* AI is referred to as *'Artificial Intelligence'* these days and is most focused on the *Machine Learning* approach. The field that is concerned with human like *strong* AI is the field of Artificial General Intelligence (AGI) that we talked about in the previous section. This shift of focus has mainly been due to a lack of success in AGI.

Turing believed that by the turn of the century there would be computers that *"play the imitation game so well that an average interrogator will not have more than 70 per cent chance of making the right identification after five minutes of questioning."* [-@Turing:1950cm, p. 442] Recent winners of the Loebner price [@AISB:lp], which is awarded to the most humanlike chatbot judged by a Turing-inspired test, show that this has not quite come to pass. On the other hand Turing himself said that it would take *"at least 100 years"* [-@Turing:1952ca, p. 434] until a general Turing Test could be passed --- and the goal of AGI reached --- which is still well in the realm of the possible. Turing's wrong prediction of the development can be mainly accredited to his underestimation of the needed processing power for Machine Learning [-@Turing:1950cm, p. 455]. Recent accomplishments in AI with deep neural networks for example have only become feasible because computers are able to run networks with millions of neurons in real time.[^nn-size]



[^nn-size]: Steven Wolfram writes: *"Computers (and especially linear algebra in GPUs) got fast enough that [...] it became practical to train neural networks with millions of neurons, on millions of examples. [...] this suddenly brought large-scale practical applications within reach. [...] I don’t think it’s a coincidence that this happened right when the number of artificial neurons being used came within striking distance of the number of neurons in relevant parts of our brains. [...] if we’re trying to achieve “human-like” image identification [...] then this defines a certain scale of problem, which, it appears, can be solved with a “human-scale” neural network."* [-@Wolfram:2015ii]

<!--
### Turing on how to device a machine that can pass the test

- child mind with learning ability
- sensory organs
- interaction with teacher
- Helen Keller example
- reverse engineering approach to AI with neural networks most successfull
- Machine Learning
- 4th core claim from Turing
-->



### Turing's fourth claim {-}

However Turing's idea about how to build a computer that could pass his test are more interesting than his timeline predictions. His claim that *"the problem [of building a computer that passes the Turing Test] is mainly one of programming"* [-@Turing:1950cm, p. 455] still rings true today.

We have already learned of his idea that computers should be able to simulate the brain [-@Turing:1951cd]. Indeed this reverse engineering approach to AI is the basic idea behind those neural networks that power the most successful image entity-recognition algorithms today and was already investigated by @Turing:1948im [see also @Copeland:1999at]. It seems plausible that we might achieve AGI through brain simulation bevor we deeply understand how the brain works.

Even more interesting Turing also predicted the Machine Learning approach to build intelligent algorithms and saw it's non-deterministic nature as a characteristic feature.

> *"Instead of trying to produce a programme to simulate the adult mind, why not rather try to produce one which simulates the child's? If this were then subjected to an appropriate course of education one would obtain the adult brain. [...] We have thus divided our problem into two parts. The child-programme and the education process. These two remain very closely connected. We cannot expect to find a good child-machine at the first attempt. One must experiment with teaching one such machine and see how well it learns."* [@Turing:1950cm, p. 456]
>
> *"An important feature of a learning machine is that its teacher will often be very largely ignorant of quite what is going on inside, although he may still be able to some extent to predict his pupil's behaviour. [...] This is in clear contrast with normal procedure when using a machine to do computations : one's object is then to have a clear mental picture of the state of the machine at each moment in the computation. [...] Processes that are learnt do not produce a hundred per cent certainty of result; if they did they could not be unlearnt."* [@Turing:1950cm, p. 458-459]

This description is very much how modern statistical Machine Learning algorithms work. They consist of an algorithm that describes a mathematical model which is trained with human annotate data (for example a grammar analysis of sentences) and are then able to perform their task on similar data. [See @Schubert:2015cl for an overview about approaches to Natural Language Processing; and @Jurafsky:2015uu for a more technical introduction.] As Turing mentions this is a paradigm shift from classical algorithms which have results that are clearly defined by the programmer and predictable independent of any training data. We might add a fourth core claim:

4. Turing believes that the approach to device intelligent computers must be based on learning algorithms that are trained and do not behave predictable in a classic sense.

We should note that devising intelligent algorithms is a quite different task and involves techniques where an interpretation of the state of the program at each step becomes hard too impossible --- especially in the case of deep neural networks. We will see later why this matters for a Davidsonian perspective.

<!--
### Summary and Conclusion

- We are right in taking the simplified version of the test as the purest expression of Turing's idea
- The tests relevance is mainly that it provides the clearest answer to what AGI is about.
- Turing has rightly identified the main question of research in AGI to be about how a machine can learn to communicate.
- independence of the Turing principle from his other more interesting claims.
- The nature of Machine Learning.
-->

### Summary {-}

We have seen that a simplified interpretation of the Turing Test as proposed in @Davidson:1990tt is the core of Turing's idea. However we have also seen that an interpretation of the Turing Test as an operational definition or sufficient condition for intelligence is not inline with Turing's writing. Instead I have proposed to follow @Moor:1976at and interpret the test as a framework to collect empiric evidence that a computer can perform human like tasks. We have seen that this can provide a good and clear definition of a special class of computers that are the goal of AGI research.

Furthermore we have established that Turing first of all claims that (1) communication abilities are representative for intellectual abilities in general and (2) that his test is adequate to evaluate those abilities. I have pointed out that his claim (3) that computers can simulate the brain, the Turing principle, which is the main point most philosophers critique is completely independent of the other claims and is the least essential one for Turing

Lastly we have seen that Turing made pathbreaking suggestions about how to device algorithms that could pass his test. Such algorithms (4) need to be able to learn when trained with data and that different from classical algorithms their outcome is not predictable and the states of their operation are not easily interpretable.





# Davidson's Critique of the Turing Test

## Relevance of Turing's Test for Davidson

### Why the test is interesting to Davidson

- Test is concerned with the nature of thought
- Pragmatic approach to the question of thought
- Empiric criterion for thought
- Not confined to maschines

> *"The whole thinking process is still rather mysterious to us, but I believe that the attempt to make a thinking machine will help us greatly in finding out how we think ourselves."* [@Turing:1951cd, p. 465]


*"the test is designed to throw light on the nature of thought."* [@Davidson:1990tt, p. 78]



> *“I believe that another human being thinks because his ability to think is part of a theory I have to explain his actions. [...] the evidence for the theory comes from the outward behavior of the person. [...] there is no reason why knowledge of computer thinking can not arise in the same way. I can use the computer's behavior as evidence in assessing my theory about its information processing. In neither the human case nor the computer case must I consider the thinking to be on a close analogy with my own, for the evidence might dictate that the human or computer discriminates and evaluates quite differently than I do.”* [@Moor:1976at, p. 251]




### Where does Davidson agree

- There should be an empiric test for intellect
- Linguistic comptetence is essential for intellect
- General/Strong AI might well be possible
  - Davidson sees no argument why AI shouldn't be possible
  - AI through Brain simulation should be possible
  - See also 'Representation and Interpretation' [@Davidson:1990ri]
- No need for introspection into working of mind (against Searle's chinese room)

Turing's proposed test shows that he agrees with Davidson on the fact that linguistic competence is essential to intellect. And I think we also have to interpret Davidson and Turing as agreeing that there is a scientific approach that can describe essential parts of our linguistic competence. In the case of Turing this is evident in his believe that there is a program that allows the computer to win the imitation game. For Davidson it is evident in his proposal of the empiric Unified Theory that can capture the essence of linguistic competence and rationality. We will investigate Davidson's ideas further in [Unified Theory of Understanding].










## Davidson's Critique of the Turing's Test

### The core argument: knowledge comes from interaction in shared world

- Rejection of sharp distinction between mental and physical (especially sensory) abilities (E4.5)
- distinction between semantic and syntactic abilities
(+E5.8)
- Relation to Agreement between Descartes and Turing
  - Both come from the idea that knowledge is simply in the head
- Even Turing's Helen Keller example lacks as she was interacting with the world through touch.
- Connected to rejection of Cartesion Epistemology



### Does Davidson's Critique Do Justice to Turing?

- Davidson has a good point
- but he doesn't do justice to Turing's thoughts on Machine Learning that would deserve a discussion in his paper



## Davidson's Proposal for a Modified Test

### Observe a History of interaction with the world

- The ability to determine non predefined meaning is essential for intelligence





### Summary and Conclusion



# Conditions for Linguistic Competence

## The Distinction between Linguistic Competence and Performance

### Distinction between sufficient and necessary conditions of linguistic competence

- relation to term linguistic competence and linguistic performence
- analogy to physics not being able to describe actual natural systems but only systems under ideal conditions
- See (E4.8, E5.8)



I use the term *linguistic competence*[^linguistic-competence] here to refer to Davidson's idea of the essential aspect of understanding language vs. the practical understanding of language.


[^linguistic-competence]: The term linguistic competence was introduced by Chomsky who makes a "fundamental distinction between competence (the speaker-hearer's knowledge of his language) and performance (the actual use of language in concrete situation)" [@Chomsky:2014at, p. 4]. While Davidson  criticizes the idea of linguistic competence as knowledge of a language, he adopts the term for the description of his theory that describes the interpreters essential competence in 'A Nice Derangement of Epitaphs' [-@Davidson:1986nd].



### Relation to Davidson's Philosophy

- truth conditions as a formal language
- Unified Theory, Radical Interpretation
- Sucessfull Communication & Anti-Conventionalism & Holims of knowledge





## Recursiveness and Empirism

### The Importance of Empirical Theories

- No a priori knowledge about language(-learning), only empirical knowledge (E2.1)



### Learnable Languages

- Finite set of linguistic primitives gives rise to infinite linguistic expressions

'Theories of Meaning and Learnable Languages' [@Davidson:1965tm]



## The Social Aspect of Language

### The Primacy of Ideolect

- relevance of interpretation rather than meaning (+E2.2)
  - see similarities to Gadamer's Hermeneutics of Wirkungsgeschichte (Bertram 2012)
- Relevance of Intention in communication (+E5.10)
- Arguments for primacy of ideoloect over language
  - Malapropisms and the like (E5.7)







### Why is language necessarily Social

- Wittgenstein's norm of actually getting it right in language
  - also see language game analogy in anti conventionalism (2.18)
  - and importance of disctinction between true and false beliefs in triangulation (E3.14)
- Truth only determined trough communication
  - see also Plato, socrates (E5.16)













## Anti-Conventionalism

### arguments against conventionalism

- impossibility of public sign for sincerity
- language game analogy (+E5.8)





### Remarks about how understanding does work

- At the end of [-@Davidson:1984cc], Davidson says that understanding can't be formally described
- Relation to distinction linguistic between competence and prerformence



## The Triangular Nature of Knowledge



### The basic problem of Epistemology

- Distinctiveness of three types of Knowledge (subjective, intersubjective, objective) (E3.14)
- Three Questions of Epistemology (E3.14)
  - how to know other minds
  - how to know world
  - how to know own mind without evidence





### Rejection of other Epistemologies

- Rejection of Positivism (reductionism to world knowledge) (E3.14)
- Rejection of empiricsit Epistemology (E3.14, E2.1)
  - No primacy of names and predicates in the foreground of senses
  - doesn't he contradict that in E2.9 and E4.8?
- Rejection of Cartesion Etymology (primacy of knowledge of one's own mind) (E3.14, E3.3, E3.13)
  - Rejection of skepticism (E3.14, SEP Davidson, E4.1)







### The Process of Gaining Knowledge

- Interdependency of three varieties of Knowledge
- Importance of disctinction between true and false beliefs (E5.8, E3.14, E4.1, SEP Davidson)
- Principle of Charity (Coherence and Correspondence)
(E3.14, E2.9, E3.14)
- Reaction to stimuli (E3.14)
  - proximal vs. distal stimuli (E5.4)
- Iscrutability of Reference / Indeterminacy of meaning (Quine Word and Object, E5.3, E2.16, E3.14)











### The Underlying Ontology and Metaphysics

- Ontology of only objects and events (E3.14, E5.4)
- Directness of knowledge of world
  - no intermediary entities (5.3, E5.4, E3.10)
  - no mentales, language only through communication, meaning given causally by objects events (E5.9)
- Truth as elementary non-reducible concept (E5.2, E2.I)



### Anomalous Monism

- parallels to Spinoza's causal theory of affects (E5.20)
- see arguments for irreducibility of mental in Tirangulation (E3.14)
- Reasons for Irreducibility/anaomalism of Mental to Physical (E3.14, E4.8)
  - Irreducibility of knowledge of belief to knowledge of world
  - causal nature of the mental (+E1.11, E4.8)
  - Missing independent mode of communication about mental theories (+E4.8)
- Turing's discussing of rule based behavior




Turing discusses an interesting objection to his test that is related to Anomalous Monism [-@Turing:1950cm, p 452f]. If our behavior is not ruled by strict laws but a computer is. How could it ever simulate our behavior. Turing argues that this is simply an assumptions (and even if who says that the mental states of a computer could for example not supervene on the sates of its neural network). Turing uses cryptography as an example for a process where a computer can produce output which can not be tracked back to its originating rules (but this of course is a practical limitation not a theoretical one, since all cryptographic functions can be reversed with infinite processing power.)

This raises and important question wether the anomalism of the mental is connected to our linguistic competences (or maybe just to our effectiveness?) and how computers/the unified theory could account for it. ***(need to reread in three varieties of knowledge)***

### Summary and Conclusion

# Davidson's Theory of Intellectual and Linguistic Competence

## Sources for Davidson's Theory of Intellectual and Linguistic Competence

### What is this theory of interpretation

- Anomalous Monism
- Davidson's Program
- Radical Interpretation
- Triangulation
- Unified theory of Thought, Action, and Meaning
- Prior and Passing Theories
- The social Aspect of language



So what is it that I am referring to when I speak about Davidson's theory of interpretation? While this seems like a straight forward question it is a little more complicated because of the distributed nature of Davidson's work.

Davidson's theory can be traced back to his rejection of meaning and idea that interpretation can be described as a process of 'translating' utterances into truth conditions based on assumptions about the believes of the speaker using the principle of Charity, which he develops in 'Truth and Meaning'[^davidsons-program] [@Davidson:1967tm] and 'Radical Interpretation' [@Davidson:1973ri].




[^davidsons-program]: His idea that truth conditions (T-Sentences) are all that is needed to explain interpretation, and any more fundamental notion of meaning is misconceived, has also led to what is known as Davidson's Program: The attempt to give an account of the interpretation of utterances purely with the means of first order logic.

## Outline of the Unified Theory

### Decision Theory



### Representation of Meaning/Linguistic Content

- Meaning as Language (E3.14, E2.2) (not things in world, not entities sui generis)





### How does the interpretation Process work

## Relation to Davidson's Test

### Interpreting Davidson's Test as a Test for a Unified Theory 'machine'



### Summary and Conclusion

## Possible Objections against Davidson's Test

### Behaviorism

### Mechanism

### Scope of the Test

### Blockheads

### The Chinese Room (Internal Operation)

### French: Associative Priming and Rating Games



### Ability to cope with Abstract Terms

- It remains unclear how well Davidson's theory might be able to cope with abstract terms in the language.
- He throws very little light on how understanding of abstract terms might work.
- There are good reason's to doubt that communication about abstract terms can work in the same way as other communication. Something like the Wirkungsgeschichte becomes way more plausible, if we look at how culturally loaded language is
- See also Bertram's critique: Gadamer's idea

[@Bertram:2012ta]
[@Davidson:1997gp]




### Wirkungsgeschichte

# Conclusion

## Prospects of Davidson's Pragmatic Theory



While Davidson is skeptical about the possibility of explaining our linguistic performance. He believes that there is a pragmatic and empirical theory about the essence of linguistic competence.

## Implications for Artificial Intelligence and Computer Linguistics





Davidson tries to device a theory that can model human intellectual abilities in an empiric theory that has the power to explain them. (As opposed to only a simulation of the brain by a machine)

While it currently seems more probable that Turing’s Test and also Davidson’s Test will be passed by a computer that leverages trained large scale deep neural networks aka. something into the direction of simulating the brain. Davidson’s consideration still provide important input into what is needed to achieve human level of natural language abilities. That is the ability to somehow interact with the world and have some sensory impression of it and have a triangular model of determining world interaction.

### Possibility of AI and the importance of Language

- Davidson sees artificial intelligence as possible.
- He agrees that language is the key test for intelligence.



### Important boundary conditions for linguistic competence

- Linguistic and intellectual competence are inherently social/intersubjective
- Linguistic and intellectual competence require interaction with the shared world (empiric)





### Denial of conventionalism and statistical linguistics

- The social and empiric traits of linguistic and intellectual competence can not be modeled by conventionalism, if this convention requires a previously shared common practice. Interpretation emerges in the instance of communication and cannot be predetermined in anyway.
- Abilities of linguistic interaction can not be clearly separated from abilities for physical interaction. Both are necessary for intelligence.









