Q1

The Output, "hey form meeeage1" --> in the container "1"

-------------------------------------------------------------------------------

Q2

the Output, 

"hey from message1" 	--> 	 in the container "1"

"hey from message2" 	-->	 in the container data("1")



the context will run the first method because it doesn't depend on other methods, 

and the second method since it relies on Qualifier("1") it will wait for it to run before it

-------------------------------------------------------------------------------

Q3

the Output, 

"hey from message1"

"hey from message3"          

"hey from message2"     

OR

"hey from message3"
"hey from message2"
"hey from message1"

&nbsp;			OR

"hey from message3"

"hey from message1"

"hey from message2"



method2 relies on method3 so it will never run before it, but method1 is flexible it can run before or after (2and3) OR between them.

-------------------------------------------------------------------------------

Q4

the Output,

the First

"hey from message1"

"hey from message3"				

"hey from message2"

"hey from main controller"				

OR Second 

"hey from message1"

"hey from message3"

"hey from main controller"

"hey from message2"

OR Third

"hey from message1"

"hey from main controller"

"hey from message3"

"hey from message2"

OR Fourth 

"hey from message3"

"hey from message1"

"hey from message2"

"hey from main controller"

OR Fifth 

"hey from message3"

"hey from message2"

"hey from message1"

"hey from main controller"

OR Sixth 

"hey from message3"

"hey from message1"

"hey from message2"

"hey from main controller"



the rule here is (method3 then method2), and (controller then method1), and between them it can be anything.

---------------------------------------------------------------------------------

Q5

the Output,

"hey from message3"

"hey from message2"

"hey from main controller"

"hey from message1"

method3 doesn't depend on any methods so it will run first, and since method3 is required to run method2, now method2 can run.

after that the controller can run since it requires method2 to run before it,

after controller run the last method running will be method1, and it is requiring controller to run first so it can run.









