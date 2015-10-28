---
title: DAVIDSON'S TEST
subtitle: Donald Davidson's Critique of the Turing Test as an Expression of his Theory of Intellectual and Linguistic Competence
author: Tobias Lohse
date: \today

papersize: a4paper
toc: true
toc-depth: 2

bibliography: references.bib
link-citations: true
citation-style: style.csl
nocite: '@*'

abstract: |
  In this paper I discuss Donald Davidson's critique [-@Davidson:1990tt] of the Turing Test in which he agrees with Turing [-@Turing:1950cm] that communication is the essential hallmark of human-like intellectual abilities and proposes a modified version of the Turing Test that requires the judge to observe the learning process of the computer through social interactions in a shared world. This modified test serves as an illustration of Davidsons ideas about the nature of our linguistic and intellectual competences, especially his Epistemology of 'Triangulation' of subjective, intersubjective, and objective knowledge [-@Davidson:1991tv] and his empirical 'Unified Theory of Meaning, and Action' [-@Davidson:1980tu]. My discussion aims to expose how we can treat Davidson's Test as an operational definition of his concept of intellectual competence and how it relates to his rejection of other theories of meaning.

  Furthermore, I argue that Davidson and Turing agree that the essence of communication can be captured in a formal theory and that both saw social interaction in a shared world as essential for human-like intellectual competence; for Davidson this is grounded in his idea of a triangular Epistemology; for Turing it is grounded in his understanding that Machine Learning is needed to achieve Artificial Intelligence. Davidson however goes further by denying that such experience of interaction can simply be encoded in predetermined conventions, and requiring the ability for 'Radical Interpretation' of previously unknown expressions in the very instance of communication. In the end, I give an outlook for the implications of Davidson's thoughts for Machine Learning and Computer Linguistic approaches that would deserve further research.

keywords: |
  Donald\ Davidson, Philosophy\ of\ Mind, Philosophy\ of\ Language, Epistemology, Interpretation, Turing\ Test, Artificial\ Intelligence, Computer\ Linguistic

---

# Introduction {-}




<!--
- What is the Turing Test and why is it still interesting
- How can we understand Davidson's Critique of the Turing Test
- How is Davidson's proposal for a modified test related to his Unified Theory
- How well does Davidson's Test hold up against objections?
- What can Computer Linguistics and Artificial Intelligence learn from Davidson's Test
-->

This paper discuses Donald Davidson's critique [-@Davidson:1990tt] of the Turing Test as an illustration of Davidson's theory of linguistic and intellectual competence. After a short Introduction to Donald Davidson it consists of four main sections.

