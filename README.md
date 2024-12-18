# Requirement Analysis in Software Development.
The purpose of this repository is to state down the requirement analysis of an AIRBNB clone project by creating a detailed blueprint of the requirement analysis phase for a booking management system.

## What is Requirement Analysis?
Requirement analysis is an important phase in software development lifecycle where/ project teams gather, analyze and define the requirements of a software application. This process ensures that all stakeholders have a clear and mutual understanding of what the system should do and how it should perform.

## Why is Requirement Analysis Important?
Clarity and Understanding: It helps in understanding what the stakeholders expect from the software, reducing ambiguity.
Scope Definition: Clearly defines the scope of the project, which helps in preventing scope creep.
Basis for Design and Development: Provides a solid foundation for designing and developing the system.
Cost and Time Estimation: Facilitates accurate estimation of project cost, resources, and time.
Quality Assurance: Ensures that the final product meets the specified requirements, leading to higher customer satisfaction.

## Key Activities in Requirement Analysis.
1. Requirement Gathering
Engage with stakeholders to collect initial requirements.
Use various techniques like interviews, surveys, and workshops.

2. Requirement Elicitation
Refine and elaborate on the gathered requirements.
Use techniques like brainstorming, focus groups, and prototyping.

3. Requirement Documentation
Document the requirements in a detailed and structured format.
Use requirement specification documents, user stories, and use cases.

4. Requirement Analysis and Modeling
Analyze and prioritize the requirements.
Create models to visualize and understand the requirements.

5. Requirement Validation
Review and validate the requirements with stakeholders.
Define acceptance criteria and ensure traceability.

## Types of Requirements.

### Functional requirements
These are the specific features and functions that the system must support:

- User Management:
Users can create an account with email and password.
Admins can manage user roles and permissions.

- Booking Management:
Users can create, view, update, or cancel bookings.
Admins can view and manage all bookings across the system.

- Search and Filter:
Users can search for available slots, services, or locations.
Search results can be filtered by date, time, location, or service type.

- Payment Integration:
Users can make secure payments through integrated payment gateways.
Payment history is stored and accessible for users and admins.

- Notifications:
Users receive email or SMS notifications for booking confirmations, updates, and cancellations.
Admins are notified of new bookings or cancellations.

- Analytics Dashboard:
Admins can view insights such as the number of bookings, revenue, and user activity.

### Non-functional requirements
These define the quality and operational standards the system must meet:

- Performance:
The system should handle up to 10,000 concurrent users without significant latency.
API responses should not exceed 500ms on average under normal load.

- Scalability:
The system should be designed to scale horizontally to accommodate an increasing number of users and bookings.

- Security:
All sensitive data must be encrypted in transit and at rest.
Authentication and authorization must follow industry best practices (e.g., OAuth2.0, JWT).

- Usability:
The user interface should be responsive and accessible across devices.
The system must comply with accessibility standards like WCAG 2.1.

- Reliability and Availability:
The system should maintain 99.9% uptime.
Backups must be taken daily to ensure data recovery in case of system failure.

- Maintainability:
The codebase should follow clean coding standards and include comprehensive documentation.
Updates or fixes should be deployable with minimal downtime.

## Use Case Diagrams.
What are Use Case Diagrams?

Use case diagrams show how different users (actors) interact with the system to achieve specific goals (use cases).

- Creating Use Case Diagrams:
Identify actors (e.g., guest, registered user, admin).
Define use cases (e.g., search properties, book property, manage listings).
Draw interactions between actors and use cases.

- Benefits of Use Case Diagrams:
Provide a clear visual representation of system functionalities.
Help in identifying and organizing system requirements.
Facilitate communication among stakeholders and development team.

## Acceptance Criteria.

- Importance of Acceptance Criteria
Acceptance Criteria are essential in Requirement Analysis as they:

- Define Clear Goals: Specify exactly what a feature or functionality should achieve, eliminating ambiguity.
- Ensure Alignment: Help all stakeholders, including developers, testers, and product owners, align on what constitutes a “done” feature.
- Facilitate Testing: Provide a basis for writing test cases and verifying that the feature works as intended.
- Prevent Scope Creep: Limit additional, unplanned functionalities by setting explicit expectations.
- Example: Acceptance Criteria for the Checkout Feature.
  
### The Checkout Feature in the Booking Management System must satisfy the following conditions:

1) User Authentication:
Only authenticated users can proceed to the checkout process.
If a user is not authenticated, they should be redirected to the login page.

2) Booking Summary:
The checkout page must display a summary of the booking, including:
 - Service name
 - Booking date and time
 - Total cost

3) Payment Integration:
Users must have the option to pay using at least two payment methods (e.g., Credit Card and PayPal).
Payment must be processed securely, and sensitive data (e.g., card details) must not be stored on the platform.

4) Success Confirmation:
Upon successful payment, users should be redirected to a confirmation page displaying:
- Booking reference number
- Payment confirmation
- Details of the booking

5) Error Handling:
If a payment fails, users must see a clear error message and be allowed to retry.
Errors must not cause the application to crash or lose user data.

6) Responsiveness and Accessibility:
The checkout page must be mobile-friendly and accessible (complying with WCAG 2.1 standards).

7) Audit Logging:
All transactions must be logged for auditing purposes, including user ID, booking details, and payment status.
