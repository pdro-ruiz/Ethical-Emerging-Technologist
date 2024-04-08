# Ethics and Privacy in Data Technology

## Data Privacy and Protection of PII

### Data Privacy

- **Definition:** The ability to control the sharing, identifiability, and the image created by personal data.
- **Key Aspects:**
  - Selectively sharing data.
  - Withdrawing from unwanted interactions.
  - Control over identifiability in online and offline activities.

### Personally Identifiable Information (PII)

- **Definition:** Data that uniquely identifies an individual.
- **Importance:** Protecting PII is central to privacy.

### Types of PII

1. **Direct Identifiers:**
   - Unique by themselves (e.g., Social Security numbers, passport).
   - Linked to personal properties (e.g., vehicle VIN).

2. **Biometric Data:**
   - Fingerprints, facial image, facial geometry, voice signatures.

3. **Non-sensitive or Indirect PII:**
   - Public data (e.g., full name, address, phone number).
   - Considered non-sensitive due to their public availability.

4. **Combined Data:**
   - Combination of data that can become PII.
   - Example: Name + date and place of birth = Unique identification.

### Context in Identification

- **PII Determination:** Depends on context, not just the nature of the data.
- **Importance of Context:** Individual data may be harmless, but dangerous when combined.

### International Comparison

- **PII in the US:** Specific term for identifying data.
- **Personal Data in Europe (GDPR):**
  - Broader definition than PII.
  - Any data that can directly or indirectly identify a person.

### Risks and Concerns

- **Misuse Risk:** Unauthorized access to PII can have serious consequences.
- **Risk Consideration:** It's crucial to assess the risks of sharing PII.

### Implications for Privacy Protection

- Effective protection of PII and conscious management of data privacy are fundamental to mitigate risks and ensure individual confidentiality.




## Privacy Risks in IoT/Ambient Intelligence

### Introduction

- **Definition of Ambient Intelligence:** Networked IoT device systems designed to collect real-time data for personalized services.
- **Trend:** Increase in the number and type of IoT devices, making privacy choices harder.

### Main Risks

1. **Data Collection:**
   - Unknowns about what data are collected and their use.
   - Example: IoT thermostats capturing not just temperature but also IP addresses and geolocation.

2. **Data Transmission:**
   - Vulnerability due to lack of encryption in 90% of cases.
   - Risk of criminal inferences from data patterns.

3. **Data Storage:**
   - Concerns over storage security and retention policies.
   - Data linked to the individual indefinitely without a clear end-of-life plan.

4. **Data Access:**
   - Uncertainty over who has access and for what purposes.
   - Data shared or sold to third parties without consent.

### Specific Risks

- **IoT Device Security:**
  - Devices shipped with default passwords and minimal security measures.
  - Users have limited privacy control.

- **Surveillance and Tracking:**
  - Continuous and close monitoring by design.
  - Wearable devices tracking public actions via Wi-Fi and Bluetooth.

### Impact on Privacy

- **Erosion of Private Spaces:**
  - Transforming homes and vehicles into more public spaces.
  - Unilateral decisions by owners affect guests' privacy.




## Privacy Protection through Individual Authorization

### Informed Consent

- **Definition:** Voluntarily agreeing with full knowledge of the implications.
- **Origin:** Healthcare sector, extended to other areas.
- **Voluntariness:** Right to withdraw consent easily.

### Clarity in Privacy Policies

- **Problem:** Long, inaccessible policies filled with legal jargon.
- **Solutions:**
  - Nutrition Label Model: Clear and concise policies.
  - Creative Commons License: Three layers of policy (legal, human-readable, machine-readable).

### Opt-out vs. Opt-in

#### Opt-out (Voluntary Exclusion)

- Default policy; data collected unless otherwise indicated.
- Privacy burden falls on the individual.

### Opt-in (Voluntary Inclusion)

- No data collected without express permission.
- Implementation through checkboxes.

### Technological Authorization

- **Tools:**
  - Anonymous accounts for greater privacy.
  - Mute buttons for temporary control over data collection.
  - Privacy panels for selective management of shared data.

### Impact on Autonomy and Self-determination

- **Reflection:** Changes in consent perception and its effect on personal autonomy and self-determination in personal data management.



## Privacy Protection through Data Management

### Personal Data Management

- **Goal:** To make it difficult or impossible to identify the unique individual behind collected data.
- **Challenge:** Managing both direct and indirect identifiers.

### Key Strategies

1. **De-identification:**
   - **Process:** Preventing the disclosure of unique identity.
   - **Direct Identifiers:** Recognize a specific person by themselves.
   - **Indirect Identifiers:** Combine with other data to identify an individual.

2. **Pseudonymization:**
   - **Method:** Replacement of direct identifiers with temporary codes.
   - **Key Storage:** Secure and separate.
   - **Risk:** Possible reidentification, though minimal.

3. **Anonymization:**
   - **Process:** Removing or mathematically altering direct and indirect identifiers.
   - **Outcome:** Unrecognizable data, impossible to reidentify.
   - **Key Difference:** Personal data are not replaced; they are destroyed.

### Important Considerations

- **Reidentification Risk:** 
  - Pseudonymization: Present but reduced.
  - Anonymization: Completely eliminated.

- **Handling of Indirect Identifiers:** 
  - Pseudonymization: Remain, possibility of combining to identify.
  - Anonymization: Removed or altered, eliminating risk.




## Privacy by Design

### Origin and Fundamentals

