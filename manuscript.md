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

This paper discuses Donald Davidson's critique [-@Davidson:1990tt] of the Turing Test as an illustration of Davidson's theory of linguistic and intellectual competence. After a short Introduction to Donald Davidson it consists of three main sections.

[**Section 1**](#section1) explores Turing's original ideas and their relevance. It discusses different interpretations and versions of the Turing Test and establishes wich interpretation I follow. It also contains a discussion of the significance of the test and Turing's ideas about Machine Learning for the field of Artificial (General) Intelligence.

[**Section 2**](#section2) presents and evaluates where Davidson agrees and disagrees with Turing. It also presents Davidson's modified version of the Turing Test which allows to judge the computer based on an observation of its learning process. I argue that this test acts as a definition for intelligence and expression of Davidsons theory of linguistic and intellectual competence.

[**Section 3**](#section3) delves deeper into Davidson's theory by looking at its parts: reconstructing his argument for supervenience of the mental, exposing his epistemology of triangular knowledge, and describing his empirical anti-conventionalist theory of interpretation. It shows how those elements come together as a unified theory about the essence of linguistic and intellectual abilities that constitute Davidson's definition of rationality or intelligence that is incorporated in Davidson's Test. After that I discuss how Davidson's Test fences against some classical objections against the Turing Test and some other concerns.

[I conclude][Conclusion] with a summary of the core agreements and distinctions between Davidson and Turing and a brief discussion of the implications of Davidson's ideas (holistic theory and anti-conventionalism) for Computer Linguistic and Machine Learning approaches that might deserve further investigation.



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

    Davidson's life and career are actually quite inspiring, *fascinating*, and unconventional. Davidson started out in the History of Philosophy and ventured into psychology and economy during his studies and as a professor. Certainly it is no coincidence that he was cited by continental and analytical philosophers and even computer scientists alike. To learn more about Davidson's life I recommend to read Lepore's 'Interview with Donald Davidson' [-@Davidson:2004id] and Davidson's own 'Intellectual Autobiography' [Davidson:1999ia]





### Historical Context
<!--
- Vienna Circle and Empiricism
- Wittgenstein and the social aspect of language
- Quine and the new non-empiricist analytical philosophy
- brief overview of players
-->

Language has been a philosophical topic since Plato, but it especially gained attention in the so-called 'Linguistic Turn' of the 20th century, when it was recognized as the medium for our rational access to the world. Names like Frege, Russel, the early Wittgenstein, and the Vienna Circle stand for the earlier Ideal Language Philosophy and Logical Empiricism which hoped to solve problems of Metaphysics through a *definite logical analysis* of meaning. However, This approach did not turn out very successful. Led by Austin, Ryle, and the late Wittgenstein analytical philosophy paid more attention to Ordinary Language, focusing on the importance of *social and performative aspects*. Quine and Davidson stand at the resolution of this tension with an approach that recognizes linguistic behavior in its context while leveraging the formal methods for their analysis [@Bertram:2011sz]. Through Davidson the analytical tradition also became linkable to the 'continental' Hermeneutic traditions, contributing to the dissolution of the philosophical divide of the 20th century. [@Malpas:2015dd, p. 2]

# The Turing Test and Its Relevance {#section1}





<!--
- the imitation game
- establishing a baseline
-->

Alan Turing (1912--1954) first proposed his famous test in 'Computing Machinery and Intelligence' [-@Turing:1950cm]. The thesis of his paper is that the question "Can machines think?" --- which he deemed too vague to deserve discussion --- can be replaced with the question wether a computer can pass a specified test (that is now known as the 'Turing Test'). This test is described as a game: the imitation game.

The imitation game consists of an *interrogator* who can communicate via a real-time text chat interface with two players. One player is a *computer*, the other a *human*. The interrogator’s task is to identify the human after a given time. The computer's task is to pretend to be a human[^no-sexism] and trick the interrogator into wrongly identifying it as the human. The human's task is to help the interrogator to make the correct identification. If many interrogators consistently[^baseline] can't tell the computer apart from the human the computer wins the game and passes the test. [@Turing:1950cm, p. 433--434]



[^no-sexism]: I think it is pretty clear that Davidson [-@Davidson:1990tt, p. 78] misinterprets Turing when he suggests that Turing wants the computer to play the literal imitation game and pretend to be a *woman* and that the interrogator's task would be to decide on the gender. This becomes pretty clear when Turing says: "If the man were to try and pretend to be the machine [...]" [-@Turing:1950cm, p. 435] and from all his examples that are focused on how the machine can imitate being a *human* not a woman. [See also  @Copeland:2000tt, p. 526.]

[^baseline]: Turing's idea is that a baseline is established by the traditional imitation game, in which a man tries to imitate a woman and the interrogator has to decide on the gender. While this might not be the best way to establish a baseline, it means that Davidson's critique that "Turing does not say what he would make of a computer that was consistently chosen over the [...human] to be the [...human]" [-@Davidson:1990tt, p. 78], is ill-conceived, as the computer will unambiguously fall over or under the baseline within a margin of error.

<!--
- Overview of this Section
-->

In the following I discuss different interpretations of the Turing Test and establish which interpretation and version of the test I take as the basis for my discussion. Furthermore, I argue for the relevance of this interpretation of the test and work out 4 main claims from Turing's discussion of his test. In doing so I specifically emphasize some of Turing's visionary ideas on how a computer must be programmed to pass the test, that have implications for Davidson's discussion of the test.

## Interpretations and Versions of the Turing Test {#test-interpretations}




<!--
- Interpretation as definition, sufficient conditions, just framework to gather evidence
- two or one player?
- definition of intelligence uninteresting. Focus on application of intelligence
-->

The interpretations are not as straight forward, as it might seem. There are three main interpretations for what it means to pass the Turing Test:

1. The Turing Test is taken as an operational *definition* --- a *sufficient* and *necessary* condition --- of *intelligence*[^intelligence]: Something is intelligent if and only if it passes the Turing Test. [Such an interpretation is for example found in @Millar:1973pi.]
2. The Turing Test is taken as a *sufficient* condition of intelligence: Something is intelligent if it passes the Turing Test. But it is not necessary for something to pass the Turing test in order to be intelligent. [@Davidson:1990tt takes this interpretation.]
3. The Turing Test is taken "as a potential source of good inductive evidence for" intelligence: If Something passed the Turing Test one would be *justified* for inductively inferring that it is intelligent. [This interpretation goes back to @Moor:1976at, p. 249, 251.]

The first interpretation and any reading of intelligence in a broader sense are clearly not in line with Turing's ideas. Turing was not interested in a definition of intelligence but in setting a clear goal for further research. In fact I would argue that the third interpretation from Moor does Turing most justice. This becomes fairly clear from the following section of a radio interview [-@Turing:1952ca], which represents Turing's simplest expression of the test:

> “I *don’t want to give a definition of thinking* [...] I don’t really see that we need to agree on a definition at all. The important thing is to try to *draw a line between the properties of a brain, or of a man, that we want to discuss, and those that we don’t.* […] I would like to suggest a particular kind of test that one might apply to a machine. You might call it a test to see whether the machine thinks, but it would be better to avoid begging the question, and *say that the machines that pass are (let’s say) ‘Grade A’ machines*. The idea of the test is that the machine has to try and pretend to be a man, by answering questions put to it, and it will only pass if the pretence is reasonably convincing.” [@Turing:1952ca, p. 466, emphasis added]

Turing clearly describes the imitation game as a test that defines a special *class of computers*, but not as one that defines thinking/intelligence. It is also implicit that he sees the *ability to communicate* as quintessential for human-like intellectual abilities.

The quotation also gives a simplified version of the test, in so far as it removes the second human player. While this might be limiting for a quantitative analysis, it ensures the focus on the main question and removes any undue emphasis on strategy. Davidson proposes the same simplification in his discussion [-@Davidson:1990tt]. He goes even further in proposing that since "we might count an object as thinking even if it were easily distinguishable from a person. [...T]he interrogator [...should simply] be asked to decide whether or not the object is thinking" [-@Davidson:1990tt, p. 81]. If we assume that any bias against the object's ability to think can be removed (which makes sense for this philosophical discussion), this seems to be the clearest expression of Turing's idea. Therefore, I will follow Davidson and refer to this simplified version in the following.



[^intelligence]: The term 'intelligence' is adopted here purely in reference to Artificial Intelligence. Turing mostly uses the term 'thinking' and Davidson [-@Davidson:1995ct] mostly uses the term 'rationality' to refer to the concept that this thesis is concerned with. I will introduce and explicate the term intellectual competence for this concept in \autoref{theory}.

## Relevance of the Test and the Turing Principle {#test-relevance}




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

[^loebner-critique]: @Shieber:1994lr criticizes the Loebner Prize for its inappropriateness to award advances in natural-language-processing techniques instead of engineering tricks oriented to the exigencies of the restricted task like parrying and insertion of random typing errors. The setup of the scoring system alone shows how pointless it is to even judge current systems by a direct Turing Test. He argues that a subjective award modeled after the Nobel Prizes would make significantly more sense.

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

## Turing on Machine Learning {#turing-learning}


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

### Turing's fourth main claim {#fourth-claim}

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

We have already learned of his idea that computers should be able to simulate the brain [-@Turing:1951cd]. Indeed this reverse engineering approach to AI is the basic idea behind the neural networks which power the most successful image entity-recognition algorithms today. @Turing:1948im pioneered  this approach with his B-type unorganized machine which consisted of neurons that are trained through an 'education' process, and he proved that they were equivalent with digital computers [see also @Copeland:1999at]. It is plausible that we might achieve AGI through brain simulation before we even deeply understand how the brain works.

Even more interesting is that Turing also predicted the Machine Learning approach to build intelligent algorithms and saw its non-deterministic nature as a characteristic feature:

> "Instead of trying to produce a programme to simulate the adult mind, why not rather try to produce one which simulates the child's? If this were then subjected to an appropriate course of education one would obtain the adult brain. [...] We have thus divided our problem into two parts. The child-programme and the education process. These two remain very closely connected. We cannot expect to find a good child-machine at the first attempt. One must experiment with teaching one such machine and see how well it learns." [@Turing:1950cm, p. 456]
>
> "An important feature of a learning machine is that its teacher will often be very largely ignorant of quite what is going on inside, although he may still be able to some extent to predict his pupil's behaviour. [...] This is in clear contrast with normal procedure when using a machine to do computations : one's object is then to have a clear mental picture of the state of the machine at each moment in the computation. [...] Processes that are learnt do not produce a hundred per cent certainty of result; if they did they could not be unlearnt." [@Turing:1950cm, p. 458-459]

This description is very much how modern statistical Machine Learning algorithms work. They consist of an algorithm that describes a mathematical model which is trained with human-annotated data (for example, a grammar analysis of sentences) and are then able to perform their task on similar data. [See @Schubert:2015cl for an overview about approaches to Natural Language Processing; and @Jurafsky:2015uu for a more technical introduction.] As Turing mentions, this is a paradigm shift from classical algorithms which have results that are clearly defined by the programmer and predictable independent of any training data. We might add a fourth core claim:

4. Turing believes that the approach to device intelligent computers should be based on learning algorithms that are trained and do not behave predictable in a classic sense.

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

In this section I will first discuss the relevance of the Turing Test for Philosophy of Mind and for Davidson specifically. I will then argue where Davidson agrees with Turing, where his criticism of Turing applies, and in how far I think this criticism does Turing justice. The section ends in an exposition of Davidson's proposal for a modified Turing Test that provides a definition for intelligence.

## Relevance of Turing's Test for\ Davidson's\ Philosophy\ of\ Mind {#relevance-philmind}



<!--
- Test is concerned with the nature of thought
- Not confined to machines
- Pragmatic approach to the question of thought
- Empiric criterion for thought
- There should be an empiric test for intellect
- good introduction to Davidson's ideas
-->

I have argued that the Turing Test is misunderstood as a definition or sufficient condition for intelligence in general and merely provides a pragmatic goal for AGI research. But why should it be relevant to Philosophy of Mind then? Davidson says "the test is designed to throw light on the nature of thought [...and it] can be applied to any object" [-@Davidson:1990tt, p. 78]. While Davidson interprets the test as a sufficient condition for though, his statement also reveals another more important aspect that is echoed by Turing:

> "The whole thinking process is still rather mysterious to us, but I believe that the attempt to make a thinking machine will help us greatly in finding out how we think ourselves." [@Turing:1951cd, p. 465]

So the Turing Test and the related task of constructing a machine which can pass it, is a practical device to learn more about the nature of thought and communication. This resonates very much with Davidson's philosophy. For the essential paradigm shift of his philosophy about language is following Quine's rejection of Carnap's Logical Empiricism[^empiricism]. The objective of a theory of meaning for Davidson "is sought not in reductive analyses [of the meaning of expressions], but rather in showing how evidence can be marshalled in support of a theory[^theory] of interpretation for a speaker." [@Lepore:2009d, p. 9] Philosophy is not an a priori discipline but simply a more general empirical discipline. "'Language is a social art' [...and] evidence for its acquisition and deployment must be intersubjective, and, hence, recoverable from overt behaviour" [@Lepore:2009d, p. 22--23]. Therefore the search for a definition of meaning or of intelligence itself is rather uninteresting. A definition is only relevant as part of an empirical theory that can be judged by its successful application. (I'll talk more about this at the end of this section.) The search for a definition is therefore replaced by the search of an empirical theory of intelligence.

From this angle the task of programming a machine which can pass the Turing Test, seems closely related to that of devising and testing an empirical theory of intelligence. At least if we accept that the essence of such a theory could be expressed recursively. Judging a computer as passing the test is not so different from judging a person as rational being after all. Moor argues:  

> “I believe that another human being thinks because his ability to think is part of a theory I have to explain his actions. [...T]he evidence for the theory comes from the outward behavior of the person. [...T]here is no reason why knowledge of computer thinking can not arise in the same way. I can use the computer's behavior as evidence in assessing my theory about its information processing.” [@Moor:1976at, p. 251]

Davidson and Turing agree that we can devise a scientific theory that describes the essential parts of our linguistic competence. In the case of Turing this is evident in his believe that there is a program that allows the computer to win the imitation game. For Davidson it is evident in the proposal of his Unified Theory which can capture the essence of linguistic competence and rationality. However there are some important distinctions between the nature of these approaches that will be highlighted in \autoref{supervenience}.



[^empiricism]: For historical reasons, the terminology here is easily confusing: The term 'Empiricism' ought to be treated very carefully as distinct from empirical. Davidson's theory is empirical, meaning observable evidence plays an important role in it, but it disagrees with the dogmas of Logical Empiricism (sometimes also called Logical Positivism), namely the analytic-synthetic distinction and reductionism [@Quine:1951td] and the dualism of scheme and content [@Davidson:1973vi]. Davidson replaces the concepts of meaning and proximal stimuli by a holistic and empirical theory which treats language and knowledge as elementary intersubjective. [@Lepore:2009d, p. 22--23]

[^theory]: Davidson moved from his interest in the historic aspect of philosophy to analytical philosophy, because Quine had convinced him "that it was possible to be serious about getting things right in philosophy" and to take philosophy "as serious as science" [@Davidson:2004id, p. 239]. But through the recession of Logical Empiricism it had become clear that this progress could not simply lie in treating philosophy as the logic of mathematics and reasoning. His experiences in studying business, working with J.C.C. McKinsey on decision theory, and studying Tarski, gave Davidson "an appreciation for what it's like to have a serious theory" [@Davidson:2004id, p. 253] and convinced him that the progress of ordinary language philosophy could be found in looking for a pragmatic empirical theory.



### Linguistic abilities as the essence of Intelligence
<!--
- Davidson agrees with Turing's first claim
- Justification by Davidson's Epistemology (and Metaphysics)
- Davidson rejects Turing's second claim and modifies it
- Davidson also finds Turing's third claim (the Turing Principle) uninteresting but tends to agree (related to his ontology)
- Davidsons critique ignores Turing's fourth claim but the content of his critique is actually related to it, as we will see later.
-->

What we have discussed so far depends on accepting Turing's first claim that communication abilities are representative of intellectual abilities. As mentioned in the introduction, Davidson agrees since he "sees our nature as linguistic beings as the key to the possibility of thought" [@Lepore:2009d, p. 1]. This believe springs from his metaphysics[^metaphysics] and from his epistemology. The later will be examined in more detail in \autoref{triangulation}. However, Davidson emphasizes the interrogator's judgement as the essential point:

> "Turing was right, in my opinion, in taking as the only test for the presence of thought and meaning the interpretive powers and abilities of a human interpreter." [@Davidson:1990tt, p.86]

As we will discuss in \autoref{davidsons-test} Davidson very intentionally changes the emphasis here, since he argues that the ability to be interpreted is not a sufficient, but a necessary condition for attributing thought --- introspection into the working of the mind for example is *not* a sufficient condition for Davidson. For Davidson the essence of Turing's approach is that "instead of asking how the content of a concept [...] is thought of by the creature that has the concept [...], we ask [...] how an observer can size up the contents of the thoughts of another creature" [@Davidson:2001wt, p. 137].

The third claim (Turing's Principle) is not of particular interest to Davidson, but because of his naturalistic ontology[^ontology] he agrees: "A person is a physical object which [...] functions according to physical laws. So [...] there is no reason why an artificial object could not think[... . The real question is:] how much like us must an artifact be, and in what ways, to qualify as having thoughts?" [-@Davidson:1990ri, p. 87].

The second claim (the appropriateness of the test) is what Davidson discusses and criticizes extensively in his essay 'Turing's Test' [-@Davidson:1990tt]. The fourth claim (the importance of Machine Learning) is something Davidson does not pay much attention to, but that is closely related to his critique. Both are the topic of the next subsection.

So we have seen why *Davidson* finds Turing's Test particularly interesting. *I* have chosen his critique for discussion here, since it clearly relates to Computer Science and because it "opens the way for Davidson's own view into the nature of thought" [@Cavell:2004i, p. xvii].



[^metaphysics]: Davidson argues that: "If we have the semantics of a language right, the objects we assign to the expressions of the language must exist" [@Davidson:1993mm, p. 40]. Since being able to communicate successfully means getting semantics pretty right. This will in turn also mean, that if we can communicate successfully, we must get it pretty right what things are in the world and in which relation they stand to each other. And this certainly seems to be a sufficient condition for intelligence. Davidson's argument for his claim that semantics is a method for metaphysics [-@Davidson:1993mm] is based on the fact that we must get things mostly right about the world, if we are intelligible as rational beings at all.

[^ontology]: Davidson's ontology takes only objects and events as basic entities [-@Davidson:1991tv]. He rejects the need for any propositions of proximal stimuli as entities in the mind [-@Davidson:1990mt]. The content of propositional knowledge is directly caused by the distal objects and events the world is made up of.

## Davidson's Critique {#davidsons-critique}

<!--
- No need for introspection into working of mind
- distinction between semantic and syntactic abilities
- Rejection of sharp distinction between mental and physical (especially sensory) abilities
- Relation to Agreement between Descartes and Turing who both come from the idea that knowledge is simply in the head
- Even Turing's Helen Keller example lacks as she was interacting with the world through touch.
- Connected to rejection of Cartesion Epistemology
-->

Davidson finds Turing's Test inadequate to show that an object is thinking. Not because communication is not a sufficient criterion for intellectual competence for Davidson --- as we have discussed. Neither because a test would require an introspection into the workings of the mind. Davidson explicitly says that it is not inadequate because it "restricts the available evidence to what can be observed from the outside" [-@Davidson:1990tt, p.83]. But because it does not enable the interrogator to observe a history of three-way engagement between the object, a shared world, and other minds in which the object develops its semantics.

This is related to the "fundamental difference between semantics, which relates words to the world, and syntax, which does not" [@Davidson:1990ri, p. 94, he adopts the terminology from Tarski]. For Davidson, the essential requirement for though or intelligence is to assign meaning to words, to relate them to the world. But he argues that the interrogator in the Turing Test can not guarantee that the computer is able to do that:

>"[T]he interrogator [...] has no clue to the semantics of the object. There is no way he can determine the connection between the words that appear on the object's screen and events and things in the world. Of course there must be some connection; there is no other way to account for the intelligibility of the object's English. [...But i]t is perfectly possible that the connection between words and things was established by someone who programmed the object, and then provided purely syntactic connections between words for the object to wield. In this case it is the programmer who [...] has given meaning to the words [...], but the object doesn't mean anything, and there is no reason to take it to be thinking.
>
> In order to discover whether the object has any semantics, the interrogator must learn more about the connections between the output of the object and the world [...], through observing relevant causal interactions between the speaker, the world, and the speaker's audience. [...T]he interrogator [must be allowed] to watch the object interact with the world." [@Davidson:1990tt, p. 83]

The interpreter can only determine wether the computer means something by its words if he or she can tell what the computer means by them. Therefore "any evidence that thinking is going on will have to be evidence that particular thoughts are present" [-@Davidson:1990tt, p. 80]. While it is clear that thoughts have caused the computer's interaction, the test framework is not giving the interrogator a chance to determine how any thought has come to the computers knowledge, only that it has.

Davidson accredits this failure to the fact that "Turing wanted his test to draw ‘... a fairly sharp line between the physical and the intellectual capacities of man’ (p. 434). [But t]here is no such line" [@Davidson:1990tt, p. 84]. Turing was wrong that the ‘body’ of the object does not matter. Even though the details in which the sense organs convey impressions may not matter, the existence of such organs can not be reduced to purely textual communication. Turing has a somewhat Cartesian[^descartes] approach to thought. He might not prescribe to an ontological mind-body dualism, but he tends to view thoughts as independent from sensory access to the world and only dependent on being able to communicate. Turing claims the “example of [the deaf blind] Helen Keller shows that education can take place provided that communication in both directions between teacher and pupil can take place” [@Turing:1950cm, p. 456]. He overlooks that Helen Keller for one had been able to see and hear for her first 19 months and, more importantly, only learned to communicate when her teacher correlated her signs to Helen's feeling of touch [@Wikipedia:2015hk]. So this example might serve more to illustrate Davidson's externalist approach to epistemology rather than underline Turing's point that communication alone is essential for thought.

The ability to interact with the world in any way and a history of such interactions and communications about those experiences with others, is essential for developing a semantics. You "don't understand a language if there are not numerous connections between your use of words and experiences" [@Davidson:1990tt, p. 85]. The interrogator needs to observe the computer's history of engagement with the world, to judge its intelligence.



[^descartes]: In fact Descartes somewhat preconceived Turing's test in his 'Discourse on the Method'. He claims: machines "could never use words or other signs arranged in such a manner as is competent to us in order to declare our thoughts to others" [@Descartes:1637dm, Part V].

### Fairness of the Critique
<!--
- Davidson has a good point
- but he doesn't do justice to Turing's thoughts on Machine Learning that would deserve a discussion in his paper
- His emphasis on a history of causal interaction with the world is partly satisfied by machine learning
-->

So Davidson's main critique is that Turing's idea of a sharp line between physical and intellectual abilities is ill-conceived and Turing doesn't see the importance of interaction in a shared world as essential for (1) *developing* thoughts and for (2) *judging* intellectual abilities.

While the second critique is certainly justified, since the computer is hidden from the interrogator, the first point is debatable in light of Turing's work about Machine Learning. In his last footnote, Davidson claims that Turing "views this [learning] simply as an economical way of producing a device with mature thoughts; he does not see it as the only way" [-@Davidson:1990tt, p.86]. As outlined in \autoref{section1}, I think this is overestimating Turing's interest in presenting a sufficient condition for intelligence and underestimating his interest in actually building a certain grade of computer. Turing's ideas on Machine Learning take up a third of his essay [-@Turing:1950cm, pp. 454--460] and constitute --- as I argued --- a [fourth main claim](#fourth-claim). Most of his research from 1948--1952 was indeed not focused on the test which became so famous, but on approaches to build learning computers and simulating neural networks. Non of this work mentions any other approaches for building AI. Turing actually outlines ideas how a computer with an indexed memory can be constructed that relates past experiences to new situations using associative connections and evaluation based on reactions of its teacher and later based on self constructed norms [see @Turing:1951im, p. 257--258]. This seems closer to Davidson's requirement of having a history of interaction in a shared world than he gives credit for. So maybe classifying Turing as having a Cartesian approach to epistemology is premature.

Nevertheless, Davidson's critique of the *test* is justified. In the light of our discussion of Turing's work however, our perspective might change: from seeing the inadequacy of the test as a result of Turing's underestimation of the importance of learning and interaction with the world; to surprise that he deemed the learning process, that he saw as essential too, as so irrelevant for the judgement.

## Davidson's Proposal for a Modified Test {#davidsons-test}


<!--
- Davidson's outline of his test
- The ability to determine non predefined meaning is essential for intelligence
- My definition of Davidson's test
- why this ensures a rich conceptual system of the computer
-->



Davidson in fact, does not simply critique the test, but he proposes a modified test:

> "The Test must be modified [...]. The object must be brought into the open so that its causal connections with the rest of the world as well as with the interrogator can be observed by the interrogator.
>
> Can the interrogator now tell what the object thinks? The answer is that it depends [...]. Let us suppose the interrogator finds that the object uses words just as he does [...and] infers (let us suppose correctly) that the object's linguistic dispositions are similar to his own in relevant ways. In the case of a person, the interrogator would be justified in assuming that these dispositions were acquired in the usual way: in the basic cases, by past causal intercourse with things and circumstances of the sort to which the person is now disposed to respond. [...] But the assumption is not justified in the case of a computer: [...] The computer which has never experienced a dog and has no memory of dogs can't mean dog by the word ‘dog’ [...]. Thought and meaning require a history of a particular sort. [...U]nless we [...] can observe it in action over time, we have no basis for guessing how a computer came to have the dispositions it has.
>
> It is unclear exactly what kind of history is necessary [...]. But our intuitions are clear enough in many cases. You [...] don't understand a language if there are not numerous connections between your use of words and experiences[. ...] It may seem that minds are, after all, inscrutable if no present observation of their operation can reveal what they are thinking. But of course this does not follow. [...E]ven the mind of an artefact can, if it has one, be understood; it just takes longer, long enough for some history to be observed, since it cannot be inferred." [@Davidson:1990tt, pp. 84--86]

Davidson's rejection of the "sharp line between the physical and the intellectual capacities" [-@Davidson:1990tt, p. 84] should not be misinterpreted as a rejection of the possibility to devise a test at all. In his follow up essay 'Representation and Interpretation' [-@Davidson:1990ri] he comes back to the question "what could we detach from a person and still count him or her as a thinking creature" (p. 87). And agrees with Turing that origin, building material, and size and shape for example are irrelevant. In so far, Turing was on the right track with his test, he only went too far in detaching the history from a person. The ability to determine non predefined meaning --- to connect symbols with objects and events in the world --- is essential for intelligence and it depends on a rich base of experiences of causal interactions with these events and objects.

I put Davidson's explanation of the required nature of the test as follows: We may judge an object as intelligent, if (and only if --- as I will argue) the object can be observed to be able to

1. successfully communicate with other intelligent beings and
2. derive its own semantics from a history of its experiences of interaction with other intelligent beings and with objects and events in a shared world.

This is what I call 'Davidson's Test'.

The ability to come up with its own semantics from a history of interaction ensures that the computer has a rich conceptual system in Davidson's holistic approach. Because "to have even one thought --- one belief or desire --- a computer would have to have a very great many other thoughts and desires. Beliefs and desires can exist only in the context of a very rich conceptual system."[@Davidson:1990ri, p. 90][^example].

We will see in how far this test is an expression of Davidson's theory of linguistic and intellectual competence throughout the [next section](#section3) and specifically in \autoref{theory}.



[^example]: Davidson gives the following example to illustrate his point: "Alitalia Flight 19 leaves Turin for London on Tuesdays at 8:30 in the morning. We can learn this by consulting a computer; but does the computer know what we learn by consulting it? The answer is that it does not because it does not know what a flight is, where Turin is, or even that Tuesday is a day of the week." [-@Davidson:1990ri, p. 89]

### Interpretation of Davidson's Test as a Definition
<!--
- Interpretation of the test as sufficient condition
- The test is a necessary condition for the presence of though
- Introspection into the mind does not provide a sufficient condition for thought
-->

So we have a definition of Davidson's Test, it remains to explain how it is to be interpreted. Davidson takes the Turing Test as aiming "to discover whether a sufficient condition for thought is satisfied; the condition is not claimed to be necessary" [@Davidson:1990tt, p. 81]. So we can certainly interpret Davidson's Test as a sufficient condition for intelligence. But Davidson seems to go even further:

> "[T]he *only* way to tell if an artificial device [...] has [thoughts...] and the ability to perceive and interact with the world as a person does, is to attempt to *interpret the behavior* of the device in the same way we do the behavior of a person. [...U]nderstanding the program and physics of a device [...on the other hand] is *not* [...sufficient for] understanding the thought [...] of that device." [@Davidson:1990ri, p. 99, emphasis added]

It seems to me, that this is interpreted correctly as the claim that Davidson's Test provides not only a sufficient, but also a necessary condition --- and therefore constitutes an operational definition of intelligence. Interpreting the behavior of a person is nothing else for Davidson than interpreting its utterances (or some other communications with semantic content). This follows from the fact that the interpretation of the semantic content of an expression requires the interpreter to have a theory about the believes and semantics of the person and this theory must be based on the behavioral evidence the interpreter has. We will investigate this theory of interpretation from Davidson in more detail in \autoref{interpretation}.

The second part of Davidson's claim aims to reflect an obvious counter argument that might occur. If one completely understood the inner workings of a device's or person's brain, one could certainly also judge wether it was intelligent. While Davidson does not want to deny that dissecting a person's brain might enable one to undoubtedly judge a person as belonging to the species homo sapiens and therefore be justified to infer that he or she is intelligent; this is not the kind of proof we are looking for. The test provides an *explicit* definition of intelligence, while there might be other *implicit* ways of inference about intelligence. Davidson *does* reject that any knowledge of the brain can *explicitly* proof intelligence. To illustrate this he takes the programming of a machine as an example, which I will discuss in the [next subsection](#supervenience).

I have argued before that the search for a definition is replaced by the search for an empirical theory in Davidson's philosophy. So if we talk about an operational definition here, this only becomes relevant holistically because it is part of an empirical theory of intelligence --- and in Davidson's case this means a theory of interpretation.[^physics] So this theory is expected to fit empirical data about interpretations, to allow us to apply it and actually yield correct interpretations of utterances, or (since the theory is not developed far enough yet for that) at least to fit our intuitions for how we interpret others. Therefore we can't judge this definition by itself; we need to look at Davidson's theory as a whole and see whether it is a convincing empirical theory for our linguistic and intellectual competence, then we can judge whether this definition of intelligence, which provides the goal for this theory, is convincing to us. Hence we will discuss Davidson's theory in more detail in the next section.



[^physics]: To illustrate this point, let me give an example from first semester physics: Take momentum in classical physics --- the fact that we single out the meaning of this word by attributing it as a part of the empirical theory of classical mechanics already shows that it gains its relevance from its place in this theory. It gains its relevance from its place in this empirical theory that serves to describe the movement of mass under natural and artificially applied forces. We can't debate the definition of momentum (${\scriptstyle \vec{p}}$), not because it is defined in very clear mathematical terms as the time derivative of the product of mass and location (${\scriptstyle \vec{p}\;=\;\partial_t(m\cdot \vec{r})}$), but because changing its definition would destroy some of the predictive power of classical mechanics. If we would for example only take the simplified definition of momentum as the product of mass and velocity (which assumes the mass doesn't change over time (${\scriptstyle \partial_t\! m \;=\; 0 \;\;\Rightarrow\;\; \vec{p}\;=\;m\cdot\partial_t\! \vec{r} \;=\; m\cdot \vec{v}}$) --- which is still very clearly defined mathematically --- we couldn’t explain how a rocket flies that accelerates by throwing away mass (${\scriptstyle \partial_t\! m \;\neq\; 0}$); the theory of classical mechanics would lose some of its power to fit empirical evidence. This is closely related to Popper's [-@Popper:1935lf] requirement of falsifiability for a scientific theory. The definitions are only good, as long as changing them would mean that the theory as a whole can't fit some empirical evidence anymore. In this sense their meaning and relevance is determined holistically.



### Summary
<!--
- Davidson and Turing agree that we can device an empiric scientific theory about our linguistic competence and that this is essential for intelligence.
- Davidson's relation to Turing's claims
- critique that the test does not allow to observe history of interaction in world
- Davidson gives a definition of intelligence based on a modification of the Turing Test.
- Still have to argue for the basis of this analysis
-->

We have started with a discussion of how Davidson's approach to language as a social art and interpretation as an empirical process relates to Turing's approach to intelligence; pointing out that both Davidson and Turing think that intelligence can be described empirically and that there is a relation between the process of building an intelligent machine and devising an empirical theory of intelligence. I have also argued that both see linguistic abilities as essential for intelligence and agree in their affirmative answer to the question wether artificial intelligence is possible, even though both do not find the question very interesting.

Than we have learned that Davidson critiques Turing's Test for not exposing how the computer develops its own semantics from a history of experiences of interactions in a shared world. I have argued that this shortcoming of Turing's design is surprising because he agrees with Davidson that learning from experience is essential for developing intelligence.

At the end I have given a characterization of Davidson's Test that requires not only the observation (1) of successful communication but also (2) of the process of deriving semantics from a history of interactions in a shared world. I argued that this test should be interpreted as an operational definition of intelligence which we can only judge in light of how empirically convincing Davidson's theory of linguistic and intellectual competence is for which it provides the goal.

# Davidson's Theory of Intellectual and\ Linguistic Competence {#section3}





The goal of this section is to ground all the arguments from before in an understanding of the main characteristics of Davidson's view of ([3.1](#supervenience)) the relation between the mental and the physical, ([3.2](#triangulation)) his epistemology, and ([3.3](#interpretation)) his theory of interpretation. After this I am going to discuss how those understandings come together in his unified theory of intellectual and linguistic competence and relate to Davidson's Test. Wrapping up with a discussion how Davidson's view might fit into the more recent discussion between connectionism and the classical representational and computational theory of mind.

## The Meaning of Programs and Anomalous Monism {#supervenience}

<!--
- connect to Davidson's argument about the programming of a machine.
-->

We will not tackle Davidson's view of the relation between the mental and the physical heads on, but follow his approach in 'Representation and Interpretation' [-@Davidson:1990ri]. Davidson starts out with the question "how much like us [a computer] must [...] be, and in what ways, to qualify as having thoughts" [-@Davidson:1990ri, p.88]. But after establishing that a computer "cannot have thoughts unless it can learn and has learned from causal interactions with the world" [-@Davidson:1990ri, p.88] and that "what must be added to computers [...] to insure that they are capable of thought" [-@Davidson:1990ri, p.89] --- that they know *what* they are talking about --- is "a very rich conceptual system" [-@Davidson:1990ri, p. 90]. This is of course related to the holistic approach to semantics that we have discussed in \autoref{davidsons-test}. Davidson's main question for the rest of the essay now becomes *how* we can judge that a computer has such a rich conceptual system. Davidson starts by ruling out that knowledge of the operation of the system is sufficient for this judgement:

> "It may seem obvious that if an artificial object thinks and acts enough like a person, someone who knows how the object was designed and built would be able to describe and explain the mental states and actions of the object. But this does not follow, for there is no reason to suppose that there are definitional or nomological connections between the concepts used by the designer and the psychological concepts to be described and explained. This should be clear if we imagine that the builder has simply copied, molecule by molecule, some real person. [...] So one sort of ‘complete’ understanding does not necessarily imply another." [@Davidson:1990ri, p. 90]

The problem is one of *mental representation*. The "representation of an object or a fact [...in] the program cannot automatically be interpreted as a representation of that object or fact for the device" [-@Davidson:1990ri, p. 91] --- in its 'mind'. Davidson argues that indeed the representations differ. If an object or event falls under a certain mental concept there must not be an equivalent concept in the program or in a physical description. He gives the following analogy: "Suppose, following folk advice, I am attempting to go to sleep by counting sheep. Every now and then, at random, a goat slips into the file. In my drowsy state I find I cannot remember the classificatory words ‘sheep’ and ‘goat’. Nevertheless I have no trouble identifying each animal: there is animal number one, animal number two, and so on. In my necessarily finite list, I can specify the class of sheep and the class of goats: the sheep are animals 1, 2, 4, 5, 6, 7, 8, and 12; the goats are animals 3, 9, 10, and 11. But these classifications are no help if I want to frame interesting laws or hypotheses that go beyond the observed cases, for example, that goats have horns. I can pick out any particular sheep or goat in my animal numbering system, but I cannot, through conceptual poverty, tell the sheep from the goats generally. So it may be with the mental and the physical. Each mental event, taken singly, may have (must have, if I am right) a physical description, but the mental classifications may elude the physical vocabularies." [-@Davidson:1990ri, p. 92]

The program is purely syntactic, it can give explanations of its concepts in terms of other concepts it has, but it cannot specify anything about semantics, about references of its concepts, about relations of its concepts to objects or events in the world. "There is the language in which each animal can be picked out, but which lacks the concepts needed for classifying the animals as sheep or goats; similarly, syntax can provide a unique description of each true sentence, [...] but it can't classify sentences as true or false. [...] If we knew no more than the program, we would have no reason to say [...] that any aspect of or event in the device represented anything outside the device" [-@Davidson:1990ri, p. 91]. Physics work in the same way, when it appeals to strict laws which are only "drawing on concepts from the same conceptual domain and upon which there is no improving in point of precision and comprehensiveness. [...] Physical theory promises to provide a comprehensive closed system guaranteed to yield a standardized, unique description of every physical event couched in a vocabulary amenable to law" [-@Davidson:1970me, p. 223--224]. Just like the program a complete physics is precise and contains no ceteris paribus (other things being equal) clauses in its explanations and it does not appeal to any concepts outside of its realm[^qm-observers].

This is different for theories involving mental events where "an event is mental if and only if it has a mental description [...that involves terms like believing, intending, desiring, knowing, perceiving, remembering, and so on], the distinguishing feature of the mental is [...] what Brentano called intentionality” [-@Davidson:1970me, p. 211]. The distinguishing feature of such events is that they are dispositional predicates which are causal in nature: "if Cain killed Abel, he must have done something that caused Abel's death, and if he killed Abel intentionally, he must have been caused to act by a desire for Abel's death. Beliefs, desires, and intentions are themselves causal dispositions" [-@Davidson:1990ri, p. 95]. Such causal dispositions do not feature in physics: "it is a sign of progress in a science that it rids itself of causal concepts. The dissolving of some salt is explained, up to a point, by saying that salt is soluble and this salt was placed in water; but one could predict the dissolving on the basis of far more general knowledge if one knew the mechanism, what it is about the constitution of the salt that accounts for its dissolving. When the mechanism is known, the explanation will not call on the causal concept of solubility" [-@Davidson:1990ri, p. 96]. This is also related to the semantical nature of our mind. In "specifying the contents of a memory, [we are forced] to refer to causes normally outside the person, [...giving] a causal explanation of a belief [...and] a semantic interpretation of it" [-@Davidson:1990ri, p. 96]. In this way mental representation is externalistic, it refers to terms outside of its descriptive scope.

So we have seen that physics and programs provide comprehensive theories that are purely syntactical and thus refer to no external concepts which allow them to be expressed in strict laws which eliminate causal dispositions. We have seen that mental concepts on the other hand are semantic in an essential way and are expressed as causal dispositions. Thus we can conclude that mental predicates can not occur in strict laws [See @McLaughlin:2013am, p. 417-423]. This is what Davidson calls the Anomalism of the Mental: "there are no strict [...] laws on the basis of which mental events can be predicted and explained" [@Davidson:1970me, p. 208].[^turing-rules]

But [other than @McLaughlin:2013am seems to suggest] this is not the final argument Davidson has in mind, because externalism, ceteris paribus laws, and causal dispositions "could also be said to distinguish the concepts of many of the special sciences such as biology, [...] there must be something more basic or foundational" [@Davidson:1991tv, p. 217]. Otherwise we would assume that "knowledge of the program of a device that successfully mimics the workings of the mind, will explain the mechanisms that support or constitute thought" [@Davidson:1990ri, p. 96--97] just like physics can explain the causal disposition of solubility.

> "It is only when we can see a creature (or ‘object’) as largely rational by our own lights that we can intelligibly ascribe thoughts to it at all [...]. This means that when anyone [...] ascribes thoughts to others, he necessarily employs his own norms in making the ascriptions. There is no way he can check whether his norms are shared by someone else without first assuming that [the other is intelligible and] in large part they are [...shared. I]f the subject under study is to remain thought and intelligence, a normative methodology cannot be avoided." [@Davidson:1990ri, p. 97--98]
>
> "We depend on our linguistic interactions with others to yield agreement on [...] the sort of structures in nature that allow us to represent those structures in [...] numbers. We cannot in the same way agree on the structure of the sentences or thoughts [...], for the attempt [...] sends us back to the very process of interpretation [...]. It is here, I suggest, that we come to the ultimate springs of the difference between understanding minds and understanding the world as physical. A community of minds is the basis of knowledge; it provides the measure of all things. It makes no sense to question the adequacy of this measure, or to seek a more ultimate standard." [@Davidson:1991tv, p. 218]

Interpretation of mental concepts is essentially normative, it requires us to assume a basic shared understanding of the world without which we cant interpret others. We must assume others are largely coherent in their thoughts and corresponding to the same stimuli in the world as we are. This irreducibly normative character does not appear in physics or programs but it is this character which allows us to render any intelligible picture of the world. Physics and programs can't give an account of their semantics, only our evaluation of their predictive powers puts them in a relation to the world. The concept of causality allows us to bridge the gap between these explanatory schemes, its looseness is necessary to overcome the distance between the normative and formal explanations [see -@Davidson:1990ri, p. 98]. The ability to put things in relation to the world only emerges through our communication with others (we will discuss this more in the next \autoref{triangulation}). The mental is irreducible in so far as it constitutes the basis of our very ability to make the world intelligible through such communication about a shared world.


[^qm-observers]: This is assuming a complete physics of the world, which the practical science of physics strives to reach. In the science of physics of course there are still many issues like the inability of quantum mechanics to define in physical terms what an observation is that leads to the collapse of the wave function. But the fact that this is seen as a huge deficiency of the theory by most physicists illustrates this description of a complete physics --- independent of wether it is achievable or not.

[^turing-rules]: In his section 2.(8) about the 'Argument from Informality of Behaviour' Turing discusses a somewhat related argument that there is no "definite set of rules of conduct" [-@Turing:1950cm, p. 452] which govern the behavior of a person and that therefore a deterministic computer could not simulate a person's behavior. As Turing points out this argument (which he is not deriving directly from any other literature, but establishing himself in this crude way) fails because it is beside the point and has no evidence for its claim. But unlike Oppy and Dowe [-@Oppy:2011tt, p. 21, a fairly poor entry in the Stanford Encyclopedia of Philosophy] suggest the argument could easily be made strong if we suppose a mind-body dualism, causal influence of the mind on the body, and one of the various arguments like the one given here that there are no strict rules governing mental processes.

### Supervenience and Anomalous Monism



We have seen that Davidson argues at length for the anomalism of the mental --- mental events don't feature in strict laws and are thus irreducible to the physical. But we have also already seen that Davidson agrees with Turing that brains might act similarly to computers and that it should be generally possible to make thinking computers. In fact, Davidson rejects any cartesian mind body dualism. "The mental and the physical share *ontologies*, but not [...] classificatory concepts" [-@Davidson:1990ri, p. 92].[^spinoza] Davidson labels this combination of ontological monism and agreement to the principle of the anomalism of the mental 'Anomalous Monism' in 'Mental Events' [-@Davidson:1970me], where he introduced this view. This view rests on the type-token-distinction: "each particular mental event [token] is identical with a particular physical event [token, but...] there are no strict psychophysical laws [...and therefore] no mental event type is a physical event type" [@Lepore:2009d, p. 17].[^fodor] So while the behavior can be completely explained on a physical level, since mental events are identified with physical events which are governed by strict laws. The physical explanation or the understanding of the program does not offer any insights for a mental explanation since the physical event tokens don't fall under any mental types. "Knowing the program is enough to explain why the device produces the marks or sounds or pictures it does given an input described in similarly abstract terms. This knowledge does not touch on questions [...] of reference to the outside world" [@Davidson:1990ri, p. 93]. To make sense of the explanation by relating it to the world we need a mental level.

> "Anomalous monism resembles materialism in its claim that all events are physical, but rejects the thesis [...] that mental phenomena can be given purely physical explanations. [...] Although the position I describe denies there are psychophysical laws, it is consistent with the view that mental characteristics are [...] dependent, or supervenient, on physical characteristics. Such supervenience might be taken to mean that [...] an object cannot alter in some mental respect without altering in some physical respect. Dependence or supervenience of this kind does not entail reducibility through law or definition" [@Davidson:1970me, p. 214]

Davidson's idea of the supervenience[^supervenience] and irreducibility of the mental to the physical has been highly discussed[^discussion] and very influential. As mentioned before it also provides the basis for the claim that "the only way to tell if an artificial device [... can think], is to attempt to interpret the behavior of the device [...because] interpretation involves the use of normative concepts [... which] have no role in the understanding of a syntactically specified program" [-@Davidson:1990ri, p. 99]. So a behavioral test like Turing's and Davidson's Test is a necessary condition to judge anything as intelligent, be it a person, an animal, or an object.



[^spinoza]: Davidson argues that 'Spinoza's Causal Theory of the Affects' [-@Davidson:1999sc] might be interpreted as a form of anomalous monism.

[^fodor]: Another famous argument against reductionism by @Fodor:1974ss is also related to the fact that a special science type has multiple realizations through physical tokens, but those will fail to establish any physical type predicate at least in most cases.

[^supervenience]: The modern use of the term supervenience actually originates in 'Mental Events' [@Davidson:1970me, p. 214]. "This is the first explicit statement of a psychophysical supervenience thesis in the literature" [@McLaughlin:2013am, p. 427, see also p. 438].

[^discussion]: Davidson's 'Mental Events' [-@Davidson:1970me] has been a very influential and highly discussed paper. For an introduction to some main discussions around Anomalous Monism about mental and physical taxonomies and event individuation, strict laws and completed physics, Ramsification, strong and weak supervenience, and type epiphenomenalism and the cause law principle see @McLaughlin:2013am.

## Triangulating Knowledge of a Shared World {#triangulation}


- Connect to questions from 'What Thought Requires'.
- Interdependency of three varieties of Knowledge
- Importance of disctinction between true and false beliefs (E5.8, E3.14, E4.1, SEP Davidson)
- Principle of Charity (Coherence and Correspondence)
(E3.14, E2.9, E3.14)
- Reaction to stimuli (E3.14)
  - proximal vs. distal stimuli (E5.4)
- Iscrutability of Reference / Indeterminacy of meaning (Quine Word and Object, E5.3, E2.16, E3.14)
- The Underlying Ontology and Metaphysics
  - Ontology of only objects and events (E3.14, E5.4)
  - Directness of knowledge of world
    - no intermediary entities (5.3, E5.4, E3.10)
    - no mentales, language only through communication, meaning given causally by objects events (E5.9)
  - Truth as elementary non-reducible concept (E5.2, E2.I)

"Adding a second person [...] narrows down the relevant cause to the nearest cause common to two agents who are triangulating the cause by jointly observing an object and each other's reactions. The two observers don't share neural firings or incoming photons; the nearest thing they share is the object prompting both to react in ways the other can note. […] Triangulation also creates the space needed for error, not by deciding what is true in any particular case, but by making objectivity dependent on intersubjectivity." [@Davidson:2001wt, p. 142--143]





> “So we need to ask what would turn calculation, in the sense in which [...] a computer can calculate, into thought? […] Some non-human animals can learn a great deal, but they do not learn that something is true. […Only] a creature with propositional attitudes is equipped to fit a new concept into a complex scheme in which concepts have logical and other relations to one another. […S]ome degree of holism goes with having concepts.
>
> [T]he fundamental distinction [lies] between a mindless disposition to respond differentially to the members of a class of stimuli, and a disposition to respond to those items as members of that class. […] A creature that cannot entertain the thought that it may be wrong has no concepts, no thoughts. To this extent, the possibility of thought depends on the idea of objective truth, of there being a way things are which is not up to us. […] What is needed is something that can provide a standard against which an individual can check his or her reactions, and only other individuals can do this. […] Adding a second person helps on both counts. It narrows down the relevant cause to the nearest cause common to two agents who are triangulating the cause by jointly observing an object and each other's reactions. The two observers don't share neural firings or incoming photons; the nearest thing they share is the object prompting both to react in ways the other can note. […] Triangulation also creates the space needed for error, not by deciding what is true in any particular case, but by making objectivity dependent on intersubjectivity. ” [@Davidson:2001wt, p. 138--137 & 141--143]

Principle of Coherence
connection to Theory of action [see @Lepore:2009d, p. 12]



See [@Lepore:2009d, p. 19--20] for the importance of Triangulation





### Three Types of Knowledge

- The basic problem of Epistemology
  - Distinctiveness of three types of Knowledge (subjective, intersubjective, objective)
  - Three Questions of Epistemology
    - how to know other minds
    - how to know world
    - how to know own mind without evidence
- Rejection of other Epistemologies
  - Rejection of Positivism (reductionism to world knowledge) (E3.14)
  - Rejection of empiricsit Epistemology (E3.14, E2.1)
    - No primacy of names and predicates in the foreground of senses
    - doesn't he contradict that in E2.9 and E4.8?
  - Rejection of Cartesion Etymology (primacy of knowledge of one's own mind) (E3.14, E3.3, E3.13)
    - Rejection of skepticism (E3.14, SEP Davidson, E4.1)

















### The Social Aspect of Language {#social-language}

- The Primacy of Ideolect
  - relevance of interpretation rather than meaning (+E2.2)
    - see similarities to Gadamer's Hermeneutics of Wirkungsgeschichte (Bertram 2012)
  - Relevance of Intention in communication (+E5.10)
  - Arguments for primacy of ideoloect over language
    - Malapropisms and the like (E5.7)
- Why is language necessarily Social
  - Wittgenstein's norm of actually getting it right in language
    - also see language game analogy in anti conventionalism (2.18)
    - and importance of disctinction between true and false beliefs in triangulation (E3.14)
  - Truth only determined trough communication
    - see also Plato, socrates (E5.16)







## From Prior to Passing Theories of Interpretation {#interpretation}


- Sources of Davidson's theory
  - Davidson's Program
  - Radical Interpretation from Quine adopted
  - Triangulation
  - Prior and Passing Theories
  - The social Aspect of language
  - Unified theory of Thought, Action, and Meaning



So what is it that I am referring to when I speak about Davidson's theory of interpretation? While this seems like a straight forward question it is a little more complicated because of the distributed nature of Davidson's work.

Davidson's theory can be traced back to his rejection of meaning and idea that interpretation can be described as a process of 'translating' utterances into truth conditions based on assumptions about the believes of the speaker using the principle of Charity, which he develops in 'Truth and Meaning'[^davidsons-program] [@Davidson:1967tm] and 'Radical Interpretation' [@Davidson:1973ri].




[^davidsons-program]: His idea that truth conditions (T-Sentences) are all that is needed to explain interpretation, and any more fundamental notion of meaning is misconceived, has also led to what is known as Davidson's Program: The attempt to give an account of the interpretation of utterances purely with the means of first order logic.

Descision theory: Sprang from his early times at Stanford when collaborating with Patrick Suppes and JJC McKinsey. [@Lepore:2009d, p. 2]

See also [@Rescorla:2013rc] for discussion of unified theory

### The recursive and empirical nature of interpretation

- No a priori knowledge about language(-learning), only empirical knowledge
- Finite set of linguistic primitives gives rise to infinite linguistic expressions
- Representation of Meaning/Linguistic Content: Meaning as Language (E3.14, E2.2) (not things in world, not entities sui generis)



'Theories of Meaning and Learnable Languages' [@Davidson:1965tm]

in first order logic[^action]

[^action]: Davidson's contribution to the analysis of action sentences with first order logic has gained widespread use by computational linguists. "Action sentences present a problem for semantics because of their capacity to take an endless variety of adverbial phrase, which themselves can be endlessly complex. [...] The event analysis that Davidson introduced treats action verbs as introducing an implicit existential quantifier over events, and the adverbs as contributing predicates of it." [@Lepore:2009d, p. 16] The sentence "Brutus stabbed Caesar violently with a knife" for example can analyzed as: ${\scriptstyle \exists}$ *e* : *e* = 'event of stabbing by Brutus of Caesar' : UsingKnife(*e*) ${\scriptstyle \land}$ Violent(*e*).





### Anti-Conventionalism

- arguments against conventionalism:
  - impossibility of public sign for sincerity
  - language game analogy (+E5.8)
- Remarks about how understanding does work
  - At the end of [-@Davidson:1984cc], Davidson says that understanding can't be formally described
  - Relation to distinction linguistic between competence and prerformence







### The Distinction between Linguistic Competence and Performance {#linguistic-competence}

- Distinction between sufficient and necessary conditions of linguistic competence
  - relation to term linguistic competence and linguistic performence
  - relation to *radical* interpretation
  - analogy to physics not being able to describe actual natural systems but only systems under ideal conditions
  - Davidson's transition from a formal (logical/mathematical) theory of meaning (that describes how to derive meaning) to an empirical theory of meaning (that judges interpretation as evidence) is essential here.
  - See (E4.8, E5.8)
- Relation to Davidson's Philosophy
  - truth conditions as a formal language
  - Unified Theory, Radical Interpretation
  - Sucessfull Communication & Anti-Conventionalism & Holims of knowledge
- How is the anomalism of the mental connected to our linguistic competences (or maybe just to our effectiveness?), how does the unified theory account for it.







> "we have erased the boundary between knowing a language and knowing our way around in the world generally. For there are no rules for arriving at passing theories, no rules in any strict sense, as opposed to rough maxims and methodological generalities. A passing theory really is like a theory at least in this, that it is derived by wit, luck, and wisdom from a private vocabulary and grammar, knowledge of the ways people get their point across, and rules of thumb for figuring out what deviations from the dictionary are most likely. There is no more chance of regularising, or teaching, this process than there is of regularising or teaching the process of creating new theories to cope with new data in any field—for that is what this process involves." [@Davidson:1986nd, p. 107]

I use the term *linguistic competence*[^linguistic-competence] here to refer to Davidson's idea of the essential aspect of understanding language vs. the practical understanding of language.


[^linguistic-competence]: The term linguistic competence was introduced by Chomsky who makes a "fundamental distinction between competence (the speaker-hearer's knowledge of his language) and performance (the actual use of language in concrete situation)" [@Chomsky:2014at, p. 4]. While Davidson  criticizes the idea of linguistic competence as knowledge of a language, he adopts the term for the description of his theory that describes the interpreters essential competence in 'A Nice Derangement of Epitaphs' [-@Davidson:1986nd].



## Davidson's Test and the Theory of Intellectual\ and\ Linguistic Competence {#theory}


- Interpreting Davidson's Test as a Test for a Unified Theory 'machine'



### Objections against Davidson's Test {#objections}

- behaviorism
- mechanism
- scope of the test
- Objection based on Internal Operation Arguments
  - Blockheads
  - The Chinese Room (Internal Operation)
- French: Associative Priming and Rating Games
- abstract terms and wirkungsgeschichte









Ability to cope with Abstract Terms

It remains unclear how well Davidson's theory might be able to cope with abstract terms in the language.

He throws very little light on how understanding of abstract terms might work.

There are good reason's to doubt that communication about abstract terms can work in the same way as other communication. Something like the Wirkungsgeschichte becomes way more plausible, if we look at how culturally loaded language is

See also Bertram's critique: Gadamer's idea [@Bertram:2012ta]

Davidson to Gadamer, [@Davidson:1997gp]



### Anti-Representationalism and Connectionism

- status of program not interpretable
- non-deterministic in some way
- externalistic because of data dependence
- Davidson as a connectionist, rejects classicist Computational Theory of Mind, agrees with computability of mind
- Also externalist, anomalous monism solves problem of external dependence of mind, even though brain is in the scull

"A neural network is a collection of interconnected nodes. Nodes fall into three categories: input nodes, output nodes, and hidden nodes (which mediate between input and output nodes). Nodes have activation values, given by real numbers. One node can bear a weighted connection to another node, also given by a real number. Activations of input nodes are determined exogenously: these are the inputs to computation." [@Rescorla:2015ct]




# Conclusion {-}







## Davidson's Theory and Machine Learning {-}


- is Davidson's argument of understanding a program really justified

While Davidson is skeptical about the possibility of explaining our linguistic performance. He believes that there is a pragmatic and empirical theory about the essence of linguistic competence.

## Implications for Artificial Intelligence and Computer Linguistics {-}






Davidson tries to device a theory that can model human intellectual abilities in an empiric theory that has the power to explain them. (As opposed to only a simulation of the brain by a machine)

While it currently seems more probable that Turing’s Test and also Davidson’s Test will be passed by a computer that leverages trained large scale deep neural networks aka. something into the direction of simulating the brain. Davidson’s consideration still provide important input into what is needed to achieve human level of natural language abilities. That is the ability to somehow interact with the world and have some sensory impression of it and have a triangular model of determining world interaction.

- Possibility of AI and the importance of Language
  - Davidson sees artificial intelligence as possible.
  - He agrees that language is the key test for intelligence.
  - Davidson and Turing agree that the task is not to explain human linguistic practice, but create an empirical theory that models the essence of linguistic competence. This is a very important philosophical distinction that should be understood very well in order to build language processing systems and not get distracted with the wrong problems.
- Important boundary conditions for linguistic competence
  - Linguistic and intellectual competence are inherently social/intersubjective
  - Linguistic and intellectual competence require interaction with the shared world (empiric)
- Denial of conventionalism and statistical linguistics
  - The social and empiric traits of linguistic and intellectual competence can not be modeled by conventionalism, if this convention requires a previously shared common practice. Interpretation emerges in the instance of communication and cannot be predetermined in anyway.
  - Abilities of linguistic interaction can not be clearly separated from abilities for physical interaction. Both are necessary for intelligence.





# Acknowledgements {-}

Many thanks to ... for reading this paper ...

### Colophon

This paper was written with [Gingko](https://gingkoapp.com) in [Pandoc Markdown](http://pandoc.org) and typeset using [XeTeX](http://xetex.sourceforge.net) in Gotham Narrow. My research process is inspired by Luhmann's Zettelkasten methodology, using [Evernote](https://evernote.com). If you are interested, you can find an article about my research and writing process on my blog (<http://MrLoh.se/2015/10/research-and-scientific-writing-process>).

# References {-}
