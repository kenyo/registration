# registration
Registration assignment for RU due 4/22

Project Description
You will build part of a college's course registration system (similar to WebReg, though considerably less complex). The system will keep track of a catalog of courses that students can take. It will allow the user (a student) to view and search the course catalog, and to add (register for) and drop (withdraw from) courses.

The following restrictions apply:

All courses meet only once per week, for one class period.
Days will be denoted by the following letters: 
M - Monday, T - Tuesday, W - Wednesday, H - Thursday, F - Friday, S - Saturday. There are no Sunday courses.
Class periods (time slots) are numbered from 1 to 9.
A student cannot register for a course that is not in the catalog.
There is a limit on the number of courses a student may take in one semester.
There is NO explicit limit on the number of credits a student may carry in one semester.
A student cannot register for two courses that meet on the same day and time.
Objects Implementation (Phase 2)
Course.java contains the definition of a class called Course. A Course object represents an entry for a course in the catalog. Each Course object keeps track of the name of a course, its course number (department and individual course number), the day of week and class period at which the course is scheduled, and the number of credits earned for completing the course. The Course object also keeps track of the roster – a list of students currently enrolled in the course.

*****Implement Course.java.*****

Make sure all of your fields are private and your method signatures are written exactly as defined below.


*You can assume that all parameters being passed into the constructors will be in their valid ranges.*

*You can also assume that the objects passed into the ‘equals’ or ‘compareTo’ methods will NOT be null.”



Course.java :

public Course(int department, int courseNum, String name, char day, int timeSlot, int credits)
department and course numbers can range from 0 to 999
the day and time slot are used to create a Period object – do not store the day and time slot individually
credits range from 1-4
each course maintains a list (array) of students – maximum number of students for a course is 20
getter methods for all of the variables passed into the constructor:
public int getDepartment() //returns the department number
public int getCourseNumber() //returns the course number
public String getName() //returns the name of the course
public Period getPeriod() //returns the period of the course
public int getCredits() //returns the number of credits for the course
public Student[] getRoster() //returns the roster – list of students who are enrolled in the course
public String toString()
return the course in the same format as in catalog.txt: “department:courseNum [name] period credits:credits”
ex: 198:111 [Introduction to Computer Science] T5 credits:4
public boolean equals(Course other)
two courses are considered equal if their department and course numbers are the same