[**Section 1**](#section1) explores Turing's original ideas and their relevance. It discusses different interpretations and versions of the Turing Test and establishes wich interpretation I follow. It also contains a discussion of the significance of the test and Turing's ideas about Machine Learning for the field of 'Artificial (General) Intelligence'.

[**Section 2**](#section2) presents the core agreements and points of criticism from Davidson and evaluates in how far they do Turing justice. It ends with a display of Davidson's proposal for a modified test that allows to judge the computer based on an observation of its learning process.

[**Section 3**](#section3) delves into the necessary conditions Davidson requires from a theory of linguistic competence, starting with a definition of the concept of linguistic competence in Davidson's writing. It discusses the empirical, recursive, and extensional requirements for theories of meaning, the social aspect of language, Davidson's anti-conventionalism, and the triangular nature of cognition and interpretation.

[**Section 4**](#section4) seeks to illuminate Davidson's theory of intellectual and linguistic competence and show in how far Davidson's modified Turing Test might act as an operational definition of the topic of this theory. It also discusses how well Davidson's Test fences against some objections.

[I conclude][Conclusion] with a summary of the core agreements and distinctions between Davidson and Turing and a brief discussion of the implications of Davidson's ideas (especially his empirical theory and anti-conventionalism) for Computer Linguistic and Machine Learning approaches that would deserve further investigation.



## Introduction to Donald Davidson {-}




Donald Davidson (1917--2003) "was one of the most important philosophers of [action, language, and mind in] the latter half of the twentieth century [...] with a reception and influence that, of American philosophers, is perhaps matched only by that of [his friend, mentor, and colleague] W. V. O. Quine" [@Malpas:2015dd, p. 1].  His thoughts are exposed through a collection of very densely written essays (published from 1963--2001)[^life] which "form a mosaic out of which emerges a unified and surprisingly elegant overall view of the mind and its relation to the world. It sees our *nature as linguistic beings* as the key to the possibility of thought, to the objectivity of the world [...], and to how the [irreducably mental] mind moves us to action in a [physical] world" [@Lepore:2009d, p. 1, emphasis added]

To give a very brief overview of Davidson's philosophy:

![Donald Davidson by David Levine in Forum Gallery, New York](donald-davidson.jpg)

- He takes the causal nature of thought [-@Davidson:1963ar] as an argument for the supervenience and irreducibility of the mental to the physical known as 'Anomalous Monism' [-@Davidson:1970me].
- He argues that semantic theories for natural languages must be recursive [-@Davidson:1965tm] and that meaning and propositions can be replace by truth conditions and distal stimuli [-@Davidson:1967tm].
- Based on Quine's Radical Translation, he takes interpretation as a process of adapting a theory of intertwined understanding and believe about the speaker [-@Davidson:1973ri].
- He rejects Conventionalism [-@Davidson:1984cc] based on his argument for the primacy of ideolect, placing the social aspect of language in Epystemology [-@Davidson:1994sa].
- Rejecting positivist and cartesian Epistemology, he sees knowledge of self, world, and others as interdependent [-@Davidson:1991tv].
- His Unified Theory [-@Davidson:1980tu] aims to captures the essence [-@Davidson:1995ct] of mind, language, and action.
- He compares his philosophy to Spinoza [-@Davidson:1999sc] and Plato and Gadamer [-@Davidson:1997gp].



[^life]: It is remarkable that a contemporary philosopher of Davidson's calibre only started publishing his relevant papers in his 40s after he had been a professor for over a decade. The publication dates of Davidson's papers ought to be interpreted with care though. His fried and student Ernie Lepore recounts: "[Davidson was] adventurous and daring [...] from early on right up until his death. [...] Donald was without even the slightest speck of careerism from the very start. He traveled the world giving papers in exotic places and often handed them over to local journals upon request. [...M]any of the papers were written somewhat contemporaneously. [...Some were] given much earlier than they were published and relatively around the same time. [...] I possess a mimeographed copy of his quotation paper dated from the early 60’s, long before its 1979 publication." [Lepore:2003me].

    Davidson's life and career are actually quite inspiring, *fascinating*, and unconventional. Davidson started out in the History of Philosophy and ventured into psychology and economy during his studies and as a professor. Certainly it is no coincidence that he was cited by continental and analytical philosophers and even computer scientists alike. To learn more about Davidson's life I recommend to read Lepore's 'Interview with Donald Davidson' [-@Lepore:2004id] and Davidson's own 'Intellectual Autobiography' [Davidson:1999ia]



### Historical Context
<!--
- Vienna Circle and Empiricism
- Wittgenstein and the social aspect of language
- Quine and the new non-empiricist analytical philosophy
- brief overview of players
-->

Language has been a philosophical topic since Plato, but it especially gained attention in the so-called 'Linguistic Turn' of the 20th century, when it was recognized as the medium for our rational access to the world. Names like Frege, Russel, the early Wittgenstein, and the Vienna Circle stand for the earlier Ideal Language Philosophy and Logical Empiricism which hoped to solve problems of Metaphysics through a *definite logical analysis* of meaning. However, This approach did not turn out very successful. Led by Austin, Ryle, and the late Wittgenstein analytical philosophy paid more attention to Ordinary Language, focusing on the importance of *social and performative aspects*. Quine and Davidson stand at the resolution of this tension with an approach that recognizes linguistic behavior in its context while leveraging the formal methods for their analysis. [@Bertram:2011sz] Through Davidson the analytical tradition also became linkable to the 'continental' Hermeneutic traditions, contributing to the dissolution of the philosophical divide of the 20th century. [@Malpas:2015dd, p. 2]

# The Turing Test and Its Relevance {#section1}






<!--
- the imitation game
- establishing a baseline
-->

Alan Turing (1912--1954) first proposed his famous test in 'Computing Machinery and Intelligence' [-@Turing:1950cm]. The thesis of his paper is that the question "Can machines think?" --- which he deemed too vague to deserve discussion --- can be replaced with the question wether a computer can pass a specified test (that is now known as the 'Turing Test'). This test is described as a game: the imitation game.

The imitation game consists of an *interrogator* who can communicate via a real-time text chat interface with two players. One player is a *computer*, the other a *human*. The interrogator’s task is to identify the human after a given time. The computer's task is to pretend to be a human[^no-sexism] and trick the interrogator into wrongly identifying it as the human. The human's task is to help the interrogator to make the correct identification. If many interrogators consistently[^baseline] can't tell the computer apart from the human the computer wins the game and passes the test. [@Turing:1950cm, p. 433--434]



[^no-sexism]: I think it is pretty clear that Davidson [-@Davidson:1990tt, p. 78] misinterprets Turing when he suggests that Turing wants the computer to play the literal imitation game and pretend to be a *woman* and that the interrogator's task would be to decide on the gender. This becomes pretty clear when Turing says: "If the man were to try and pretend to be the machine [...]" [-@Turing:1950cm, p. 435] and from all his examples that are focused on how the machine can imitate being a *human* not a woman. [See also  @Copeland:2000tt, p. 526.]

[^baseline]: Turing's idea is that a baseline is established by the traditional imitation game, in which a man tries to imitate a woman and the interrogator has to decide on the gender. While this might not be the best way to establish a baseline, it means that Davidson's critique that "Turing does not say what he would make of a computer that was consistently chosen over the [...human] to be the [...human]" [-@Davidson:1990tt, p. 78], is ill-conceived, as the computer will always unambiguously fall over or under the baseline within a margin of error.

<!--
- Overview of this Section
-->

In the following I discuss different interpretations of the Turing Test and establish which interpretation and version of the test I take as the basis for my discussion. Furthermore, I argue for the relevance of this interpretation of the test and work out 4 main claims from Turing's discussion of his test. In doing so I specifically emphasize some of Turing's visionary ideas on how a computer must be programmed to pass the test, that have implications for Davidson's discussion of the test.

## Interpretations and Versions of the Turing Test



<!--
- Interpretation as definition, sufficient conditions, just framework to gather evidence
- two or one player?
- definition of intelligence uninteresting. Focus on application of intelligence
-->

The interpretations are not as straight forward, as it might seem. There are three main interpretations for what it means to pass the Turing Test:

1. The Turing Test is taken as an operational *definition* --- a *sufficient* and *necessary* condition --- of *intelligence*[^intelligence]: Something is intelligent if and only if it passes the Turing Test. [Such an interpretation is for example found in @Millar:1973pi.]
2. The Turing Test is taken as a *sufficient* condition of intelligence: Something is intelligent if it passes the Turing Test. But it is not necessary for something to pass the Turing test in order to be intelligent. [@Davidson:1990tt tends towards this interpretation.]
3. The Turing Test is taken "as a potential source of good inductive evidence for" intelligence: If Something passed the Turing Test one would be *justified* for inductively inferring that it is intelligent. [This interpretation goes back to @Moor:1976at, p. 249, 251.]

The first interpretation and any reading of intelligence in a broader sense are clearly not in line with Turing's ideas. Turing was not interested in a definition of intelligence but in setting a clear goal for further research. In fact I would argue that the third interpretation from Moor does Turing most justice. This becomes fairly clear from the following section of a radio interview [-@Turing:1952ca], which represents Turing's simplest expression of the test:

> “I *don’t want to give a definition of thinking* [...] I don’t really see that we need to agree on a definition at all. The important thing is to try to *draw a line between the properties of a brain, or of a man, that we want to discuss, and those that we don’t.* […] I would like to suggest a particular kind of test that one might apply to a machine. You might call it a test to see whether the machine thinks, but it would be better to avoid begging the question, and *say that the machines that pass are (let’s say) ‘Grade A’ machines*. The idea of the test is that the machine has to try and pretend to be a man, by answering questions put to it, and it will only pass if the pretence is reasonably convincing.” [@Turing:1952ca, p. 466, emphasis added]

Turing clearly describes the imitation game as a test that defines a special *class of computers*, but not as one that defines thinking/intelligence. It is also implicit that he sees the *ability to communicate* as quintessential for human-like intellectual abilities.

The quotation also gives a simplified version of the test, in so far as it removes the second human player. While this might be limiting for a quantitative analysis, it ensures the focus on the main question and removes any undue emphasis on strategy. Davidson proposes the same simplification in his discussion [-@Davidson:1990tt]. He goes even further in proposing that "the interrogator [...should simply] be asked to decide whether or not the object is thinking" [-@Davidson:1990tt, p. 81]. If we assume that any bias against the object's ability to think can be removed (which makes sense for this philosophical discussion), this seems to be the clearest expression of Turing's idea. Therefore, I will follow Davidson and refer to this simplified version in the following.



[^intelligence]: The term 'intelligence' is adopted here purely in reference to Artificial Intelligence. Turing mostly uses the term 'thinking' and Davidson [-@Davidson:1995ct] mostly uses the term 'rationality' to refer to the concept that this thesis is concerned with. I will introduce and explicate the term intellectual competence for this concept in [section 4.1](#linguistic-competence).

## Relevance of the Test and the Turing Principle



<!--
- the challenge of AGI
- How the TT solves the definition problem of AGI
- other tests
- Why the TT is a good test
-->

Where does it leave the relevance of the Turing Test, if we follow Moor and interpret it merely as a framework to gather evidence for human-like intelligence? For Computer Scientists it might be *prudent* to follow Turing and ignore the philosophical question of a definition of intelligence and instead take the Turing Test as a definition of a certain class of computers. In this way the Turing Test can give a clear goal to the field of 'Artificial General Intelligence' (AGI), for which the unclarity about a clear definition of its topic is a core challenge. Unlike other propositions for an operational definition[^agi-tests] of AGI, the Turing Tests provides a clear and well-justified empirical goal. In his analysis Moor argues why the Turing Test is well apt for that:

> "[T]here are two strong arguments why the Turing test is a good format for gathering inductive evidence. First, the Turing test permits direct or indirect testing of virtually all of the activities one would count as evidence for thinking. Secondly, the Turing test encourages severe testing. […T]he computer would be tested in detail over a wide range of subjects […and] the interrogator's goal is to find a refuting instance which gives the computer away.” [@Moor:1976at, pp. 251--252]

Critics of the Turing Test as a goal for AGI mostly fall into two camps. The first point Moor provides is aimed against the first type of critic who suggests the test sets the wrong goal. As Moor argues, communication is a very clear framework to investigate all kinds of thinking. A further practical reason for the relevance of the Turing Test --- that I would add --- is that natural language communication provides a 'gold standard' for completely natural and seamless computer user interfaces. Many of those critics mistake the question as philosophical while it is best treated as definitional. Computer Scientists ought not to be concerned with defining intelligence in general but with a good definition for "Grade A" computers --- to use Turing's terminology. In this regard, the interpretation of the Turing Test as a framework to gather empirical evidence can be set as a clear definition of the goal of AGI.


The other type of critic questions the adequacy of the test to determine whether the goal is reached. Moor's second point is aimed against that by pointing out how well the test encourages thorough testing. The critics sometimes mistake Turing's predictions as a specification that the test ought to take only 5 minutes and limited implementations of the Turing Test that favor engineering tricks like the Loebner Prize[^loebner-critique] discredit Turing's intentions. I agree with Copeland's interpretation of Turing: the goal set by the test is a computer that "plays the imitation game successfully come what may, with no field of human endeavour barred, and for any length of time commensurate with the human lifespan." [@Copeland:2000tt, p. 530]



[^agi-tests]: See @Muehlhauser:2013wa for a brief overview of operational definitions of AGI, including the Coffe-Brewing and College Test. From a philosophical perspective all those seem rather random and dubious --- certainly much further away from clearly capturing necessary conditions of human-like intellectual competences.

[^loebner-critique]: Shieber [-@Shieber:1994lr] criticizes the Loebner prize for its inappropriateness to award advances in natural-language-processing techniques instead of engineering tricks oriented to the exigencies of the restricted task like parrying and insertion of random typing errors. But the setup of the scoring system alone shows how pointless it is to even judge current systems by a direct Turing Test.

### Turing's three main claims
<!--
- Turing supports the fact that a universal computer can simulate every physical process including the brain. (also known as the Turing Principle, Wikipedia)
- Turing believes that communication is a suitable means to expose the relevant intellectual abilities that determine wether a machine can think.
- Turing thinks the imitation game specifically is suited to test the communicative abilities of the computer.
-->

Following Copeland [-@Copeland:2000tt, p. 530], we can establish the following two main claims of Turing from our previous discussion:

1. Turing sees communication as suitable to expose the relevant intellectual abilities that determine wether a computer can perform tasks on paar with a human being.
2. Turing thinks that his test *specifically* can determine wether a computer possesses such communicative abilities.

But there is also a third claim which is known as the Turing Principle[^turing-thesis]:

3. Turing believes that universal computers can simulate any physical process, including the brain.

This might be most clearly expressed in Turing's lecture on 'Can Digital Computers Think?': "If it is accepted that real brains [...] are a sort of machine it will follow that our digital computer suitably programmed will behave like a brain" [@Turing:1951cd, p. 463]. This is a much more controversial claim and --- as Turing was well aware --- he had few arguments and even less evidence for it.

It is important to highlight that this claim is not central in Turing's writing and that it is separate and fully *independent* from the others claims. Nevertheless, it is the main point many philosophers  have attacked. [The most famous example is probably @Searle:1980mb.] This is often tied to the misinterpretation of the Turing Test as a definition or sufficient condition for intelligence in a philosophical sense. I am not particularly interested in the discussion of this third claim here.


[^turing-thesis]: This is also known as the 'Church–Turing–Deutsch Principle' and represents an extension of the well-known Church-Turing Thesis to artificial intelligence.

## Turing on Machine Learning

<!--
- Move from AGI to AI and Machine Learning
- Turing's (wrong) predictions
- Loebner Prize state
- 1952 predictions
- success through NN scale
-->

Unlike the obsession in popular culture with human-like 'Artificial Intelligence' (AI) might suggest, the interest of Computer Scientists in the last years has been more focused on so-called 'weak' AI. This refers to applying 'Machine Learning' to apply domain-specific intelligence to special problems (most notably: image recognition, domain-specific language processing, and robotics). The field that is concerned which this is referred to as 'Artificial Intelligence' these days. The field that is concerned with human-like strong AI is the field of Artificial General Intelligence (AGI) which was referenced in the previous section. This shift of focus has mainly been due to a lack of success in AGI.

Turing believed that by the turn of the century there would be computers that "play the imitation game so well that an average interrogator will not have more than 70 per cent chance of making the right identification after five minutes of questioning" [-@Turing:1950cm, p. 442]. Recent winners of the Loebner Prize [@AISB:2015lp], which is awarded to the most human-like chatbot judged by a Turing-inspired test, show that this has not quite come to pass. On the other hand, Turing himself said that it would take "*at least* 100 years" [-@Turing:1952ca, p. 434] until a general Turing Test could be passed --- and the goal of AGI reached --- which is still well within the realm of the possible. Turing's wrong prediction of the development can be mainly accredited to his underestimation of the required processing power for Machine Learning [-@Turing:1950cm, p. 455]. Recent accomplishments in AI with deep neural networks, for example, have only become feasible because computers are able to run networks with millions of neurons in real time.[^nn-size]



[^nn-size]: Steven Wolfram writes: "Computers (and especially linear algebra in GPUs) got fast enough that [...] it became practical to train neural networks with millions of neurons, on millions of examples. [...T]his suddenly brought large-scale practical applications within reach. [...] I don’t think it’s a coincidence that this happened right when the number of artificial neurons being used came within striking distance of the number of neurons in relevant parts of our brains. [...I]f we’re trying to achieve 'human-like' image identification [...] then this defines a certain scale of problem, which, it appears, can be solved with a 'human-scale' neural network." [-@Wolfram:2015ii]

### Turing's fourth main claim
<!--
- child mind with learning ability
- sensory organs
- interaction with teacher
- Helen Keller example
- reverse engineering approach to AI with neural networks most successfull
- Machine Learning
- 4th core claim from Turing
-->



However, Turing's idea about *how* to build a computer that could pass his test are more interesting than his timeline predictions. His claim that "the problem [of building a computer that passes the Turing Test] is mainly one of programming" [-@Turing:1950cm, p. 455] still rings true today.

We have already learned of his idea that computers should be able to simulate the brain [-@Turing:1951cd]. Indeed this reverse engineering approach to AI is the basic idea behind the neural networks which power the most successful image entity-recognition algorithms today and was already investigated by @Turing:1948im [see also @Copeland:1999at]. It seems plausible that we might achieve AGI through brain simulation before we deeply understand how the brain works.

Even more interesting is that Turing also predicted the Machine Learning approach to build intelligent algorithms and saw its non-deterministic nature as a characteristic feature:

> "Instead of trying to produce a programme to simulate the adult mind, why not rather try to produce one which simulates the child's? If this were then subjected to an appropriate course of education one would obtain the adult brain. [...] We have thus divided our problem into two parts. The child-programme and the education process. These two remain very closely connected. We cannot expect to find a good child-machine at the first attempt. One must experiment with teaching one such machine and see how well it learns." [@Turing:1950cm, p. 456]
>
> "An important feature of a learning machine is that its teacher will often be very largely ignorant of quite what is going on inside, although he may still be able to some extent to predict his pupil's behaviour. [...] This is in clear contrast with normal procedure when using a machine to do computations : one's object is then to have a clear mental picture of the state of the machine at each moment in the computation. [...] Processes that are learnt do not produce a hundred per cent certainty of result; if they did they could not be unlearnt." [@Turing:1950cm, p. 458-459]

This description is very much how modern statistical Machine Learning algorithms work. They consist of an algorithm that describes a mathematical model which is trained with human-annotated data (for example, a grammar analysis of sentences) and are then able to perform their task on similar data. [See @Schubert:2015cl for an overview about approaches to Natural Language Processing; and @Jurafsky:2015uu for a more technical introduction.] As Turing mentions, this is a paradigm shift from classical algorithms which have results that are clearly defined by the programmer and predictable independent of any training data. We might add a fourth core claim:

4. Turing believes that the approach to device intelligent computers must be based on learning algorithms that are trained and do not behave predictable in a classic sense.

Note that devising intelligent algorithms is a quite different task and involves techniques where an interpretation of the state of the program at each step becomes difficult or even impossible --- especially in the case of deep neural networks. And where the outcome is not just dependent on the set of rules specified in the programming but also on the 'experience' gathered in the program during its learning process. We will see later why this matters for a Davidsonian perspective.

### Summary
<!--
- We are right in taking the simplified version of the test as the purest expression of Turing's idea
- The tests relevance is mainly that it provides the clearest answer to what AGI is about.
- Turing has rightly identified the main question of research in AGI to be about how a machine can learn to communicate.
- independence of the Turing principle from his other more interesting claims.
- The nature of Machine Learning.
-->

We have seen that a simplified interpretation of the Turing Test as proposed by @Davidson:1990tt reveals the core of Turing's idea. However, we have also seen that an interpretation of the Turing Test as an operational definition or sufficient condition for intelligence is not in line with Turing's writing. Instead, I have proposed to follow @Moor:1976at and interpret the test as a framework to collect empirical evidence to show that a computer can perform human-like tasks. We have seen that this can provide a good and clear definition of a special class of computers that are the goal of AGI research.

Furthermore, we have established that Turing claims that (1) communication abilities are representative of intellectual abilities in general and (2) that his test is adequate to evaluate those abilities. I have pointed out that his claim (3) that computers can simulate the brain (the Turing Principle), which is the main point most philosophers critique, is completely independent of the other claims and is the least essential one for Turing.

Lastly, we have seen that Turing had pioneering ideas about how to devise algorithms which could pass his test. Such algorithms (4) need to be able to learn when trained with data and, different from classical algorithms, their outcome is not predictable independent of their 'experience' and the states of their operation are not easily interpretable.





# Davidson's Critique of the Turing Test {#section2}



<!--
- Overview of this section
-->

In this section I will first discuss the relevance of the Turing Test for Philosophy of Mind and for Davidson specifically. I will then argue where Davidson agrees with Turing, where his criticism of Turing applies, and in how far I think this criticism does Turing justice. The section ends in an exposition of Davidson's proposal for a modified Turing Test.

## Relevance of Turing's Test for\ Davidson's\ Philosophy\ of\ Mind


<!--
- Test is concerned with the nature of thought
- Not confined to machines
- Pragmatic approach to the question of thought
- Empiric criterion for thought
- There should be an empiric test for intellect
- good introduction to Davidson's ideas
-->

I have argued that the Turing Test is misunderstood as a definition or sufficient condition for thought in general and merely provides a pragmatic goal for AGI research. But why should it be relevant to Philosophy of Mind then? Davidson says "the test is designed to throw light on the nature of thought [...and it] can be applied to any object" [-@Davidson:1990tt, p. 78]. While Davidson might be interpreting the test more like a sufficient condition for though, his statement also reveals another more important aspect that is echoed by Turing:

> "The whole thinking process is still rather mysterious to us, but I believe that the attempt to make a thinking machine will help us greatly in finding out how we think ourselves." [@Turing:1951cd, p. 465]

So the Turing Test and the related task of constructing a machine which can pass it, is a practical device to learn more about the nature of thought and communication. This resonates very much with Davidson's philosophy. For the essential paradigm shift of his philosophy about language is following Quine's rejection of Carnap's Logical Empiricism[^empiricism]. The objective of a theory of meaning for Davidson "is sought not in reductive analyses [of the meaning of expressions], but rather in showing how evidence can be marshalled in support of a theory of interpretation for a speaker." [@Lepore:2009d, p. 9] Philosophy is not an a priori discipline like mathematics but simply a more general empirical discipline. "'Language is a social art' [...and] evidence for its acquisition and deployment must be intersubjective, and, hence, recoverable from overt behaviour" [@Lepore:2009d, p. 22--23]. Therefore the search for a definition of meaning or of intelligence is rather uninteresting. It is replaced by the pragmatic search for an empirical theory that is judged by its successful application.

From this angle the task of programming a machine which can pass the Turing Test, becomes essentially the same as that of devising and testing an empirical theory of interpretation. At least if we accept that such a theory of interpretation could be expressed recursively. Then judging a computer as passing the test is not so different from judging a person. Moor argues:

> “I believe that another human being thinks because his ability to think is part of a theory I have to explain his actions. [...T]he evidence for the theory comes from the outward behavior of the person. [...T]here is no reason why knowledge of computer thinking can not arise in the same way. I can use the computer's behavior as evidence in assessing my theory about its information processing.” [@Moor:1976at, p. 251]

Davidson and Turing agree that we can devise a scientific theory that describes the essential parts of our linguistic competence. In the case of Turing this is evident in his believe that there is a program that allows the computer to win the imitation game. For Davidson it is evident in the proposal of his Unified Theory which can capture the essence of linguistic competence and rationality --- this is discussed further in [section 4](#section 4).

So we have seen why *Davidson* finds Turing's Test particularly interesting. *I* have chosen his critique for discussion here, since it clearly relates to Computer Science and because it "opens the way for Davidson's own view into the nature of thought" [Cavell:2004i, p. xvii].



[^empiricism]: For historical reasons, the terminology here is easily confusing: The term 'Empiricism' ought to be treated very carefully as distinct from empirical. Davidson's theory is empirical, meaning observable evidence plays an important role in it, but it disagrees with the dogmas of Logical Empiricism (sometimes also called Logical Positivism), namely the analytic-synthetic distinction and reductionism [@Quine:1951td] and the dualism of scheme and content [@Davidson:1973vi]. Davidson replaces the concepts of meaning and proximal stimuli by a holistic and empirical theory which treats language and knowledge as elementary intersubjective. [@Lepore:2009d, p. 22--23]



### Linguistic abilities as the essence of Intelligence
<!--
- Davidson agrees with Turing's first claim
- Justification by Davidson's Epistemology (and Metaphysics)
- Davidson rejects Turing's second claim and modifies it
- Davidson also finds Turing's third claim (the Turing Principle) uninteresting but tends to agree (related to his ontology)
- Davidsons critique ignores Turing's fourth claim but the content of his critique is actually related to it, as we will see later.
-->

What we have discussed so far depends on accepting Turing's first claim that communication abilities are representative of intellectual abilities. As mentioned in the introduction, Davidson agrees since he "sees our nature as linguistic beings as the key to the possibility of thought" [@Lepore:2009d, p. 1]. This believe springs from his metaphysics[^metaphysics] and from his Epistemology. The later will be examined in more detail in [section 3.5](#triangulation). However, Davidson emphasizes the interrogator's judgement as the essential point:

> "Turing was right, in my opinion, in taking as the only test for the presence of thought and meaning the interpretive powers and abilities of a human interpreter." [@Davidson:1990tt, p.86]

The second claim is what Davidson discusses and criticizes extensively and which I will discuss in the next subsection.

The third claim is not of particular interest to Davidson, but because of his naturalistic ontology[^ontology] he agrees: "A person is a physical object which [...] functions according to physical laws. So [...] there is no reason why an artificial object could not think" [-@Davidson:1990ri, p. 87].

The fourth claim is something Davidson does not pay much attention to. It is only mentioned in his last footnote where he claims that Turing "views this simply as an economical way of producing a device with mature thoughts; he does not see it as the only way" [-@Davidson:1990tt, p.86]. As outlined in the previous section, I think this is overestimating Turing's interest in sufficient conditions for intelligence and underestimating his importance in pioneering those ideas in Machine Learning which take up a third of his essay [@Turing:1950cm, pp. 454--460]. This is relevant because Turing's fourth claim is closely related to Davidson's own critique --- probably the reason why Davidson mentions it at the footnote at the end of his essay.


[^metaphysics]: Davidson argues that: "If we have the semantics of a language right, the objects we assign to the expressions of the language must exist" [@Davidson:1993mm, p. 40]. Since we need to get semantics pretty right to be able to communicate. This will in turn also mean, that if we can communicate, we get it pretty right what things are in the world and in which relation they stand to each other. And this certainly seems to be a sufficient condition for intelligence. Davidson's argument for his claim is based on the fact that we must get things mostly right about the world, if we are intelligible as rational beings at all.

[^ontology]: Davidson's ontology consists only of objects and events [-@Davidson:1991tv]. He rejects the need for any propositions of proximal stimuli in the mind [-@Davidson:1990mt]. The content of propositional knowledge is directly caused by the objects and events the world is made up of.

## Davidson's Critique of the Turing's Test
<!--
**Davidson's core criticism: knowledge comes from interaction in shared world**
- No need for introspection into working of mind (against Searle's chinese room)
- Rejection of sharp distinction between mental and physical (especially sensory) abilities (E4.5)
- distinction between semantic and syntactic abilities
(+E5.8)
- Relation to Agreement between Descartes and Turing
  - Both come from the idea that knowledge is simply in the head
- Even Turing's Helen Keller example lacks as she was interacting with the world through touch.
- Connected to rejection of Cartesion Epistemology
- relation to French (1990)
-->

Davidson finds Turing's Test inadequate to show that an object is thinking. Not because communication is not a sufficient criterion for intellectual competence for Davidson as we have discussed. Neither because a test would require an introspection into the workings of the mind. Davidson explicitly says that it is not inadequate because it "restricts the available evidence to what can be observed from the outside" [-@Davidson:1990tt, p.83]. But because it does not enable the interrogator to observe a history of three-way engagement between the object, a shared world, and other minds in which the object develops its semantics.


**Does Davidson's Critique Do Justice to Turing?**
- Davidson has a good point
- but he doesn't do justice to Turing's thoughts on Machine Learning that would deserve a discussion in his paper
- His emphasis on a history of causal interaction with the world is partly satisfied by machine learning

### Appropriateness of the Critique


## Davidson's Proposal for a Modified Test

**Observe a History of interaction with the world**
- The ability to determine non predefined meaning is essential for intelligence





**Summary**



# Necessary Conditions for Linguistic\ Competence {#section3}







## The Distinction between Linguistic\ Competence\ and\ Performance {#linguistic-competence}


**Distinction between sufficient and necessary conditions of linguistic competence**
- relation to term linguistic competence and linguistic performence
- analogy to physics not being able to describe actual natural systems but only systems under ideal conditions
- Davidson's transition from a formal (logical/mathematical) theory of meaning (that describes how to derive meaning) to an empirical theory of meaning (that judges interpretation as evidence) is essential here.
- See (E4.8, E5.8)



I use the term *linguistic competence*[^linguistic-competence] here to refer to Davidson's idea of the essential aspect of understanding language vs. the practical understanding of language.


[^linguistic-competence]: The term linguistic competence was introduced by Chomsky who makes a "fundamental distinction between competence (the speaker-hearer's knowledge of his language) and performance (the actual use of language in concrete situation)" [@Chomsky:2014at, p. 4]. While Davidson  criticizes the idea of linguistic competence as knowledge of a language, he adopts the term for the description of his theory that describes the interpreters essential competence in 'A Nice Derangement of Epitaphs' [-@Davidson:1986nd].



**Relation to Davidson's Philosophy**
- truth conditions as a formal language
- Unified Theory, Radical Interpretation
- Sucessfull Communication & Anti-Conventionalism & Holims of knowledge





## Recursiveness and Empirism {#recursiveness}


**The Importance of Empirical Theories**
- No a priori knowledge about language(-learning), only empirical knowledge (E2.1)



**Learnable Languages**
- Finite set of linguistic primitives gives rise to infinite linguistic expressions

'Theories of Meaning and Learnable Languages' [@Davidson:1965tm]



## The Social Aspect of Language {#social-language}


**The Primacy of Ideolect**
- relevance of interpretation rather than meaning (+E2.2)
  - see similarities to Gadamer's Hermeneutics of Wirkungsgeschichte (Bertram 2012)
- Relevance of Intention in communication (+E5.10)
- Arguments for primacy of ideoloect over language
  - Malapropisms and the like (E5.7)







**Why is language necessarily Social**
- Wittgenstein's norm of actually getting it right in language
  - also see language game analogy in anti conventionalism (2.18)
  - and importance of disctinction between true and false beliefs in triangulation (E3.14)
- Truth only determined trough communication
  - see also Plato, socrates (E5.16)













## Anti-Conventionalism {#anti-conventionalism}


**arguments against conventionalism**
- impossibility of public sign for sincerity
- language game analogy (+E5.8)





**Remarks about how understanding does work**
- At the end of [-@Davidson:1984cc], Davidson says that understanding can't be formally described
- Relation to distinction linguistic between competence and prerformence



## The Triangular Nature of Knowledge {#triangulation}




**The basic problem of Epistemology**
- Distinctiveness of three types of Knowledge (subjective, intersubjective, objective) (E3.14)
- Three Questions of Epistemology (E3.14)
  - how to know other minds
  - how to know world
  - how to know own mind without evidence





**Rejection of other Epistemologies**
- Rejection of Positivism (reductionism to world knowledge) (E3.14)
- Rejection of empiricsit Epistemology (E3.14, E2.1)
  - No primacy of names and predicates in the foreground of senses
  - doesn't he contradict that in E2.9 and E4.8?
- Rejection of Cartesion Etymology (primacy of knowledge of one's own mind) (E3.14, E3.3, E3.13)
  - Rejection of skepticism (E3.14, SEP Davidson, E4.1)







**The Process of Gaining Knowledge**
- Interdependency of three varieties of Knowledge
- Importance of disctinction between true and false beliefs (E5.8, E3.14, E4.1, SEP Davidson)
- Principle of Charity (Coherence and Correspondence)
(E3.14, E2.9, E3.14)
- Reaction to stimuli (E3.14)
  - proximal vs. distal stimuli (E5.4)
- Iscrutability of Reference / Indeterminacy of meaning (Quine Word and Object, E5.3, E2.16, E3.14)











**The Underlying Ontology and Metaphysics**
- Ontology of only objects and events (E3.14, E5.4)
- Directness of knowledge of world
  - no intermediary entities (5.3, E5.4, E3.10)
  - no mentales, language only through communication, meaning given causally by objects events (E5.9)
- Truth as elementary non-reducible concept (E5.2, E2.I)



**Anomalous Monism**
- parallels to Spinoza's causal theory of affects (E5.20)
- see arguments for irreducibility of mental in Tirangulation (E3.14)
- Reasons for Irreducibility/anaomalism of Mental to Physical (E3.14, E4.8)
  - Irreducibility of knowledge of belief to knowledge of world
  - causal nature of the mental (+E1.11, E4.8)
  - Missing independent mode of communication about mental theories (+E4.8)
- Turing's discussing of rule based behavior




Turing discusses an interesting objection to his test that is related to Anomalous Monism [-@Turing:1950cm, p 452f]. If our behavior is not ruled by strict laws but a computer is. How could it ever simulate our behavior. Turing argues that this is simply an assumptions (and even if who says that the mental states of a computer could for example not supervene on the sates of its neural network). Turing uses cryptography as an example for a process where a computer can produce output which can not be tracked back to its originating rules (but this of course is a practical limitation not a theoretical one, since all cryptographic functions can be reversed with infinite processing power.)

This raises and important question wether the anomalism of the mental is connected to our linguistic competences (or maybe just to our effectiveness?) and how computers/the unified theory could account for it.
[ ] **Reread in three varieties of knowledge to see what this means**

**Summary**


# Davidson's Theory of Intellectual and\ Linguistic\ Competence {#section4}







## Sources for Davidson's Theory of Intellectual and Linguistic Competence

**What is this theory of interpretation**
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

## Outline of the Unified Theory of Meaning and Action

**Decision Theory **

Sprang from his early times at Stanford when collaborating with Patrick Suppes and JJC McKinsey. [@Lepore:2009d, p. 2]

**Representation of Meaning/Linguistic Content**
- Meaning as Language (E3.14, E2.2) (not things in world, not entities sui generis)





**How does the interpretation Process work**

## Relation to Davidson's Test

**Interpreting Davidson's Test as a Test for a Unified Theory 'machine'**



**Summary and Conclusion**

## Possible Objections against Davidson's Test

**Behaviorism**

**Mechanism**

**Scope of the Test**

**Blockheads**

**The Chinese Room (Internal Operation)**

**French: Associative Priming and Rating Games**



**Ability to cope with Abstract Terms**

- It remains unclear how well Davidson's theory might be able to cope with abstract terms in the language.
- He throws very little light on how understanding of abstract terms might work.
- There are good reason's to doubt that communication about abstract terms can work in the same way as other communication. Something like the Wirkungsgeschichte becomes way more plausible, if we look at how culturally loaded language is
- See also Bertram's critique: Gadamer's idea

[@Bertram:2012ta]
[@Davidson:1997gp]




**Wirkungsgeschichte**

# Conclusion {-}








## Prospects of Davidson's Pragmatic Theory {-}




While Davidson is skeptical about the possibility of explaining our linguistic performance. He believes that there is a pragmatic and empirical theory about the essence of linguistic competence.

## Implications for Artificial Intelligence and Computer Linguistics {-}






Davidson tries to device a theory that can model human intellectual abilities in an empiric theory that has the power to explain them. (As opposed to only a simulation of the brain by a machine)

While it currently seems more probable that Turing’s Test and also Davidson’s Test will be passed by a computer that leverages trained large scale deep neural networks aka. something into the direction of simulating the brain. Davidson’s consideration still provide important input into what is needed to achieve human level of natural language abilities. That is the ability to somehow interact with the world and have some sensory impression of it and have a triangular model of determining world interaction.

**Possibility of AI and the importance of Language**
- Davidson sees artificial intelligence as possible.
- He agrees that language is the key test for intelligence.
- Davidson and Turing agree that the task is not to explain human linguistic practice, but create an empirical theory that models the essence of linguistic competence. This is a very important philosophical distinction that should be understood very well in order to build language processing systems and not get distracted with the wrong problems.



**Important boundary conditions for linguistic competence**
- Linguistic and intellectual competence are inherently social/intersubjective
- Linguistic and intellectual competence require interaction with the shared world (empiric)





**Denial of conventionalism and statistical linguistics**
- The social and empiric traits of linguistic and intellectual competence can not be modeled by conventionalism, if this convention requires a previously shared common practice. Interpretation emerges in the instance of communication and cannot be predetermined in anyway.
- Abilities of linguistic interaction can not be clearly separated from abilities for physical interaction. Both are necessary for intelligence.







# Acknowledgements {-}

Many thanks to ... for reading this paper ...

### Colophon

This paper was written with [Gingko](https://gingkoapp.com) in [Pandoc Markdown](http://pandoc.org) and typeset using [XeTeX](http://xetex.sourceforge.net) in Gotham Narrow. My research process is inspired by Luhmann's Zettelkasten methodology, using [Evernote](https://evernote.com). If you are interested, you can find an article about my research and writing process on my blog (<http://MrLoh.se/2015/10/research-and-scientific-writing-process>).

# References {-}


