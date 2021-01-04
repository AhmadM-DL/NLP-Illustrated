# Lecture Notes

This is a basic notes jotted while reading "[Speech and Language Processing](https://web.stanford.edu/~jurafsky/slp3/) (3rd ed. draft) by Dan Jurafsky and James H. Martin"

## Introduction

### NLP in one paragraph

[The  HAL  9000  computer  in  Stanley  Kubrick’s  film2001:  A  Space Odyssey is  one  of  the  most  recognizable  characters  in  twentieth-century cinema.   HAL  is  an  artificial  agent  capable  of  such  advanced  language-processing behavior as speaking and understanding English, and at a crucial moment in the plot, even reading lips. It is now clear that HAL’s creator Arthur C. Clarke was a little optimistic in predicting when an artificial agent such as HAL would be available. But just how far off was he? What would it take to create at least the language-related parts of HAL? Minimally, such an agent would have to be capable of interacting with humans via language, which includes understanding humans via **speech recognition** and  (and of course **lip-reading**), and of communicating with humans via **natural language generation** and **speech synthesis**. HAL would also need to be able to do **information retrieval**(finding out where needed textual resources reside), **information extraction**(extracting pertinent facts from those textual resources),  and **inference**( drawing conclusions based on known facts). Although these problems are far from completely solved, much of the language-related  technology that HAL needs is currently being developed, with  some  of  it  already  available  commercially. Solving  these  problems, and  others  like  them,  is  the  main  concern  of  the  fields  known  as Natural Language  Processing,  Computational  Linguistics  and  Speech  Recognition and Synthesis, which together we call Speech and Language Processing.   The applications  we will consider are all of those needed for agents like HAL, as well as other valuable areas of language  processing  such  as **spelling correction**, **grammar  checking**, **information retrieval**, and **machine translation**.]J

[TODO: this script is written in 2020 many things changes and should edit Jurafsky introduction.]

### Knowledge in Speech and Language Processing

[To summarize, the knowledge of language needed to engage in complex language behavior can be separated into six distinct categories:

* Phonetics and Phonology – The study of linguistic sounds.
* Morphology – The study of the meaningful components of words.
* Syntax – The study of the structural relationships between words.
* Semantics – The study of meaning.
* Pragmatics – The study of how language is used to accomplish goals.
* Discourse – The study of linguistic units larger than a single utterance.]J

### AMBIGUITY

[All tasks in speech and language processing can be viewed as resolving ambiguity at one of these levels.]J Language is Ambiguous. "I made her duck" example statement.

## Part 1: Words

[Words are the fundamental building block of language. Every human language, spoken, signed, or written, is composed of words.Every area of speech and language processing, from speech recognition to machine translation to information retrieval on the web, requires ex-tensive knowledge about words.  Psycholinguistic models of human language processing and models from generative linguistic are also heavily based on lexical knowledge.

This  part  introduce  computational  models of the spelling, pronunciation, and morphology of words and cover three important real-world tasks that rely on lexical knowledge:  **automatic  speech  recognition**  (ASR),  **text-to-speech  synthesis**  (TTS), and **spell-checking**.  Finally, these chapters define perhaps the most important computational model for of speech and language process-ing:   the  automaton.   Four  kinds  of  automata  are  covered:

* finite-state automata (FSAs)
* regular expressions
* finite-state transducers(FSTs)
* weighted transducers
* Hidden Markov Model (HMM)
* N-gram model of word sequences]J
  
### Technique 1:  Regular Expressions

[Regular Expressions (RE) is a language for specifying text search strings.]J Although it is the simplest form of Natural Language Processing one can be surprised by how much it can be applied on different applications and be successful.

[Imagine that you have become a passionate fan of woodchucks.De-siring more information  on this celebrated woodland creature,  you turn to your favorite web browser and type in woodchuck.  Your browser returns a few sites. You have a flash of inspiration and type in woodchucks. This time you  discover  ‘interesting  links  to  woodchucks  and  lemurs’  and  ‘all  aboutVermont’s unique, endangered species’.  Instead of having to do this search twice, you would have rather typed one search command specifying some-thing like woodchuck with an optional final s. Furthermore, you might want to find a site whether or not it spelled woodchucks with a capitalW(Wood-chuck). Or perhaps you might want to search for all the prices in some document; you might want to see all strings that look like $199 or $25 or $24. In this chapter we introduce the regular expression, the standard notation for characterizing text sequences.  The regular expression is used for specifying text strings in situations  like this web-search  example,  and in other information retrieval applications, but also plays an important role in word-processing (in PC, Mac, or UNIX applications), computation of frequencies from corpora, and other such tasks.]J

