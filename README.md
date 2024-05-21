# SpringProject
ІПЗ-23 Палюга Надія
# Link to mockup
https://www.figma.com/design/6HV6Fy3ZaNqfVtfBftE51v/project?node-id=7%3A309&t=Ll9md8jPZ9oISWsv-1
# ER-diagram
![image](https://github.com/NadiiaPal/SpringProject/assets/126204844/d183d958-0e9b-41bb-bdfe-185651151032)
# Functional Requirements
## User-Student: 
- See list of his subjects 
- See only his marks 
- See dates, when his mark was earned
- See theme of lesson
 
## User-teacher:
- See list of subjects in each course
- See list of students in each subject, their absence, their marks ,their dates 
- Create page in grade book with subject
- Put marks to each student
- Write themes of lessons
- Put date of lessons
- Put absence
 
## Student:
- StudentID
- StudentCourse
- StudentGroup
## Teacher:
- TeacherID
## Subjects:
- SubjectID 
## Lessons:
- Marks
- Absence
- Dates
- Themes

# GET:
/mainPage -  
Req: be authorised  
Resp:  main page
 
/studentMain -   
Req: be authorize as a student  
Resp: page of subject
 
/teacherMain - 
Reg: be authorize as a teacher
Resp: page of subject
 
/teacherMain -  
Reg: be a teacher, have a rights to create a subject  
Resp: page of creation a subj
 
/creation -   
Reg: be a teacher  
Resp: created page of subject
 
/teacherSubject -  
Reg: be authorize as a teacher  
Resp: after press a button "+" return page for   
creation lesson

# POST:
/creation -   
Reg: be a teacher  
Resp: send information about new subject
 
/teacherSubject -   
Reg: be authorize as a teacher  
Resp: send information added by teacher(marks,  
Date)  
 
/createLesson -  
Reg: be a teacher  
Resp: send information about new lesson  


