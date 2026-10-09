# HAMPINESS : Hamper Ordering System 
An Information Systems Analysis and Design (ISAD) project for a mobile platform that connects customers with hamper vendors. The project covers business problems, process and data models, user interface designs, and a proposed system architecture.
- **Course**: Information Systems Analysis and Design — ISYS6893003
- **University**: BINUS University
- **Semester**: Odd Semester 2025/2026
- **Project scope**: Academic case study, system analysis, and design
## Project Overview
Hampiness brings hamper browsing, ordering, and delivery arrangements into one platform. Customers can choose packages for birthdays, holidays, corporate events, and other occasions, while vendors manage their products and hamper packages.
The case study focuses on problems that make ordering less convenient and vendor operations harder to manage: unclear product information, inconsistent catalogue entries, delayed notifications, and uncertainty about stock and delivery status.
Our group documented the system's requirements and workflows, modelled how its components interact, and designed screens for customers, vendors, and administrators.
## Problem Identification 
Two Fishbone Diagrams examine the causes of lower customer satisfaction and inefficient vendor operations.
- **Customer experience**: Unclear package details, limited personalisation, an unintuitive ordering process, and a lack of reliable stock and delivery information.
- **Vendor operations**: Difficult product and package forms, no consistent guidance for entering catalogue information, and delayed responses to incoming orders.
These findings provide the context for the ordering, catalogue management, and reporting workflows in the design.

<img width="869" height="684" alt="image" src="https://github.com/user-attachments/assets/31d3eace-18ee-46a3-8223-04812efad090" />
<img width="958" height="732" alt="image" src="https://github.com/user-attachments/assets/d4332950-e5ae-47cc-916c-c2954ca5858b" />

## Users and Main Workflows
| User | Main Workflows |
|----|----|
| **Customer** | Register an account, browse vendors and hamper categories, place an order, make a payment, and submit a review. |
| **Vendor** | Add products, create hamper packages, receive order notifications, and submit delivery confirmation. |
| **Administrator** | Prepare ordering-trend reports and transaction activity summaries. |

The ordering flow starts with vendor and package selection, followed by the cart, checkout, and payment. Once payment is successful, the vendor prepares the packages and follows the requested delivery schedule.
The case study specifies several rules that shape this flow:
- One order can contain several hamper packages, each with its own delivery date and time.
- Payment is made by bank transfer to Hampiness within one hour. Unpaid orders are cancelled automatically.
- Vendors submit a delivery photo and an optional note to complete the delivery confirmation.
- Customers submit a rating from 1 to 5 and a written review, with an optional photo.

## Process and Data Modelling
The Context Diagram defines the system boundary and the information exchanged with customers, vendors, and administrators.
The DFD Level 0 breaks the system into six processes: account management, catalogue management, ordering, delivery, reviews, and reporting. It shows how these processes exchange information with the relevant data stores.
<img width="1618" height="876" alt="image" src="https://github.com/user-attachments/assets/c29a15ac-0d32-4d16-8aeb-5c16f57a0003" />
<img width="1786" height="886" alt="image" src="https://github.com/user-attachments/assets/efbb1c15-5f81-4ac0-8899-daf2b53b19ac" />

## Object Oriented Analysis and Design
The UML models describe the system from different views :
  
| Model | What it covers | 
| --- | --- |
| **Use Case Diagram** | Eight use cases across the customer, vendor, and administrator roles. |
| **Use Case Descriptions** | Scenarios, actors, triggers, preconditions, postconditions, activity flows, and exception conditions for all eight use cases. |
| **Class Diagram** | Classes, attributes, methods, and relationships for customers, vendors, hampers, orders, order details, reviews, and related forms. |
| **Sequence Diagrams** | Interactions between actors, controllers, and objects for each of the eight use cases. |
| **Activity Diagrams** | The steps users and the system follow during each main workflow. |
| **State Transition Diagrams** | State changes for orders, package availability, and product entry. |

<img width="1180" height="886" alt="image" src="https://github.com/user-attachments/assets/2f4eb16a-38df-4801-9dee-92a161b638d2" />
Each diagram is provided as a separate file in this repository. The preview above shows one of the UML models.

## User Interface Design 
The Figma designs show the main inputs and outputs for the three user roles.
- **Customer screens:** Registration, vendor and category browsing, package selection, cart, checkout, and payment status.
- **Vendor screens**: Product entry, package creation, order history, and delivery confirmation with a photo upload.
- **Administrator screens**: Report input forms and a reporting dashboard showing ordering trends and transaction summaries.
<img width="758" height="820" alt="image" src="https://github.com/user-attachments/assets/18f67d97-b133-4d16-907c-89f50245b38f" />
<img width="870" height="596" alt="image" src="https://github.com/user-attachments/assets/b3e68ad6-4b1e-4816-b932-d4231474d66e" />

## Project Links 
- **Figma**: [View the interface design](https://tinyurl.com/figma-hampiness)
- **Draw.io**:[view the diagrams](https://tinyurl.com/DrawIo-Diagram-File)
## Proposed System Architecture
The report proposes a three-tier client/server architecture:
| Tier | Responsbility | 
| ---- | ---- |
| **Presentation** | Mobile interfaces for accessing the system and entering or viewing information. |
| **Application** | Business logic for catalogue management, orders, reviews, and reporting. Java is proposed for this layer. |
| **Data** | Storage for user, product, package, and transaction records. MySQL is proposed for this layer. |

## Contributors 
- Nacito Florisen Astari
- Ahmad Alfakhridzi Mirza
- Putu Gde Wibi Adhidarma
- Kepin Simatupang


