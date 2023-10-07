# Decentralized Subscription Protocol
Welcome to the Decentralized Subscription Protocol project! This protocol is designed as a revolutionary solution for subscription-based services, offering a decentralized approach that ensures anonymity, security, and ease of use. With a focus on overcoming the limitations of traditional payment systems, the protocol offers a trustless environment where both service providers and subscribers can engage in transactions with confidence.

Whether you are a developer, a subscriber, or an application owner, this documentation will guide you through the features, architecture, and contribution guidelines of the Decentralized Subscription Protocol. Please read on to explore how the protocol enables a seamless subscription experience while upholding the principles of decentralization.
## Documentation

### Overview and Objectives
The protocol aims to provide an efficient, decentralized subscription system that addresses the drawbacks of conventional payment systems, such as identification requirements, compliance with varied app rules, and the risk of payment channels being closed by a central authority. The protocol facilitates anonymous, decentralized subscriptions, assuring apps and users of seamless transactions through smart contracts.

#### Objectives:
- Implement a straightforward protocol for decentralized subscription services.
- Enable anonymous transactions for both apps and users.
- Guarantee secure subscription purchases and renewals through smart contracts.
- Initially focus on supporting Telegram mini-apps with plans for broader application.

### System Architecture
The system consists of three integrated projects:

1. **Smart Contracts:** 
   - *Subscription Contract:* Manages an individual subscription, allowing for renewal, rating, and red flagging (active subscriptions only).
   - *Subscription Collection Contract:* Represents an app and its subscription collections, storing user Telegram IDs, minting subscriptions, collecting ratings and red flags, processing subscription payments, allowing withdrawals, and defining subscription plans. This contract is frozen if over 30% of active subscriptions send a red flag, disabling its mint and withdraw functions.
   - *Protocol App Collection Contract:* Mints subscription collection contracts, collects protocol fees, and has functions to release or block frozen apps.
2. **Frontend:**
   - *App Owner Interface:* A web page and Telegram app (tapp) allowing app owners to define subscription collections, initiate mint transactions, and manage contracts for withdrawals and plan adjustments.
   - *Subscriber Interface:* A web page and tapp for users to mint subscriptions, leave ratings, send red flag requests, and renew subscriptions. 
   - *Integration Library/Widget:* Helps facilitate easier user and app owner interactions with the protocol.
3. **Backend:** The backend stores data for apps and users to simplify contract location and management.

### User Roles and Responsibilities
There are two primary user types:
1. **App Users (Subscribers):** Individuals who purchase and use app subscriptions.
2. **App Owners:** Entities that own and manage the apps and their subscription plans.

#### Responsibilities:
- **App Users:**
  - Purchase and renew subscriptions.
  - Rate and red flag subscriptions as necessary.
- **App Owners:**
  - Define and manage subscription collections and plans.
  - Initiate mint transactions.
  - Manage contract withdrawals and plan adjustments.

### Subscription Workflow
The subscription process begins with each app creating its unique Subscription Collection Contract through the protocol. This contract serves as the foundation for user subscriptions, allowing individuals to mint their subscriptions based on the plans defined by the app. The entire workflow is streamlined and user-friendly, accessible through various platforms including our dedicated Telegram app (tapp), official webpage, or the conveniently designed widget. This multi-platform approach ensures a smooth and intuitive experience for users while providing flexibility for app owners in managing subscription plans and user interactions.

### Security Measures
Thanks to the protocol's decentralized nature, both users and apps can trust that their funds are secure. The system is designed to be trustless, with only one centralized decision-making point: determining whether a frozen app should be freed or blocked. This decision is based on our reputation system and fee channel, ensuring the best possible outcomes for all parties involved.

### Mission
Implement a simple, anonymous, and secure protocol to facilitate decentralized subscription services for apps, starting with Telegram mini-apps, ensuring reliable transactions for both app owners and users.

## Contribution Guidelines
We warmly welcome and appreciate contributions from the community! To ensure a productive and efficient collaboration, please follow the guidelines below:

### Reporting Issues:
- Check if the issue has already been reported by searching the repository's existing issues.
- Provide a detailed description of the issue, including steps to reproduce, expected behavior, and actual behavior.
- Attach screenshots, logs, or any additional information that may help in resolving the issue.

### Feature Requests:
- Clearly describe the feature you would like to see implemented and explain the value it would add to the project.
- Provide examples or references to other projects, if applicable.

### Pull Requests:
- Fork the repository and create a new branch from which you want to contribute.
- Ensure your code follows the project’s coding conventions and style guides.
- Write meaningful commit messages and provide detailed comments on your code.
- Before submitting a pull request, rebase your branch onto the latest version of the branch you forked from.
- Include relevant unit tests for your feature or bug fix.

### Code of Conduct:
- Engage in respectful and constructive conversation.
- Avoid discriminatory, offensive, or inappropriate language and behavior.
- Respect the decisions of project maintainers and contributors.

### Getting Help:
- If you have a question or need clarification on contributing, feel free to reach out through the project's communication channels.

### Acknowledgments:
- Contributors who successfully have their pull requests merged will be acknowledged in the project's documentation.

By following these guidelines, you'll help maintain a collaborative and open environment, making it easier for everyone to contribute to the project. Thank you for considering contributing to the Decentralized Subscription Protocol!
