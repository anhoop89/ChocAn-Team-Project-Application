# ChocAn
Group project for CS 314 at Portland State University

### 1 Introduction

This is a Requirements Specification document for a new data processing software for Chocoholics Anonymous (ChocAn). This document is intended to define what is needed from the new data processing software for ChocAn. In this section the purpose/scope and target audience of the document will be described, and a glossary of terms used throughout the document will be provided. The rest of this document describes the stakeholders, use-cases, functional requirements, non-functional requirements, and timeline for the development of the data processing software.

## 1.1 Purpose and Scope

Chocoholics Anonymous is an organization dedicated to helping people addicted to chocolate through consultations and treatments with health care professionals. The new data processing software will provide an easy to use system for ChocAn that: simplifies the process of inputting sensitive data about ChocAn members, providers, and services; manages and stores this data for ease of access; and prepares/compiles data for preformatted, individualized reports. In more detail, the new data processing software will allow providers to check validation status of members, to charge members for their services, request a Provider Directory, add or delete members, and update member or provider records. The data processing software also stores all this data which is compiled into a record of electronic funds transfer (EFT) data which is written to the disk or as weekly reports sent to managers (who can also request this report at any time), members, and providers. The software is designed to run on a specially designed ChocAn computer terminal which has a card reader for member cards. It is also designed to accept the keyboard and card reader as input. 

## 1.2 Target Audience

This document is intended to list the requirements as given by the customer for the customer to review and ensure correctness and completeness. It is also intended for system managers to plan the software’s development process based on the requirements listed, for system engineers to refer to as they develop the software based on the requirements listed, for system test engineers to refer to as they develop tests to refine and perfect the software, and for system maintenance engineers to refer to in order to see the relationships between each part of the software.

## 1.3 Terms and Definitions

Provider: Health care professional who provides services to ChocAn members.

Member: Patients of ChocAn who pay a monthly fee for access to unlimited consultations and treatments. (See Member Card)

Manager: Manages providers at ChocAn.

User: Those who will use the software directly, in this case the Providers and Managers.

Member Card: A plastic card embossed with the member’s name and a nine digit member number and incorporating a magnetic strip on which that information is encoded

Service: An activity a provider provides to benefit a member.

Service Code: A six-digit code corresponding to a service provided by providers.

Provider Directory: An alphabetically ordered list of service names and corresponding service codes and fees sent to the provider as an email attachment. All providers may access this directory. (See Service Code)

Provider Number: A unique identifier for each provider, used to access the ChocAn terminal.

Stakeholder: A person, company, or business who is involved in the development of the project.

Use Case: Type of interactions between the company and a user.


...
