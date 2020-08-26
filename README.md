# concurrency

Description
In this assignment you will gain hands-on experience with parallel programming and the
difficulty of building correct parallel programs. You are tasked with helping your professor
schedule his office hours. The professor is teaching 2 classes this semester, class A and
class B, and is holding shared office hours for both classes in his office. The professor can
have a large number of students showing up for his office hours, so he decides to impose
several restrictions.
Functional Requirements
Requirement 1: The professors's office has only 3 seats, so no more than 3 students are
allowed to simultaneously enter the professor’s office. When the office is full and new
students arrive they have to wait outside the office.
Requirement 2: The professor gets confused when helping students from class A and
class B at the same time. He decides that while students from class A are in his office, no
students from class B are allowed to enter, and the other way around.
Requirement 3: The professor gets tired after answering too many questions. He decides
that after helping 10 students he needs to take a break before he can help more students.
So after the 10th student (counting since the last break) enters the professors office no
more students are admitted into the office, until after the professors's next break. Students
that arrive while the professor is taking his break have to wait outside the office.
Requirement 4: In order to be fair to both classes after 5 consecutive students from a
single class the professor will answer questions from a student from the other class.
Requirement 5: Your program should ensure progress, i.e. if there is no student in the
professor’s office and the professor is not currently taking a break an arriving student
should not be forced to wait. Similarly, if an arriving student is compatible with the
students currently in the office he should not be forced to wait, unless the professor is due
for a break.
Requirement 6: Your code shall not deadlock. 
Non-Functional Requirements
Requirement 7: Your source file shall be named officehours.c. The source file must be
ASCII text files. No binary submissions will be accepted.
Requirement 8: Tabs or spaces shall be used to indent the code. Your code must use
one or the other. All indentation must be consistent.
Requirement 9: No line of code shall exceed 100 characters.
