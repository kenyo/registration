__Possible fields:__
__Course Object:__
Course number (int), Name (String), Credits (int), Period (int), Day (Char)

__Student Object:__
Name (String), ID (int), Registered courses {array of type course}, total credits (int)

__Period Object:__
Period (int), Day of the week (Char)

__Within Objects:__

__Course:__ Constructor for creating (initializing instance variable) courses, Getter for all field variables, method for checking if course was already inputted

__Student:__ Constructor creating student (check for duplication?), Getter for all field variables, Setter for registered courses, Setter for total credits, Method for checking if student was already inputted

__Period:__ Constructor creating period, Getter for all field variables

__Main Method:__ Registers student for the course:__
	Checks for course in course object
	Checks Max course load (check array for null values)
	Checks scheduling conflict


__Additional Thoughts:__  Field variable under student for Password, Do courses have a max amount of students that can register? If so add an int field variable to the course object that tracks students registered in it and add a getter and setter. Are half semester courses an option if so add this possibility under period object. Do we want a roster of students in each course add this under course object, Method checking if student exists? Setter for all fields for admin purposes? 

1. Create all courses
2. Create student
3. Register student
a. Is course in catalogue 
b. Max course load
c. Conflict of schedule
