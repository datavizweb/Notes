# Challenges in NLP/NLU

* Spam Detection
** Methods : Navie Bayes

* Part of Speech Tagging
** Methods
> INPUT:
  Profits soared at Boeing Co., easily topping forecasts on Wall Street, as
  their CEO Alan Mulally announced first quarter results.
  
  OUTPUT:
  Profits/N soared/V at/P Boeing/N Co./N ,/, easily/ADV topping/V forecasts/
  N on/P Wall/N Street/N ,/, as/P their/POSS CEO/N Alan/N Mulally/
  N announced/V first/ADJ quarter/N results/N ./.
  
  KEY: N = Noun, V = Verb, P = Preposition, Adv = Adverb
  
* Named Entity Recognition
** Methods
> INPUT:
  Profits soared at Boeing Co., easily topping forecasts on Wall Street, as
  their CEO Alan Mulally announced first quarter results.
  
  OUTPUT:
  Profits/NA soared/NA at/NA Boeing/SC Co./CC ,/NA easily/NA topping/
  NA forecasts/NA on/NA Wall/SL Street/CL ,/NA as/NA their/NA CEO/NA
  Alan/SP Mulally/CP announced/NA first/NA quarter/NA results/NA ./NA
  
  KEY: NA = No entity, SC = Start Company, CC = Continue Company, SL = Start Location, CL = Continue Location
      
* Sentiment analysis
** Methods
> Best roast chicken in San Francisco! - Positive
  The waiter ignored us for 20 minutes - Negative

* Coreference resolution
** Methods
> "Carter told Mubarak he shouldn't run again." To solve whether "he" is related to "Carter" or "Mubarak".

* Word sense disambiguation
** Methods
> I need new batteries for my mouse. - "mouse" is ambiguous here.

* Parsing

* Machine Translation

* Information Translation
** Methods
** To take a text as input and represent it in a structured form like a database entries.

* Text Summarization
** To take input as text document(s) and try to condense them into a summary.

* Machine dialog system
** Methods
> User - I need a flight from New York to London, arriving at 10 pm ?
  System - What day are you leaving? 
  User - Tomorrow.
     
  System detects the missing information in your sentences.
      

* Reading list
** sec2vec
** [DSSM](http://research.microsoft.com/en-us/um/people/jfgao/paper/2013/cikm2013_dssm_fullversion.pdf) : Deep Structured Semantic Model


* [Spoken Dialogue System Course](http://projects.ict.usc.edu/nld/cs599s13/index.php)
* [Error Handling in Spoken Dialouge Systems](http://www.speech.kth.se/~gabriel/thesis.html)

Spoken Dialogue Systems

* [Recent advances in Spoken dialogue systems](http://jcse.kiise.org/posting/4-1/jcse_4-1_56.pdf)
* [Discussion on SDS](https://sites.google.com/site/yrrsds2016/roundtables)
* [Seminar on Spoken Dialouge systems Columbia University](http://www.cs.columbia.edu/~sstoyanchev/SDS2015/)
* [HLT Lecture Series Videos](https://www.csail.mit.edu/videoarchive/talks/HLT_Lecture_Series)
* [Spoken Dialogue Sytstems, University of Washington](http://courses.washington.edu/ling575/SPR2016/index.html)
* [CMU Robust Spoken Langauge understanding systen](http://www.cs.cmu.edu/~air/papers/issar_ward.pdf)
* [OHSU Center for Spoken Langauge understanding](https://www.ohsu.edu/xd/research/centers-institutes/center-for-spoken-language-understanding/)

* [github paper implementation](https://github.com/mesnilgr/is13)
* [SRI Gemini SLU System](http://www.ai.sri.com/natural-language/projects/arpa-sls/nat-lang.html)
* [AT&T SLU System](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.535.3214&rep=rep1&type=pdf)
* [MIT Summit and Voyager SLU system](https://papers.nips.cc/paper/403-from-speech-recognition-to-spoken-language-understanding-the-development-of-the-mit-summit-and-voyager-systems.pdf)
* [Machine Learning for SLU and Interaction NIPS 2015 Workshop](http://slunips2015.wixsite.com/slunips2015/accepted-papers)

* [Microsoft Spoken Langauge Understanding Group](https://www.microsoft.com/en-us/research/project/spoken-language-understanding/)
* [Thesis : Knowledge discovery throught spoken dialogue](http://www.speech.cs.cmu.edu/apappu/thesis/ebook.pdf)
* [Effect of Confusion network on Voice Search](http://www.aclweb.org/anthology/E09-1028)
* [Machine learning for Spoken Dialogue](http://www.cs.cmu.edu/~dod/papers/lemon_pietquin-intersp07.pdf)

* [SAM Project : State of the art dialogue system](http://samproject.net/the-state-of-the-art-of-dialogue-systems/)
* [Automating Spoken Dialogue Systems](https://www.csc2.ncsu.edu/faculty/mpsingh/papers/others/ismis-97-toolkit.pdf)
* [cobotDS : SDS for chat](https://www.cis.upenn.edu/~mkearns/papers/cobotDS.pdf)
* [SDS Challenges and opportunity : MSR](https://www.microsoft.com/en-us/research/publication/spoken-dialogue-systems-challenges-and-opportunities-for-research-invited-talk/)
* [POMPD based SDS](http://mi.eng.cam.ac.uk/~sjy/papers/ygtw13.pdf)
