# WORKSHEET 2
## Identify Objects, Classes, and Relationships

**Instructions:** Use the process and proposed system from Worksheet 1 to complete this worksheet.

---

## Part 1. Identify the Objects

Identify the important people, things, records, transactions, or concepts that your proposed system needs to represent.

**Guide Question:**

If you were going to create a program for this process, what things would the program need to represent? 

| No. | Object | Description |
|:---:|---|---|
| 1 |User|The one who accesses the CRAM-NET system |
| 2 |Student |User who accesses academic resources and submits requirements |
| 3 |School Personnel |User who monitors network usage|
| 4 |Device |A gadget connected to the Wi-Fi. |
| 5 |Wi-Fi Network |Provides internet access to users. |
| 6 |Academic Task |A school-related activity. |
| 7 |Task Urgency |Shows the urgency of an academic task.  |
| 8 |Bandwidth |The internet speed available to users. |
| 9 |Network Session |Records a users' Wi-Fi connection. |
| 10 |Activity Log |Records a users' internet usage. |

### Object Evaluation

For each identified object, ask:

- Does it play an important role in the process?
- Does it contain information?
- Does it perform an action?
- Does it interact with another object?
- Does the proposed system need to keep track of it?

**Reminder:** Remove objects that are not necessary for your proposed system.

---

## Part 2. Analyze Object Interactions

Determine how your identified objects interact with one another.

**Example:** `Student → submits → Request`

| No. | Object 1 | Interacts | Object 2 |
|:---:|---|---|---|
| 1 | Student | Use | User |
| 2 | School Personnel | Use | User |
| 3 | School Personnel | Creates/Updates | Academic Task |
| 4 | Student | Views/Completes | Academic Task |
| 5 | Academic Tasks | Evaluates/Updates | Task Urgency |
| 6 | Task Urgency | Ranks/Flags | Academic Task |


---

## Part 3. Identify Possible Classes

Determine which objects can become classes in your proposed system.

Not every object needs to become a class. Choose only the objects that are important to your proposed system.

| No. | Class | What does it represent? |
|:---:|---|---|
| 1 |User |Represents a person who accesses the CRAM-NET system, including students and teachers. |
| 2 |Student |Represents students who view, organize, prioritize, and complete academic assessments. |
| 3 |Teacher |Represents teachers who create and update academic assessment information. |
| 4 |AcademicTask |Represents academic requirements, including assignments, quizzes, projects, and their corresponding information. |
| 5 |PriorityManager |Represents the system responsible for evaluating and ranking academic tasks based on their deadlines and importance. |

---

## Part 4. Class Analysis

Analyze the attributes and methods of each identified class.

### Class No. 1

**Class Name:** User

**Purpose:**  
Represents individuals who access the CRAM-NET system, including students and teachers. It stores their basic account information.

#### Attributes

| Attribute | Description |
|---|---|
|userID |Unique identification number of the user. |
|name |Full name of the user. |
|username |Username used to access the system. |
|password |Password used to authenticate the user. |


#### Methods

| Method Name | What does it do? |
|---|---|
|login() |Allows the user to access the system. |
|logout() |Allows the user to exit the system. |
|updateProfile() |Updates the user's personal information. |
|viewProfile() |Displays the user's account information. |

---

### Class No. 2

**Class Name:** Student

**Purpose:**  
Represents students who use CRAM-NET to manage their academic requirements, monitor deadlines, and track their assessment progress.

#### Attributes

| Attribute | Description |
|---|---|
|studentID |Unique identification number of the student. |
|gradeLevel |Grade level of the student. |
|section |Section where the student belongs. |
|taskList |List of academic tasks assigned to or recorded by the student. |

#### Methods

| Method Name | What does it do? |
|---|---|
|viewTasks() |Displays the student's recorded academic assessments. |
|addTask() |Allows the student to add an academic task. |
|updateTaskStatus() |Updates the completion status of an academic task. |
|viewPrioritizedTasks() |Displays academic tasks arranged according to priority. |

