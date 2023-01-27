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


