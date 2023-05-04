Download Link: https://assignmentchef.com/product/solved-csci321-project-nine-a-string-find-procedure
<br>
Objectives:

<ol>

 <li>Write procedures using strings as arguments</li>

 <li>Apply pointers</li>

 <li>Write user defined procedures</li>

 <li>Apply user defined procedures</li>

 <li>Apply loop</li>

</ol>

Problem Description:

Write a procedure named Str_find that searches for the first matching occurrence of a source string inside a target string and returns the matching position. The input prameters should be a pointer to the source string and a point to the target string. If a match is found, the procedure sets the Zero flag and EAX points to the matching position in the target string. Otherwise, the Zero flag is clear and EAX is undefined. The following code, for example, searches for “ABC” and returns with EAX pointing to the “A” in the target string.

.data

Target BYTE “123ABC342342”, 0

Source BYTE “ABC”, 0

Pos DWORD ?

.code

INVOKE Str_find, ADDR source, ADDR target

Jnz notFound

Mov pos, eax           ; store the position value




(Refer to Programming Project 4 on page 386)




<strong>Sample Run:</strong>

<strong> </strong>




<strong>Extra Credit:</strong>




You may notice that in my solution, I only take lower case y/n because I used “call ReadChar” and “call WriteChar” to get the user’s choice and display the user’s choice. If user try to type capital Y, the program will exit since it will read the “shift” key as user’s input. Any input different from lower case y will be consider a NO choice

Modify your solution so that it all handle the following two cases:

<ol>

 <li>If can take upper case letter as user’s choice</li>

 <li>If user’s choice is NOT Y, y, N, or n, prompt error message and ask user to reenter choice.</li>

</ol>




This worth 2% overall extra credit. No curve for this class. If you want one, do this extra credit so you get 2% curve!




<strong>Due Date:</strong>

Turn in YourNameProj9.asm via Blackboard. Due date will be announced on Blackboard.








