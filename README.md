# CIS Definition
Covisint Identity Service (CIS) is a cloud based identity management tool which handles the functionalities like Identity Management, Authorization, Authentication, Identity Verification, Identity Broker, Security Token Services supporting various industry leading protocols like SAML 1.1/2.0, WS-FED 1.1, OPEN ID 2.0, OAuth 1.0/2.0.

It integrates complex systems reaching cloud applications, manage multiple IDs, passwords and integrates across a wide network of constituents, perform administration, and reporting.

* Covisint CIS is a cloud-based Identity and Access Management application.  CIS is a multitenant SaaS solution that insulates businesses from the cost and complexity of the do-it-yourself approach to security. Covisint centralizes and automates the process of securing and managing digital identities inside and outside your organization, enabling you to manage and control access to internal and cloud applications and information for customers, business partners and suppliers. 
* With a single connection to Covisint, customers can drastically reduce the burden of complex systems integration, management of multiple IDs and passwords, time-consuming reporting, security rules enforcement and help desk administration.
Users can be easily administered with automated & configurable workflow management and provisioned to services, applications and content from sources across many sources, including cloud-based services utilized within a particular customer ecosystem.
* CIS delivers a security framework for securely accessing resources across multiple secure domains, with a single authentication step and the ability to accept inbound federated identities as well as a mobile security framework.
* As a multitenant SaaS application, CIS has a robust set of features out of the box.  This document identifies key features included in the application.

## Core Functional Components
1. Registry
    * CIS data store
    * Synchronization between CIS Registry and one or more data stores systems
    * Data store for:
        * Users 
        * Services
        * Groups
        * Roles
        * Orgs
        * Realm
    * Point of reconciliation for source systems that feed CIS
    * The CIS authoritative system of record for connections
    * Reporting originates from Registry data
    * Workflow function is part of Registry component
2. User Authentication Services
    * Everything required to ensure that a user attempting to access the system is who they say they are
    * Function is to authenticate users
    * Collects User Credential
    * Validates user against registry
    * Handles risk assessment
    * Supports multiple authentication mechanisms
        * Applies risk assessment as one method to determine authentication mechanism
    * Includes Service Provider functionality (IDP proxy model)
3. Federation Services (IDP and SP)
    * Secure communication of user information from the registry to an application
    * IDP Initiated Federation
    * SP Initiated Federation
        * Includes Service Authorization Check
    * Name Identifier mapping for services
    * Attribute Mapping for Services (SP/RP)
4. Provisioning Services 
    * Service for provisioning / de-provisioning of access to services based on data stored in the Registry
    * Authorization management where supported by Service Provider or Service Package
    * Capable of provisioning to any connected application or Service Provider a beyond set of connected SSO applications
    * Just in Time provisioning supported (JIT)
    * Ahead of Time provisioning supported (AOT)
    * Primarily unidirectional from Registry to application or service
    * Capable of synchronization between application or service and the Registry where application/service can notify synchronization engine


