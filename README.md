#CSI 410 – Database Management Systems - Fall 2016



##Meeting times:  
<table>
  <tr>
    <td>Class</td>
    <td>Mondays</td>
    <td>8/29/2016 - 12/12/2016</td>
    <td>4:15pm to 7:05pm</td>
    <td>ES0241 </td>
  </tr>
  <tr>
    <td>Final</td>
    <td>Monday</td>
    <td>12/19/2016</td>
    <td>5:45pm to 7:45pm</td>
    <td>TBA</td>
  </tr>
</table>


##Instructor
<table>
  <tr>
    <th>Name</th>
    <th>Email</th>
    <th>Office Hours</th>
  </tr>
  <tr>
    <td>Paul Tomchik</td>
    <td>ptomchik@albany.edu</td>
    <td>After class and by appointment</td>
  </tr>
</table>




##Course Description from the CS Department ([link](http://www.cs.albany.edu/cs_courses.shtml#CSI410))

> Introduction to using relational database software and database management systems. 
>
> In-depth coverage of a practical 
>
>   + Structured Query Language (SQL), 
>   + physical and logical database design, 
>   + rollback and recovery techniques,
>   + and access methods including interfaces to programming languages.
>
> Prerequisite(s): two semesters of course work in computer programming or equivalent experience. 
>
> Familiarity with data structures and operating systems concepts is helpful but not required.

##Class GitHub Repository ([link](https://github.com/csi410-fall-2016))



##Course objectives

1. This course is geared towards students who wish to become 
   back-end developers, full-stack developers, or DBAs.
   It will also be beneficial for students who wish to do research that requires managing data.
   The development of skills and hands-on experience will be heavily emphasized.

2. Homework and test questions will be modeled closely on interview-style 
   questions for the above mentioned jobs.

2. Students will be *introduced* to the theoretical and engineering problems/solutions 
   of enterprise database systems. However, this is not a theory course. 
   Theory will be covered only to the extent that
   it is needed for sound decision making and problem solving by _users_ of DBMSs.
   For a deeper understanding of the internal workings of DBMSs, CSI 508 is highly recommended.

3. Students will gain experience managing an enterprise-class database system.
   We will use Postgres 9.5 for this class. 
   You will be responsible for your own Postgres database.
   You will develop a data model and your database will be used by a web application. 
    (The web application will be provided, but you will write the structured queries.)
   Your database will be required to provide high-throughput with low latency response times
    by using a combination of optimization techniques that we will cover in this course. 
    The performance of your database will factor into the assignment grades.

4. Students will be required to read official Postgres documentation and take advantage of the 
   wide range of resources available online to understand the concepts essential for 
   large scale data management.

##Prerequisites: 

+ You will need to ssh into a \*nix (Unix/Linux) server and use the command-line.
  If you have used itsunix, you should be fine.
    Expect me to cover any tricky shell commands in class and to provide
    examples and templates.

+ Sample code and homework testing suites will use Git/GitHub.
  Very basic commands are all you will need, and I will provide those for you.
  Using Git will not be necessary, but you will be at a heavy disadvantage 
    compared to those students who know or learn how to use Git and GitHub.

