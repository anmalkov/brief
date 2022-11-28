# Security Plan - [tm-project-name]

## Preamble

The curators of this document cannot certify/attest to security of an architecture nor code - the below is intended to help identify and track design decisions and outstanding work related to discussed attack vectors identified during the engagement and intended to provide guidance to CSE dev crews.

This template is intended to help assess security risk within customer engagement and produce backlog recommendations to mitigate that risk. Security recommendations can be used in conjunction with those suggested via [BRIE (https://aka.ms/BRIE)](https://aka.ms/BRIE).

## Overview

Please find the Threat Model for [tm-project-name] below. This document shows the threat model and data flow diagram of the application. These artifacts were constructed based on documentation and source code from the project itself and are subject to change as the architecture and codebase evolves. Each of the labeled entities in the figures below are accompanied by meta-information which describes the threats, describes the data in scope, and recommendations for security controls.

## Diagrams

### Architecture Diagram

![Architecture Diagram](./architecture-diagram.png)

### Data Flow Diagram

![Data flow diagram](./data-flow-diagram.png)

#### Data Flow Attributes

| # | Transport Protocol | Data Classification | Authentication | Notes |
| :---: | :--- | :--- | :--- | :--- |
[tm-data-flow-attributes]

### Threat Map

![Threat map](./threat-map.png)

### Threat Properties

[tm-threat-properties]

---

## Appendix

### Security Principles

---

#### **Confidentiality**

Confidentiality refers to the objective of keeping data private or secret. In practice, it’s about controlling access to data to prevent unauthorized disclosure.

#### **Integrity**

Integrity is about ensuring that data has not been tampered with and, therefore, can be trusted. It is correct, authentic, and reliable.

#### **Avaliability**

 Availability means that networks, systems, and applications are up and running. It ensures that authorized users have timely, reliable access to resources when they are needed.

### Microsoft Zero Trust Principles
  
---

#### **Verify explicitly**
  
Always authenticate and authorize based on all available data points, including user identity, location, device health, service or workload, data classification, and anomalies.

#### **Use least privileged access**
  
Limit user access with just-in-time and just-enough-access (JIT/JEA), risk-based adaptive policies, and data protection to help secure both data and productivity.

#### **Assume breach**
  
Minimize blast radius and segment access. Verify end-to-end encryption and use analytics to get visibility, drive threat detection, and improve defenses.

### Commercial Data Classification Reference

---

|  Classification | Guidelines for Classification |
| :-- | :-- |
| Sensitive |  Data that is to have the most limited access and requires a high degree of integrity. This is typically data that will do the most damage to the organization should it be disclosed. Personal data (including PII) falls into this category and includes any identifier, such as name, an identification number, location data, online identifier. This also includes data related to one or more factors specific to the physical, psychological, genetic, mental, economic, cultural, or social identity of an individual. |
| Confidential |  Data that might be less restrictive within the company but might cause damage if disclosed. |
| Private  |  Private data is usually compartmental data that might not do the company damage but must be kept private for other reasons. Human resources data is one example of data that can be classified as private. |
| Proprietary |  Proprietary data is data that is disclosed outside the company on a limited basis or contains information that could reduce the company's competitive advantage, such as the technical specifications of a new product. |
| Public |  Public data is the least sensitive data used by the company and would cause the least harm if disclosed. This could be anything from data used for marketing to the number of employees in the company. |
