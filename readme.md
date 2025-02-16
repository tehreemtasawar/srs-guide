# srs-guide
> Detailed guide about creating good Software Requirement Specifications (SRS)

These notes provide a clear and concise guide on *Software Requirement Specification (SRS)*, explaining its purpose, components, and best practices for creating effective SRS documents.  

Whether you're a developer, tester, or just curious about how SRS works, this guide will help you understand:  

- What an SRS is?   
- Why it matters?     
- How to create one that works for everyone involved in a software project?  

## 🔗 Table of Contents 📚

1. [ What is SRS?](#-what-is-srs)
2. [Why is SRS Important?](#-why-is-srs-important)
3. [Parts of SRS](#-parts-of-srs)
   - [Introduction](#1-introduction)
   - [Overall Description](#2-overall-description)
   - [Functional Requirements](#3-functional-requirements)
   - [Non-Functional Requirements](#4-non-functional-requirements)
   - [System Diagrams](#5-system-diagrams-)
   - [External Interfaces](#6-external-interfaces)
   - [Assumptions and Dependencies](#7-assumptions-and-dependencies)
4. [What Makes a Good SRS?](#-what-makes-a-good-srs)
5. [Common Questions About SRS](#-common-questions-about-srs)
6. [Conclusion](#-conclusion-)

## 🔗 What is SRS?

SRS (Software Requirement Specification) is a document that explains what a software system should do. It clearly defines the software’s purpose, features, and how it should work. It acts like a blueprint for developers, testers, and stakeholders.    
 
**Example:**  
Imagine you want to build an online library system. An SRS will tell you:

- *What features should be in the system?* (e.g., book search, borrowing)
- *Who will use it?* (e.g., students, librarians)
- *What are the system’s limitations?* (e.g., works only on Windows)


## Why is SRS Important?

A well-written SRS helps in many ways:

1. *Clear Guidance:* Developers know exactly what to build.
2. *Reduces Confusion:* Everyone understands the system’s purpose.
3. *Prevents Mistakes:* Avoids costly rework by defining everything clearly.
4. *Helps in Testing:* Testers can verify if all requirements are met.
5. *Manages Scope:* Keeps the project focused, avoiding unnecessary features.

## 🔗 Parts of SRS

### 1. Introduction

- *Purpose:* </br>
Defines why the system is being created.
  - Example: "This system is for managing library books, allowing students to search, borrow, and return books easily."
  
- *Scope:* </br> Describes what the system will and won’t do.
  - Example:
    - ✅ The system will allow students to borrow books.
    - ❌ The system will NOT manage staff salaries.
  
- *Definitions:* </br>Explains technical terms used in the document.
  - Example: "Late Fee" means the fine a student must pay if they don’t return a book on time.

- *References:* </br>Lists other related documents or guidelines.

### 2. Overall Description

- *What the System Will Do:* </br>Explains the system’s purpose in a simple way.
  - Example: "This system will replace the manual process of borrowing books and make it faster."

- *Users:* </br>Describes who will use the system and their expected knowledge.
  - Example: "Librarians and students with basic computer knowledge."

- *Constraints:* </br>Lists any limitations (hardware, software, policies).
  - Example: "The system will run only on Windows and requires an internet connection."

### 3. Functional Requirements

Functional requirements specify what the system must do to fulfill its intended purpose. These are the system’s main features.

- *Example:*
</br> 1. The system should allow students to search for books by title, author, or genre. 🔍
</br> 2. The system should allow students to borrow books by scanning a barcode. 📚
</br> 3. The system should allow students to return books and automatically update records. 🔄
</br> 4. The system should send a reminder email to students about overdue books. 📧
</br> 5. The system should allow librarians to add new books to the library catalog. 📖
</br> 6. The system should track the number of books borrowed by each student.

### 4. Non-Functional Requirements

 Non-Functional requirements define how a system should work rather than what it should do. It includes system performance, security, usability, scalability, and maintainability. These requirements ensure the system runs efficiently, securely, and is easy to use and expand.

- *Example:*
</br> 1. *Performance:* The system should be able to handle up to 100 users simultaneously.
</br> 2. *Security:* User passwords should be encrypted.
</br> 3. *Usability:* The system should be user-friendly, requiring minimal training for students.
</br> 4. *Scalability:* The system should be able to scale to accommodate a growing number of books and users.
</br> 5. *Maintainability:* The system should be easy to update with new features or bug fixes.

### 5. System Diagrams 🖼

**📌 Use Case Diagram:**  
Shows how users interact with the system.

**Description of Use Case Diagram:**

- **Students:**
  - Can search for books.
  - Can borrow and return books.

- **Librarians:**
  - Can add new books to the system.
  - Can manage book records (e.g., updating, deleting, and managing book details).

- **System:**
  - Keeps track of all actions between students and books (e.g., loaning, returning, and searching).


📌 **Example:**
 </br>  Below is a use case diagram for an online library management system, showcasing interactions between users and the system.

![](./assets/use-case-diagram.webp)

### 6. External Interfaces

- *User Interface:* </br>Describes how users interact with the system.
  - Example: "A login page with fields for username and password."
  
- *Hardware Requirements:* </br>Lists required hardware.
  - Example: "A barcode scanner for book identification."

- *Software Interfaces:* </br>The system will integrate with the following software:
  - Database system (e.g., MySQL) for storing user and book records.
  - Email service (e.g., SMTP) for sending overdue reminders.

### 7. Assumptions and Dependencies

**Assumptions (What we assume to be true):**  
It includes the things expected to be true.
- **Example:**
  - Students will have basic computer knowledge. 💻
  - The library will have stable internet access. 🌐
  - Librarians will be trained to use the system.

**Dependencies (What the system relies on):**  
It includes the things our system relies on.
- The system depends on a working database to store book records. 💾
- It requires a Windows operating system. 🖥
- The system relies on a third-party email service to send notifications.

## 🔗 What Makes a Good SRS?

1. *Clear:* Written in simple, easy-to-understand language.
2. *Complete:* Covers everything the system needs.
3. *Consistent:* No conflicting details.
4. *Modifiable:* Easy to update when needed.
5. *Testable:* Helps testers check if the system meets requirements.
6. *Traceable:* Every requirement should be linked to its source, and each can be traced through the development lifecycle.

## 🔗 Common Questions About SRS

- *What happens if SRS is unclear?*
  - ❌ Developers may build the wrong system.
  - ❌ It can cause delays and extra costs.

- *Why is testing based on SRS?*
  - Testing is based on the Software Requirement Specification (SRS) because the SRS defines what the software is supposed to do. It outlines the requirements, features, and functions that the software must meet. By testing based on the SRS, we can make sure the software works as expected and fulfills all the requirements outlined in the document. If the software meets the specifications in the SRS, it means it's doing its job correctly.

- *What if SRS misses something?*
  - ❌ The system may not fulfill user needs, leading to dissatisfaction.  

- *Who is responsible for creating and maintaining the SRS?*
  - Typically, the business analyst or product manager is responsible for writing the initial SRS, while the development team and stakeholders ensure it is updated as the project evolves.

- *What are the consequences of skipping the SRS phase?*
  - ❌ Skipping the SRS phase can lead to misunderstandings between stakeholders, feature creep, missed requirements, and ultimately project failure.

- *How detailed should an SRS be?*
  - An SRS should be detailed enough to capture all requirements, but not so detailed that it becomes overwhelming or overly complex. The goal is to be clear, concise, and comprehensive, balancing both high-level needs and specific functionality.


## 🔗 Conclusion 🎯

An SRS is like a map for developers. Writing it clearly ensures that the project succeeds and meets the user’s needs. It serves as a guideline for the entire development process, ensuring that both developers and testers are on the same page. By creating a well-detailed and precise SRS, you can minimize the risk of misunderstandings, delays, and costly rework.

## License 🛠  

This document is licensed under the **Creative Commons Attribution 4.0 International (CC BY 4.0) License** 

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
