Version: NAFATH-V3
Track: AI

## Overview
This project explores six technology topics needed to build a trustworthy AI assistant for public services. Software versioning helps teams manage changes safely. AI techniques help the assistant answer questions using reliable information. Mobile security protects connections between the app and its servers. Networking supports communication between connected devices. Cybersecurity helps defend the assistant against threats such as prompt injection. Data protection guides the safe handling of chat logs and personal information. These fields work together to make the assistant more secure, reliable, and easier to maintain. Developers must also test the system, review its sources, and consider privacy risks before deployment. Understanding Retrieval-Augmented Generation (RAG) is especially important because it helps the assistant use relevant external information while answering citizens’ questions.
The AI track focuses on Retrieval-Augmented Generation (RAG) and how it can reduce incorrect answers by grounding responses in relevant retrieved information.
## Software

Semantic Versioning uses MAJOR.MINOR.PATCH version numbers. Increase MAJOR when making an incompatible change to the public API. Increase MINOR when adding functionality in a backward-compatible way. Increase PATCH when making backward-compatible bug fixes. Following these rules helps developers understand the impact of a new release and decide whether their software needs changes before upgrading.

Resource: Semantic Versioning 2.0.0 - https://semver.org/

## AI
Retrieval-Augmented Generation (RAG) combines information retrieval with text generation. Before answering a question, the system retrieves relevant information from an external knowledge source and provides it to the language model as context. This can reduce incorrect answers by grounding responses in supporting information. However, RAG does not guarantee that every answer is correct. Retrieved documents may be outdated or irrelevant, and the model may still misunderstand the evidence. Sources and answers should therefore be checked.

Resource: Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks - https://arxiv.org/abs/2005.11401

## Mobile
Apple’s  App Transport Security (ATS) helps enforce secure network connections in iOS apps by requiring appropriate transport security, including HTTPS connections that meet Apple’s security requirements. If an app tries to connect to a plain HTTP endpoint, ATS generally blocks the connection unless an exception has been configured. Developers should use HTTPS and avoid unnecessary security exceptions, because unencrypted HTTP can expose data to interception or modification during transmission.

Resource: Preventing Insecure Network Connections - https://developer.apple.com/documentation/security/preventing-insecure-network-connections
## Networking
IPv4 uses 32-bit addresses, while IPv6 uses 128-bit addresses and provides a much larger address space. This matters as the number of connected phones, sensors, appliances, and other devices grows. IPv6 helps support many more uniquely addressable devices and includes improvements to modern network operation. Moving to IPv6 requires planning because IPv4 and IPv6 systems may need to operate together during a transition. Both protocols remain important to understand.

Resource: Internet Protocol, Version 6 (IPv6) Specification - https://www.rfc-editor.org/rfc/rfc8200

## Cybersecurity
Prompt injection occurs when untrusted instructions in a user prompt or external content try to manipulate an AI system into ignoring its intended instructions. Direct prompt injection comes from input supplied directly to the system. Indirect prompt injection can be hidden in content the system retrieves, such as a webpage or document. Risk can be reduced by treating retrieved content as untrusted, limiting tools and permissions, validating actions, and requiring human approval for sensitive operations.

Resource: OWASP Top 10 for Large Language Model Applications - https://owasp.org/www-project-top-10-for-large-language-model-applications/
## Data
Anonymization removes identifying information so that a person can no longer reasonably be identified from the data. Pseudonymization replaces direct identifiers with substitutes, but a person may still be identifiable using additional information. Therefore, pseudonymized information generally remains personal data and is still subject to data protection requirements. Truly anonymized data falls outside personal data protection rules when re-identification is no longer reasonably possible. Organizations should assess re-identification risks carefully before describing data as anonymous.

Resource: What is personal data? - https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/personal-information-what-is-it/what-is-personal-data/

## Misconception in My Track
A common misconception about AI is that using Retrieval-Augmented Generation (RAG) guarantees that an AI assistant will always provide correct answers. In reality, RAG supplies relevant external information to support generation, but retrieval can fail and the model can still produce incorrect statements. The paper Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks, in its Abstract, describes RAG as improving generation by combining retrieved passages with a generator; it does not establish that every generated answer is guaranteed to be true. Developers must still evaluate sources and verify important answers.

Resource: Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks - https://arxiv.org/abs/2005.11401
## Open Question
How can a public-service AI assistant provide helpful answers while protecting personal data and making it easy for people to verify the information it gives?
