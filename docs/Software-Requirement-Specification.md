# Software Requirement Specification

## 1. Introduction

### 1.1 Purpose

The purpose of this document is to outline the requirements for The Search Engine, which is designed to provide user with the ability to search the web and find revelant information about the topic they are searching for "easily".

### 1.2 Scope

The Search Engine will support crawling, indexing, ranking, searching, personalized results, and analytics.

### 1.3 Definitions, Acronyms, Abbreviations

<!-- word: definition -->
crawling: the action of searching the web for information
indexing: the action of saving the web information or websites
ranking: the action of ranking results based of specific factors

### 1.4 References

* Search Engine Best Practices
* Database Management Best Practices

### 1.5 Overview

This document provides a detailed description of the system's functionality, performance, constraints, and other factors affecting the system.

## 2. Overall Description

### 2.1 Product Perspective

The Search Engine is a standalone system that interacts with external systems such as NoSQL databases to store the webpages.

### 2.2 Product Functions

Function: description

* Crawling: crawling the internet to look for webpages to index
* Indexing: storing those webpages found by the crawler
* Ranking: ranking the indexed webpages for revelant results
* Searching: searching the indexed webpages to find results
* Analytics: real-time analytics of a webpage to provide more revelant results
* Personalized Results: looking at history, location, user characteristics to provide more revelant results

### 2.3 User Classes and Characteristics

User Classes and Characteristics: "The primary users are students who want information about something specific."

* Students: looking for specific information
* Researchers: looking to complete their research
* Anyone curious enough: to try it and use it

### 2.4 Operating Environment

The Search Engine will operate on web browsers (Chrome, Firefox, Safari)

### 2.5 Design and Implementation Constraints

* Must comply with GDPR for data privacy.
* Use of open-source libraries for cost efficiency.

### 2.6 Assumptions and Dependencies

* Users have internet access.
* Users have basic computer literacy.
* Users have have experience with search engines.

## 3. System Features

### 3.1 Functional Requirements

#### F#01: Crawling

* Description: The process of looking for the web to find useful webpages and upadated information.
* Input: Lists of websites.
* Output: Webpages downloaded from those websites.

#### F#02: Indexing

* Description: The action of parsing and storing data to facilitate fast and accurate information retrieval.
* Input: The downloaded webpages from crawler.
* Output: The webpage and data is added to the data structure.

#### F#03: Ranking

* Description: The process of ranking webpages for revalent results.
* Input: The index data structure.
* Output: Leveling up if a webpage meets the criteria for that search.

#### F#04: Searching

* Description: The process of searching the indexed webpages to find queried information.
* Input: The query.
* Output: Found webpages containing the webpages.

#### F#05: Analytics

* Description: Real-time analytics of a webpage to help with the ranking.
* Input: Information about the search and webpages.
* Output: Analyzing the information and adding it to ranking.

#### F#06: Personalized Results

* Description: Looking at user's history, preferences, and characteristics to provide more personalized results.
* Input: User's ID.
* Output: Personalized results.

### 3.2 Non-functional Requirements

#### Performance

* The system should support up to 10000 concurrent users.

#### Security

* User data must be protected from being accessed by others.

#### Usability

* The system should be intuitive and easy to use for all user classes.

#### Reliability

* The system should have 99% uptime.

#### Scalibility

* The system should be able to scale horizontally to accommodate more users.

## 4. External Interface Requirements

### 4.1 User Interfaces

* * Web Interface: Responsive design for desktops and mobile devices.

### 4.2 Hardware Interfaces

* Servers: Hosting on on-premise servers with Nginx or Apache.

### 4.3 Software Interfaces

* Database: PostgreSQL and ElasticSearch...
* Crawling: Go
* Indexing: C/C++/Zig
* Ranking: C/C++/Zig
* Searching: C/C++/Zig
* Serving: C/C++/Zig/Erlang

### 4.4 Communication Interfaces

* Protocols: HTTPS for secure communication.

## 5. Other Non-functional Requirements

### 5.1 Performance Requirements

* Response time for any action should be less than 2 seconds.

### 5.2 Safety Requirements

* Regular backups should be taken to prevent data loss.

### 5.3 Security Requirements

* Multi-factor authentication should be implemented for logged in users (if they want it).

### 5.4 Software Quality Attributes

* Maintainability: The codebase should be modular and well-documented.
* Portability: The system should be deployable on different server platforms.

### 5.5 Business Rules

* The content provided must adhere to business standards.

## 6. Appendices

### 6.1 Glossary

* API: Application Programming Interface
* GDPR: General Data Protection Regulation

### 6.2 Analysis Models

* ER Diagrams: Database structure. Use Case Diagrams, ER Diagrams, Sequence Diagrams, UML Diagrams
* Use Case Diagrams: Illustrating user interactions with the system.
