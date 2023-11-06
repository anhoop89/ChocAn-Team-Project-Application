# ChocAn
Group project for CS 314 at Portland State University
```
Team: Anh Ho, Layla Smith, Dan Ha, Ben Anderson, Ryan Niiya, Linh Nguyen, Thomas Brooks
```



## 1 Introduction

This is a design document that will cover the design considerations, system overview, system architecture, and a detailed description of the system design for the Chocoholics Anonymous (ChocAn) software project. In this introduction section, the purpose and scope for the document and project will be described, the target audience will be outlined, and there will be a section for terms and their respective definitions. For the sake of clarity, any terms that were defined in the requirements document will be defined again in this document. 

### 1.1 Purpose and Scope

The purpose of this document is to define and demonstrate the design considerations that will be undertaken by the team for the ChocAn project. The document will be split up into 5 major sections. Following the introduction section, which is briefly described above, the document will contain design considerations, a system overview of the project, details on the system architecture, and a detailed system design. Firstly, the design considerations section will go over any constraints and dependencies (both functional and non-functional), as well an overview of the modified waterfall engineering methodology being utilized. Following this, the system overview will provide a complete, high level abstraction of the system as a whole. This will prepare readers for the system architecture section, providing diagrams and tables when needed. Next, the system architecture will provide a detailed, high level description of the various subsystems and components that will be developed by the team for the ChocAn simulator. Diagrams will be used in this section to help support the sub-systems described. This section is primarily meant for non-developers, with the next and final section, detailed system design, being more oriented towards software developers. The detailed system design section will provide more detail to the previous system architecture section, providing pseudo code, data structures, and in general a much more in-depth and software oriented approach to the system being developed.

### 1.2 Target Audience

This document is intended primarily for software developers and system engineers, as the design considerations, system overview, and detailed system design sections will heavily use software terminology and development processes. The detailed system design will be heavy on software design and terms, including pseudocode, data structures, and any other facets of implementation that will be required. The system architecture may also be viewed by customers, to show a general overview of the system that will be developed, but will additionally be primarily directed towards a developer audience. 

### 1.3 Terms and Definitions 

Provider: Health care professional who provides services to ChocAn members.

Member: Patients of ChocAn who pay a monthly fee for access to unlimited consultations and treatments. (See Member Card)

Manager: Manages providers at ChocAn.

User: Those who will use the software directly, in this case the Providers and Managers.

Member Card: A plastic card embossed with the member’s name and a nine digit member number and incorporating a magnetic strip on which that information is encoded

Service: An activity a provider provides to benefit a member.

Service Code: A six-digit code corresponding to a service provided by providers.

Service Fee: Amount to be paid based on a service given.

Date of Service (DOS): Date (MM-DD-YYY) that a service was given.

Provider Directory: An alphabetically ordered list of service names and corresponding service codes and fees sent to the provider as an email attachment. All providers may access this directory. (See Service Code)

Provider Number: A unique identifier for each provider, used to access the ChocAn terminal.

Stakeholder: A person, company, or business who is involved in the development of the project.

Use Case: Type of interactions between the company and a user.

Electronic Funds Transfer (EFT): Digital movement of funds between one bank account and another, consisting of banking and provider accounts for this project.

ACME Accounting Services: Third party organization that will handle processing ChocAn membership fee payments.

Manager Terminal: Computer system that can run accounting reports and generate summary reports when needed.

Provider Terminal: Computer system that will allow providers to bill and enter in provided services, access fees to be paid, and access the provider directory. 

Unified Modeling Language (UML) diagram: Diagram that will be utilized in this document to demonstrate the system architecture of the program.

Binary Search Tree (BST): Categorization of nodes in a hierarchical, tree-like structure. Allows for easy searching based on names or other important information. 


...

## Detailed System Design
Based on the system architecture which has been designed with a modified Model-View-Controller (MVC) pattern for the ChocAn system, we decided to use the structure of the concept of object-oriented programming with a single-inheritance hierarchy to build the ChocAn system. We break down the requirements of the design into several classes that help us easier to implement and maintain the system. There are four main classes and a few subclasses supporting the main classes. The main classes include manager, model, provider, and member. The subclasses will be used for data structures of the binary search tree and collected information, which is from providers and members, to export a weekly report. The software system will be fully implemented using C++ language programming.
