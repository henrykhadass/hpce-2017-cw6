HPCE CW6 Individual Reflection
==============================

Imperial login : hh2214

Github login : henrykhadass

CW5 group : Baozi

CW6 group : Baozi

Cohort : [DOC4] (delete as appropriate)

Guidance
--------

_The goal of this component is to get people to think about what they
have learnt in an individual sense, and to try to think about how
this course has developed or changed your own skills, knowledge, and/or attitudes.
This section is individually marked, so I (m8pple) will look at
every single submitted `reflection.md` and evaluate it. There may
or may not be feedback provided on this component (and if there is,
it will come way off in Feb or something). Usually most people will say
something sensible and realistic, which is the main point, and
serves as immediate feedback in and of itself. I'm most likely
to comment if the points made are particularly good, or particularly
vague, generic, dismissive. Ideally these should be specific to an individual,
not to a group, so I suggest doing it alone._

_There is no hard marks schema (I moderate across the cohort),
no example answers, and I'm not seeking a specific answer. A response
given by one student might be excellent, but almost the same response by
another might look quite weak - it all depends on individual context.
Each of the 50 word responses is weighted equally._

_A possible response to some questions could be: "I haven't learnt
anything, I already knew how to do it." That's awesome, presumably
made this course very easy, and should be reflected in the
performance-oriented marks for CW5+CW6. Not everyone gets something from the
course: some people just need to get marks or pick something they already
know how to do. Those who already knew the content or have covered it in
other courses should (theoretically) cruise through. An entirely intentional
aspect of this component is that those who already have the most experience
will need to work that bit harder to justify why and where they have learnt
something._

_The load of this component is expected to be at most an hour per
person, and up to 500 words. *You do not need to write 500 words to
get good marks.* The 50 word limit per answer [is mainly to encourage
specific-ness and reduce work-load](https://github.com/HPCE/hpce-2017-cw6/issues/42)._

Connections with existing courses and knowledge
===============================================

_Which courses that you took in previous years did you think this course was most related to,
and why? These could be courses in any department or any university._

I have never taken an optimisation related course before so I am not able to make a comparision in that sense. However, I have taken a C++ course before in DoC which was very practical like this course, as well as a Robotics course in which we had to complete a new assignment every two weeks last year.

_What relevant pre-existing skills and existing knowledge did you bring to the course?_

I could program! I am not very comfortable with C++ since I have not used it very often even though we were taught it in DoC as mentioned above. I was also familiar with Git since I have used it extensively over the years of my degree and was surprised that some EIE students were using it for the first time. 

What have you learnt in the course? : practise
==============================================

_What has been the most useful practical skill you have acquired in this course?_

Gaining an understanding of how to translate a peice of software to OpenCL, particularly the concept of passing messages using buffers. I feel that had I done this in my own time I would not have been able to understand that section of the course.

_When would it have been useful in your own past activities?_

I have not had an occaison in the past were I had encountered an optimisation problem in software engineering, which was my main reason for taking the course as I wanted to learn about this area of computing.

_When do you anticipate it might be useful in the future?_

I would like to pursue a career in quantative finance were they deal with (software) optimisation problems almost daily so I hope this would be a useful addition to my CV and to my personal arsenal of knowledge.

_What practical aspect (e.g. TBB, OpenCL, AWS, shell, ...) do you think is
 the *least* likely to be useful, and why?_
 
In my opinion it would be the shell. Although pretty much everything is done through it, there is no need to become a 'master' at using the shell, however knowing how to interact with it while writing scripts is an incredilby useful skill. Knowing a number of basic commands should be enough to get you through this course


What have you learnt in the course? : theory/concepts
=====================================================

_How has the course changed your understanding of how to accelerate
or improve program performance? _

I had no knowledge of how to go about accelerating or improving program performance before the start of the course. The only thing I was vaguely aware of was the use of FPGA's. As such I have learnt a lot about TBB and OpenCL as tools for acceleration, in addition to algorithmically restructuring programs to acheive acceleration as well.

_What is a _specific_ example of tuning agglomeration *you* encountered or resolved in CW5 or CW6? Where
 possible, refer to a commit and source file (e.g. embed a link)._

Personally, outside of CW2 I did not implement any agglomeration techniques. For CW5 we did not identifiy any areas where we could agglomorate, however my team mates implemented agglomeration for one particular [case](https://github.com/HPCE/hpce-2017-cw6-Baozi/blob/master/testu01/testu01/bbattery.cpp) in Rabbit where they decreased the granularity of the tast_groups parralelising the test suite.

_What is a _specific_ example of managing critical path that *you* encountered or resolved in CW5 or CW6?
 Where possible, refer to a commit and source file._

We speculated as a group to reducing the time taken for MultiNom to run, as it was the longest running test, however this was not an *individual* encounter per se. 

_What is a _specific_ example of balancing communication vs computation cost from CW5 or CW6?
 Where possible, refer to a commit and source file._

During CW5 I worked on the Mining and Heat World puzzles by putting them on the GPU through OpenCL. The TEA_Hash algorithm in the Mining puzzle was a clear example of balancing communication vs computation since the algorithm was itself coputationally intensive but didn't frequently talk to its parent method [Execute](https://github.com/HPCE/hpce-2017-cw5-Baozi/blob/master/provider/mining.hpp#L2). 