---

### Class No. 3

**Class Name:** Teacher

**Purpose:**  
Represents teachers who provide and manage academic assessment information so students can keep track of their requirements and deadlines.

#### Attributes

| Attribute | Description |
|---|---|
|teacherID |Unique identification number of the teacher. |
|subjectHandled |Subject or subjects handled by the teacher. |
|sectionHandled |Section or sections handled by the teacher. |
|assessmentList |List of academic assessments created by the teacher. |

#### Methods

| Method Name | What does it do? |
|---|---|
|createAssessment() |Adds a new academic assessment to the system. |
|updateAssessment() |Modifies the details of an existing assessment. |
|deleteAssessment() |Removes an assessment that is no longer needed. |
|viewAssessmentList() |Displays the assessments created by the teacher. |

---
**Additional Classes:** Add another copy of the Class Analysis section for each additional class you identify.

**Reminder:** Keep your project simple. Avoid creating unnecessary classes.

---

### Class No. 4

**Class Name:** AcademicTask

**Purpose:**  
Represents the different academic requirements that students need to complete, including their subject, assessment type, deadline, importance, and completion status.

#### Attributes

| Attribute | Description |
|---|---|
|taskID |Unique identification number of the academic task. |
|taskName |Name or title of the assessment. |
|subject |Subject associated with the academic task. |
|dueDate |Date and time when the assessment is due. |
|assessmentType |Category of the assessment, such as quiz, assignment, or project. |
|importance |Indicates the importance of the academic task. |
|completionStatus |Indicates whether the task is pending, completed, or overdue. |

#### Methods

| Method Name | What does it do? |
|---|---|
|addTask() |Records a new academic task in the system. |
|updateTask() |Updates the information of an existing academic task. |
|deleteTask() |Removes an academic task from the system. |
|markAsCompleted() |Changes the task's completion status to completed. |

---

### Class No. 5

**Class Name:** PriorityManager

**Purpose:**  
Represents the system component responsible for evaluating and organizing academic tasks according to their deadlines, importance, and urgency.

#### Attributes

| Attribute | Description |
|---|---|
|priorityLevel |Indicates the priority assigned to an academic task. |
|urgencyLevel |Indicates how urgent an academic task is. |
|daysRemaining |Number of days remaining before the deadline. |
|prioritizedTaskList |List of academic tasks arranged according to priority. |

#### Methods

| Method Name | What does it do? |
|---|---|
|calculateUrgency() |Determines how urgent an academic task is based on its deadline. |
|assignPriority() |Assigns a priority level based on the task's urgency and importance. |
|rankTasks() |Arranges academic tasks from highest to lowest priority. |
|identifyOverdueTasks() |Identifies academic tasks that have passed their deadlines without being completed. |

---
## Part 5. Identify Class Relationships

Determine how your identified classes are related to one another.

| No. | Class 1 | Relationship | Class 2 | Why are they related? |
|:---:|---|---|---|---|
| 1 |User |Inheritance |Student |Student is a specialized type of User that has additional student-related information and functions. |
| 2 |User |Inheritance |Teacher |Teacher is a specialized type of User that has additional teacher-related information and functions. |
| 3 |Teacher |Association |AcademicTask |Teachers create and update academic tasks that students need to complete. |
| 4 |Student |Association |AcademicTask |Students view, record, monitor, and complete their academic tasks. |
| 5 |AcademicTask |Association |PriorityManager |PriorityManager evaluates academic tasks and determines their urgency and priority levels. |
| 6 |PriorityManager |Association |Student |PriorityManager provides students with an organized list of prioritized academic tasks. |

### Relationship Types

| Relationship | Description |
|---|---|
| **Association** | Two classes interact with one another. |
| **Aggregation** | One class groups or contains objects that can exist independently. |
| **Composition** | One class strongly owns another object. |
| **Inheritance** | One class is a specialized version of another class. |

**Reminder:** Use only the relationship types that make sense for your proposed system. Not all relationship types are required.