+ Some examples from the lectures will use [Docker](https://www.docker.com/). 
  If you would like to run these on your own and modify them, you will need to install Docker.
  They will assume an intermediate level of \*nix command-line skills.
  Those who are familiar with, or who make the effort to learn, 
  the command-line in \*nix will be at an advantage as they will be able
  to explore these materials more throughly.

+ Coding assignments will be mostly limited to SQL. 
  The exceptions would be that I will require some simple Bash scripts that call 
    Postgres admin programs such as pg_dump and pg_restore.

    * [pg_dump](https://www.postgresql.org/docs/9.5/static/app-pgdump.html)
    * [pg_restore](https://www.postgresql.org/docs/9.5/static/app-pgrestore.html)


##Required texts: None. 

Throughout the semester, reading and video-watching assignments will be given 
from various online resources. For many of these assignments, 
I expect that you will need to find supplementary reading materials to clarify
and to ask questions regarding the more advanced details of these assignments.

###Sample reading material sources:
+ [dba.stackexchange.com](http://dba.stackexchange.com)
+ [Google books](https://books.google.com/books?id=1PgCCVryjOQC&lpg=PP1&pg=PP1#v=onepage&q&f=false)
+ [YouTube Database Convention Presentations](https://www.youtube.com/watch?v=W6B8-srOsrs)
+ [Official Postgres Documentation](https://www.postgresql.org/docs/9.5/static/index.html)
+ [Official Postgres User Forums](http://planet.postgresql.org/)

I will be using these (or similar) books as I prepare for lectures:
+ [PostgreSQL 9 Administration Cookbook](https://www.amazon.com/PostgreSQL-9-Administration-Cookbook-Second/dp/1849519064)
+ [PostgreSQL 9 High Availability Cookbook](https://www.amazon.com/PostgreSQL-9-High-Availability-Cookbook/dp/1849516960)
+ [PostgreSQL for Data Architects](https://www.amazon.com/PostgreSQL-Data-Architects-Jayadevan-Maymala/dp/1783288604)


##Grading:

I want everyone to do well in this course. 
I realize that some people test well, while others do not.
The grading for this class will therefore be flexible to accommodate different types of abilities.

Below, I specifically state the flexiblity that I will allow myself when assigning grades.
Out of fairness, these rules are final. 

I will curve the grades, if needed. 
Any raw score above 90 will be guaranteed an A-. 
Any raw score above 95 will be a guaranteed A.

###Grading formula weights
<table>
  <tr>
    <td>Homeworks</td>
    <td>30-50%</td>
  </tr>

  <tr>
    <td>Exams</td>
    <td>50-70%</td>
  </tr>
  <tr>
    <td></td>
    <td>
      <table>
        <tr>
          <td>Midterm</td>
          <td>25-35%</td>
          <td>(Oct. 24th 5:05pm to 7:05pm)</td>
        </tr>
        <tr>
          <td>Final</td>
          <td>25-35%</td>
          <td>(Dec. 19th 5:45pm to 7:45pm)</td>
        </tr>
      </table>
    </td>
  </tr>
</table>


The weights given to homeworks and exams will be determined according to the rules explained below.
*They will always be applied in the manner that maximizes your overall final score.*
The flexibilty built into these rules is to allow you to benefit from hard work 
throughout the semester (homework), or your ability to recall knowledge while under pressure (exams).


###Homeworks:
+ There will be at least 10 homework assignment "units."
    (The number of units assigned to a homework assignment will depend on 
      the number of weeks given for you to complete the assignment.
      The minimum value of an assignment will be 1 unit. 
      Longer assignments will be worth 2 units.
      Expect 1 unit a week, except for those weeks leading up to exams when there will be no homework.)

+ Homeworks must be submitted via BlackBoard. Do not email them to the instructor or T.A.

+ Homeworks will be accepted up to 48 hours after the deadline. 
    After that, they will receive a grade of zero.
    A late penalty of 1% of the assignment grade will be deducted 
      for each _hour_ that it is late.
    Re-submitting an assignment after the deadline subjects the grade to the same penalty.

+ The best 6 homework units will necessarily count towards your homework average.

+ For each assignment (up to 4) that you complete beyond the required 6,
    it will be included in the calculation of your homework score 
    and the weight given towards homework assignments will increase by 5%
    if and only if applying this rule to that assignment increases your overall course score.
    
    In otherwords, if you complete 10 homework units, 
    and your average across all 10 of those assignments is higher than your exams score, 
    your homework average will count for 50% of your final score. 
    If, on the other hand, you complete 10 homework units,
    but including the 9th highest homework grade drops your homework average 
    below your exams score, the highest 8 homework units will count 
    and your homework score will be 40% of your final raw score.

+ Any collaboration on homeworks will be considered cheating unless the assignment 
    specifically states that teamwork is allowed. 

    You should use the time before the assignment is given to pool together your 
    knowledge and resources.

    To document that your collaboration with classmates occurred before the assignment
    was given, use the BlackBoard forums. 

    I will not alter homework assignments to avoid giving questions covered
    in the BlackBoard discussions. If a forum post makes a problem trivial, 
    thank the person who made the post.


###Exams:
+ There will be a midterm and a final. Both exams will be mandatory.

+ They will each count equally towards your final score. 

+ Together they will comprise the remainder of your final score after the homeworks.
  Therefore, together, their weight may range from 50-70% of the final score.

+ The exams will be closed-book.
  I will allow a single, double-sided, 8.5 inches x 11 inches sheet of paper with notes for each exam.

###Makeup Exams: 

Makeup exams will be given only for valid and verifiable excuses (e.g. a major
medical situation). If you are going to miss an exam, you must contact your instructor ahead of
time and arrange to take a make-up exam at an alternate date/time. In general, a makeup exam
will be harder than the regular exam.

###Attendance: 
Although class attendance is not required, you are strongly urged to attend the lectures.

###Advice:
+ The rules are designed to *incentivize hard work*. 
  Treat them otherwise at your own peril. (They have the potential to punish laziness.)
  They are also designed so that you will need to be engaged in the class all the way until the end, 
    though your stress level for the final may be relatively light.

  
##Readings
+ Readings will be assigned *before* the material is covered in class. The reasons for this are:
      
  1. The ability to self-teach is extremely valuable in computer programming.
     If you do not already have that skill, you need to develop it.

  2. I am relying on you to ask me questions before and during class.
     This course will be better if I know what aspects of the class you find 
     especially challenging and/or interesting.

+ Before lecture, you will be expected to discuss the upcoming lecture's material 
  with classmates on BlackBoard. In addition to the reading materials that I 
  assign and suggest, I hope that you will contribute materials that you 
  discover on your own and that you find helpful (No copyright infringements!)

##Classroom Etiquette
+ *TURN OFF YOUR PHONES OR SILENCE THEM BEFORE CLASS STARTS.*
  If you must only silence them, make sure to remove them from the UAlbany WiFi network
    so that they do not waste the limited WiFi resources of the classroom. 

+ If I begin to see groups of people regularly showing up late for class, my policy will
  be to lock the door after class begins. 
  Advice: *"If you are not 5 minutes early, you are 10 minutes late."*

##Policy on Cheating:
(Largely taken from Prof. Ravi's CSI 604)

As described in the grading section above, I intend to curve the grades and reward hard work.
If you cheat on any assignment or exam, you will harm those students who work hard for 
their place on the curve. I will have no mercy on you. If you have a tendency to cheat 
in your classes, you should drop this course now.

1. Cheating in an exam will result in an E grade for the course. 
   Further, the students involved will be referred to the Dean’s
   office for disciplinary action.

2. Homework problems are meant to be individual exercises unless otherwise stated; 
    you must do these by yourself.  Any of the following actions will be considered as cheating.

      (a) A solution which is identical to or nearly identical to 
            the solution submitted by another student in the class.

      (b) A solution which is identical to or nearly identical to 
            a solution available on the Internet.

   Cheating in a homework exercise will result in the following penalty for all the students involved.

    (a) The homework in which cheating occurred will be assigned a grade of ZERO.

    (b) Every homework assignment will now count.
        You lose the abilty to drop any homework grade. (Homeworks will count as 50% of your grade.)
        This change is retroactive: 
          IF YOU CHOSE NOT TO DO AN EARLIER ASSIGNMENT THINKING THAT IT WOULD BE DROPPED, 
            IT WILL STILL COUNT AS A ZERO TOWARDS YOUR GRADE.

    *Advice*:
      You are better off not handing in an assignment handing in one in which you cheated.

   Students who cheat in two or more homeworks will receive an E grade for the course. 
   The names of such students will also be forwarded to the Dean’s office for disciplinary action.

##Policy on I grades: 
'I' grades will only be given for genuine extenuating circumstances that
are beyond your control after the final drop date with a ‘W’ grade 
(Monday November 8, 2016 for undergraduates). 

At the time when you request an I grade, your work must be in good standing.
Written documentation must be supplied either by you or by the University administration 
about the extenuating circumstances.



##Course Outline 
(Largely from Ted Borys' Syllabus)

1. ####Administration

2. ####Introduction
  + History
  + Advantages, disadvantages, and functions
  + General database terminology

3. ####Relational theory and background
  + Concepts
  + Terminology
  + Relational Algebra

4. ####SQL: Data Manipulation Language
  + Syntax
  + Semantics

5. ####SQL: Data Definition Language
  + Syntax
  + Semantics

6. ####Physical Implementation
  + Indexing
  + Optimization

7. ####Logical and physical database design
  + Normalization
  + Top-down versus bottom-up
  + Logical integrity
  + Business rules
  + Draft physical database design

8. ####Transaction management
  + Before / after images
  + Locks
  + Commitment
  + Physical integrity
  + Update-in-place algorithm
  + Alternate algorithms

9. ####Advanced topics (as time allows)
  + RAID
  + Distributed databases and two-phase commit
  + Replication
  + PostGIS (Spatial and Geographic objects for PostgreSQL)
  + Posgres JSON Datatype
  + NoSQL Systems
  + Operational versus decision support
  + Performance considerations
  + Data warehouse / data mart

* I expect the midterm to include material up to and including section 5,
  and possibly include material from section 6.


#GOOD LUCK!
