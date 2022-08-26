# Technical Phone Screen, Coding Interviews, and Whiteboarding Interviews

## Objectives: 
By the end of this lesson, you will be able to:
 - Explain what to expect in a technical phone screen or coding challenge
 - Explain what to expect in a whiteboarding interviews
 - Explain strategies for success in these interviews

## Rationale: 
You’ll face a variety of technical interviews throughout your job search process. While these are intended to test your technical skills, they also - importantly - are intended to test your communication skills. This lesson will give you an overview of what to expect.

### What is a technical phone screen?

The next step in most hiring processes (for data science, this can happen before or after the take-home) is a technical phone screen. The phone screen will usually take about 30 minutes, and is performed by a data scientist or software engineer who may or may not be the hiring manager. Sometimes, the types of questions you get asked at this stage of the interview will be very similar to questions that you get asked during the onsite - though the onsite will allow for a deeper dive into these topics. This stage often consists of:

* **Technical deep dive on your project.** The interviewer may ask you to tell them about a project, or may choose one from your resume to ask you about. After you give a technical explanation of your process, he or she will ask questions about the process you used, why you made the decisions you made, and about the technologies you used or related technologies. 
* **Coding problem.** Your interviewer may ask you a basic coding problem. They will give you a chance to work through it, write it down, and tell them your solution. For some examples of these kinds of problems, see here: https://sites.google.com/site/steveyegge2/five-essential-phone-screen-questions
* **Conceptual questions that don’t require code.** These are mostly to test the depth of your knowledge about technologies or concepts you claim to know. For example, for web dev students, they may ask questions about how certain functions work in JavaScript; for data science, you may get questions about certain machine learning algorithms and how you would use them to solve certain problems.
* **(For WD) Systems design questions.** From a high level, how would you design a certain product? They will want to see that you can understand the requirements, break it into pieces/steps, and then apply the correct technologies to each step.
* **(For DS) Math and stats questions.** Be ready for topics such as A/B testing, statistical significance, and how p-values are calculated. Sometimes you may also be asked about regression and linear algebra. Make sure to dive into the details to show your experience in these areas.
* **Questions about the company’s product.**

The key here is communication - many students find that they have a hard time explaining topics that they feel they understand well in their heads. For both the phone screen and later onsite interview, be prepared to talk - in detail - about the following:

**Topics for Data Science Interviews**

* Basic algorithms in sorting and searching, similar to the anagrams question
* Use of Stack and Queues / Recursion problems / Dynamic programming (Very rare)
* Data structure question about dictionary and list
* Trade-offs between memory and speed
* Bayes theorem questions
* Counting permutations and combination problems, given 5 coin flip, probability of observing at least 1 head
* Distribution questions, usually Poisson, Binomial or Exponential
* How would you make suggestions about what we should change in the company? (your answer should be relevant to the role and easily implemented. This is an opportunity for you to show what analysis you would do as an analyst.)
* What experiments you would run as an experimenter? (You should visit the website / use the product of the company and be prepared to answer the question.)
* Questions surrounding acquisition, retention, referral, and measuring value of users
* Details of logistic / linear, RF, SVM, Naive Bayes
* Statistical Power, Multiple Testing corrections, Bootstrapping
* Applied machine learning: especially supervised learning. How would you set up an algorithm for a prediction problem? See more [here](https://alyaabbott.wordpress.com/2014/10/01/how-to-ace-a-data-science-interview/)

**Topics for Web Dev/Software Engineering**

* BigO Complexity Analysis
* Array search
* Recursion
* Quicksort and mergesort
* Hashtables, trees (binary, k-ary, trie-trees, traversal algorithms, BFS, DFS
* Graphs
* Dijkstra’s algorithm
* Sometimes: math questions
* Sometimes: operating systems

For more information on these topics and how to prepare, see Lesson 8, Resources for Technical Interview Prep.


### What is a live coding interview?

A live coding interview may take the place of the phone interview - or could happen in addition to it. For this kind of interview, you will be asked to code on a shared screen or in an editor that your interviewer can see. 

Usually, the questions asked in these interviews will be similar to the kinds of online programming challenges that are readily available on web sites like HackerRank. The big difference is that you will also be explaining your thought process out loud. 

Before you start this kind of interview, make sure you have laid out the ground rules with your interviewer - for example, are you allowed to google things as you normally would? Also, ask clarifying questions to make sure you fully understand what you’re being asked before you start coding. Make sure you talk your way through the whole problem to your interviewer as you are solving it.

Afterwards, be prepared to answer questions about the problem you just solved, why you chose to solve it the way that you did, and how you could optimize your solution. 

Another version of this interview is the debugging interview. You may be given some code that isn’t running properly and be asked to find why that is. 

(You may also be asked to do a live coding interview - or a pair programming interview - as part of the final, onsite interview process. Read more about these [here](https://vampwillow.wordpress.com/2014/07/23/hacking-thoughtworks-recruitment-part-3-pairing-interview/) )


### What is a whiteboarding interview?

The whiteboarding interview is another test of your technical and communication skills. In this interview, you will be asked a question and asked to code it on the whiteboard. 

These kinds of interviews are very difficult - because they are testing a skill set that you pretty much will never use in real life. These kinds of interviews are staples for both data science and web development, and happen at all levels of roles. 

Keep in mind when doing a whiteboarding interview that the focus is actually less on getting the question right (though that also is important!) and more about showing your interviewer how you reason through a problem. When you’re coding on your computer, you have a lot of aids to get you through tough times (ahem, StackOverflow). The point of this interview is to see how you tackle something on your own - how you can break apart a problem into smaller pieces, qualify the problem, and attack it in a more or less systematic way. They are also looking for your communication skills throughout. Do you talk your way through the problem, so the interviewer can understand what you’re thinking? Or do you get silent and just start writing code?

**To prepare for a whiteboarding interview:**

* Practice ahead of time on a whiteboard. To make the experience even more realistic, get a buddy from your cohort to practice with. Give each other questions, and practice talking out loud as you work your way through them. 
* Use practice questions from Cracking the Coding Interview or another similar resource.
* Practice thinking out loud. Even if you don’t have a whiteboard, this is one of the most difficult skills to get used to - so just start talking your way through your homework assignments. 
* Practice doing problems under time pressure. Coding interviews will usually last from about 20 minutes to an hour. During an actual interview you will be much more stressed out than you will be practicing at home, and the time pressure will add yet another layer of stress. Practice working through problems quickly to help prepare yourself for this.

**When you’re doing the interview:**

* Listen carefully as the interviewer gives you the question - and take notes of everything the interviewer says.
* Ask clarifying questions to make sure you understood the prompt correctly. It’s ok to ask for more details, as well - “What did you mean when you said…?” “Tell me more about the data.” If you don’t ask these questions in advance to narrow the solution you’re working towards, your interviewer may use it against you later by pointing out edge cases you forgot to rule out.
* Do a verbal roadmap - “this is the direction I’m going to go” - and double check with the interviewer that you are actually on track. You do not need to start coding immediately.
* If you can’t think of an elegant solution, start with a brute force solution. If you’re really stuck, see if you can work the problem backwards.
* Mention invalid inputs you would check for, and edge cases. You don’t need to write the code for these unless the interviewer asks you to. 
* Run through an example and try to catch your own bugs.
* If, after this, you can think of a more elegant solution, go ahead and explain it. Be prepared to answer questions about what you wrote. 



