# 470Capstone


## 1/19
## ---------

Sofwater Dev
Sequential vs. iterative (waterfall v. agile) 

Use waterfall if requierments are stable and low risk (predictability) 
Iterative has more flexibility in working with unknowns 

### Documentation
-forces you to think the problem all the way through
-vehcile for communications

### Timing 
20-30% devoted to up-front planning and requirements
Build in contingency time
Set clear milestones with specific timelines

Gantt Chart - grapical representation [gnattvisual](https://teamngnatt.com)


### Project Skills
Docmentation via a project notebook 
      - contains refrences, designs, ideas, timelines

Project Communication 
Weekly status report for customer updates
Document meetings and plans to help with final report
Develop Agenda for meetings 

Report Porblem searn and articulate unkowns

Maintain a github for the group and use sticky notes (Padlet, Trello, Miro, Pivotal Tracker, Asana) 

The main document is both requirements and design:
      Enough detail to explain the project (5-10 pages) 
            -Overview
            -Requirments
            -Design
            -Planning
            -References
            
            
            
## 1/24

ALEX HILL scholarship if working on a community project

Feb 7 Resume Review


###Common Security Problems (465) 
"24 Deadly Sins of Software Security"

AI Systems causeless insecure code...
Those with AI "believe" they wrote more secure code

-Holes in web software + flaws in server software
"Blaster Worm"


#### SQL Injection - add aditional code for password input

XSS (cross site spliting) [Dom based, refleced, stored types] 
      input from user - echo back to user
      
#### Web client vulnerabilites
Use SSL or store data on server side + encrypt

#### Buffer Overruns
inputing beyond the limit
-Look for input read ins
-Transfer data to internal struces             * Dont allow user input to affect buffer size calculation
-look for unsafe string handling calls
-pre allocate max buffer size
                        C++ STL considered safe
                        Chek loops and arrays 
                        
#### Format strings - %x %n (looking at 4 bytes at a time) 
                        if echoing back to user ensure formatting
                        
#### INT overflows 
number too big for allocated bits - reverts back to 0 
signed int to larger
0x7f --- 0x00000007F

signed int to larger unsigned
-1 = 0xFFFFFFFFF or 4,294,967,295
                        use SafeInt class
                        Use unsighned ints if appropriate
                        Straightfowrad Code
                        
#### C++ Pointers
method of corrupting pointers
overwriting virtual methods
                        Use STL 
                        Declerae private constructors and operator assignments
                        Initialize all variables
                        do not mix up array new/delete with regular new/delete
                        
##### Exceptions
if you don't know just quit
                        Do not catch all exceptions

#### Command Injection
accessing things that have root access
calls directly to "system" , "exec", "root"
                        always check user input
                        
#### Failure to handle errors
address error reports 

#### info leakage
software versions, debug info, error messages

#### race conditions
multi-threaded applications 
multi processes to same source
                        lock access to any query for mutual exclusion
#### Poor usability
            ----Future Lecture-----

#### Not updating Easily
make updates easy

#### Executing Code with Too Much Privlage
                        Aim for lowest privlege if things go wrong
                        
#### Finish here  
Pick up next class

## 1/26

# Arctic Spark Thermal Imaging with Boro
[Proposal Guildines](https://docs.google.com/document/d/1FXH15dz2AcKGvCCo54791-7nqb79ktrdqKgJnAyRNec/edit)

### Continuing Security Sins

### Design

fdsa

## 1/31

REMEMBER TO COMMIT YOUR WORK STUPID!!!!!!


### Resume Tips w/ Alexis from Career Services

Don't use Canva
Obtain Templets from Career Services, USA JOBS

Tailor your resume for each JOB!!! Mimic the language used in the Job Description

- Highlight the job description
- Note related and transferable skills 
- Note anything else might be relevant

- Projects section !!!!
- Arctic Coastline Modeling
- DuckieBot
- New thing I'm working on 
- Skills Section
- Don't use photos
- 

Cover Letter
- start using cover letters
- match w/ cover letter template
- Dear hiring manager

part | contents
--|--
intro | who are you and why you are interested
body | exapnd qualifications
conclusion | tahnk you for you considerations
> using personalized 'I' language to convey a story about your qualifications

### 470 Notes for the day

Proposal due wednsday Feb 8th 
- Status report
      1. brief description
      2. what progress has been made
      3. challenges have you face
      4. what are you going to work on next

### Gui Bloopers 

#### Basic Principles 
![image](https://user-images.githubusercontent.com/70354960/215926227-43f67d41-f2f8-474e-bf50-235435feba32.png)

> mistakes when designing graphical user interfaces. Goal is to give example of mistakes and help designesrs and developers
1. Foucus on user and their tasks, not the tech
      - software shouldn't be designed for them or by them, but with them
2. Consider function first, presentation later
      > function is the basic requirements of the software, before Gui creation we need to know what data the users can create, view or modify
3. conform to user's view
      - strive for naturalness
      - don't impose abitary restrictions
      - user vocabulary not tech jargon
      - keep internals inside (don't allow access to critical functionality) 
4. dont complicate user's tasks
      - don't give extra problems to solve, operate in the background of user's though process
5. facillitate and promote learning 
      > be consistent in design and implementaiton 
6. Deliver information, not just data
7. the screen belongs to the user
      > helsp the user retain context<br>
      > preserve display inertia, "don't jump around or reload screen" 
      - Real time interface
            - productivty falls as response time grows 
8. Test Early and often, 
