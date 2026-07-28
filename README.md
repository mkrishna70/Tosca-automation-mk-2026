Import the **DWS.tsu** file into your project. 
This file contains all the concepts covered in this project and provides access to the required functionality.



1. Use of Module:
   Module is used to store the control information in the form of list of properties

2. Control Identifications:
   In Tosca, we've 4 control identifications
      - Identify by Properties
      - Identify by Index
      - Identify by Image
      - Identify by Anchor

3. TCP [Test Configuration Parameter]:
   Storing the test data and call whenever and wherever we required.
   Syntax: {CP[TCP_NAME]}

4. ScratchBook vs Execution List
   ScratchBook:
     - Store only latest logs
     - Mainly used for Trail runs
     - Supports step level execution
     - Recovery scenario won't run from scratchBook
  
   Execution List:
     - All execution logs will be stored in execution section
     - Used for Main runs
     - Won't supports step level execution
     - Recovery scenario run from execution section.
  
5. Verify Action Mode: Action model will apply to step level,mainly used to verify the controls
     - Exists or Not
     - Enabled or Not
     - Visible or Not
     - InnerText
  
6. Wait methods:
    - TBox Wait
    - Synchronization Timeout
    - Synchronization Timeout during waitOn

7. Timers: Timers are used to measure and track the testcase execution time
    - Start timer
    - Stop timer

8. Cardinality: It is a module attribute property and which allows us to add multiple attributes to the test step.
                cardinality default value : 0-1

9. Repetitions: To repeat the same steps within the same testcase is known as a repetitions.
                Repetition property exists in Test step folder

10. Constraint Action Mode: Constraint Action Mode is used to limit the search for a particular control.

11. Recovery Scenario: It is used to handle the intermittent behavior of the application
    To use Recovery scenarios, we need 3 pre-conditios:
         - OnDialogFilure = Recovery
         - Retry level should be TestStep
         - Recovery scenarios should be execute only from execution section

12. Work states: In Testcase level, we'll see workstates
    3 types of workstates
    a. Planned
    b. In_work
    c. Completed