- **Creator:** Ann Cavoukian, Information and Privacy Commissioner of Ontario, Canada.
- **Decade:** 1990s.
- **Concept:** Integrating privacy as a fundamental element in the design of technologies and organizational operations.

### Seven Foundational Principles

#### Proactive, Not Reactive; Preventive, Not Corrective

- Anticipate and prevent privacy risks before they occur.
- Example: Using diverse data sets from the start to prevent biases.

#### Privacy as the Default Setting

- Safeguard privacy without requiring user action.
- Example: Not sharing data beyond specified purposes without explicit consent.

#### Privacy Integrated into Design

- Incorporation of privacy into the development of software, systems, and business practices.
- Challenge: Often neglected in rapid software development.

#### Full Functionality – Positive-Sum, Not Zero-Sum

- Achieve privacy and business objectives without compromises.
- Benefit: Win-win solutions that don’t sacrifice privacy for revenue.

#### End-to-End Security – Full Lifecycle Protection

- Maintain security from data collection to destruction.
- Example: Encryption at all stages of the data lifecycle.

#### Visibility and Transparency – Keep it Open

- Inform all stakeholders about privacy practices and technologies.
- Builds trust through the clarity and accessibility of privacy policies.

#### Respect for User Privacy – User-Centric

- Prioritize the user in all decisions related to their data.
- Principle of treating users' data with the utmost care.

### Impact and Reception

- **Application:** Inspired the development of frameworks and regulations like the GDPR.
- **Critiques and Acceptance:** Despite criticisms, it has been fundamental in guiding the incorporation of privacy into technologies and operations.





## Differential Privacy

### Concept and Necessity

- **Definition:** A mathematical method that protects individual privacy in data sets.
- **Goal:** To enable statistical analysis without compromising individual privacy.

### Why It Is Necessary

- **Limitations of Other Methods:**
  - Encryption: Protects data but prevents analysis.
  - Anonymization: Can be circumvented to reidentify individuals.
  - Data Curation: Vulnerable to deidentification through smart queries.

### How It Works

1. **Mechanism:**
   - Adds random noise to the data to obscure the presence or absence of individuals.
   - Epsilon (ε): Privacy loss metric; lower ε, greater privacy.

2. **Application Example:**
   - Sensitive surveys: Uses randomization to create plausible deniability and protect responses.

3. **Local vs. Global Differential Privacy:**
   - **Local:** Noise is added before sending data to the database.
   - **Global:** Requires trust; noise is added during data analysis.

### Challenges

- **Privacy Loss with Multiple Accesses:**
  - More queries increase the risk of privacy loss.
  - Limit through a privacy budget to prevent excessive queries.

### Benefits

- **Secure Analysis:** Facilitates statistical analysis while preserving privacy.
- **Useful Data without

 Compromising Individuals:** Allows sharing aggregated data without risks.



## Types of Technological Contracts

### Introduction

- The acquisition and use of software, whether traditional or cloud-based, involve different types of legal contracts.

### Types of Contracts

#### End-User License Agreement (EULA)

- **Parties:** Software company and licensee (user).
- **Nature:** More akin to a lease than a purchase.
- **Purpose:** Establishes rights to use the software under specific terms, protecting the provider's intellectual property.
- **Protection:** Mainly for the software and its intellectual property.

#### Terms of Service Document

- **Parties:** Service provider and client (individual or organization).
- **Goal:** Protect the provider more than the client.
- **Content:** Limitations of liability, service use, privacy policy, payment details, opt-out option, arbitration processes.
- **Consequences:** Non-compliance can result in service denial.

#### Service Level Agreements (SLA)

- **Application:** External (business-customer) and internal (within departments of the same organization).
- **Purpose:** Precisely define provided services and expected performance standards.
- **Details:** Service objectives, requirements, responsibilities to meet objectives.
- **Focus:** Establishes clear expectations and responsibilities of both parties.

### Key Differentiation

- **EULA:** Focused on the right to use software by end-users.
- **Terms of Service:** Establishes the rules for using a service, with emphasis on the responsibilities and restrictions of the user.
- **SLA:** Specifies expected service levels, rights, and obligations of both the provider and the client, with an emphasis on service quality and availability.




## Smart Contracts

### Definition and Nature

- **Smart Contract:** A self-executing computer program with the terms of the agreement between parties directly written into code.
- **Storage:** On a blockchain, a secure distributed network.

### Function and Comparison to Traditional Contracts

- **Function:** Similar to traditional contracts in establishing agreement details.
- **Key Differences:**
  - Fully digital.
  - Eliminates the need for central authorities or external legal systems for enforcement.

#### Practical Example: Crowdfunding Platform

- **Traditional:** Requires a central authority (crowdfunding platform) to hold and manage funds.
- **With Smart Contracts:** Eliminates the central authority, automating transaction management.

### Technical Functioning

#### Stored on Blockchain

- **Contract Data:** Each block contains data (smart contract program), a unique hash, and the hash of the previous block.
- **Validation:** Changes in data alter the hash, impacting the chain's validity.

#### Security and Distribution

- **Blockchain:** Operates as a distributed ledger across multiple nodes.
- **Transparency and Security:** Each node has a complete copy, offering additional transparency and security.

### Advantages over Traditional Contracts

- **Automation:** Automatic execution based on fulfillment of coded conditions.
- **Transparency:** Every transaction is verifiable by all network participants.
- **Security:** Blockchain structure and consensus among nodes prevent unauthorized alterations.