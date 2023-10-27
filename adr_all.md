# Architectural Decision Records of Hardware Integration, Database Storage, Navigation Strategy, and UI Tools for developing Codinggo

By Peaky Coders (Edward M., Sumandeep K., Japsimran N., and Iza L.)


## Table of contents
[Hardware Integration ADR 1](#_Toc431212768)

[Status 1](#_Toc580028659)

[Context 1](#_Toc2005597699)

[Decision 1](#_Toc442346398)

[Rationale 1](#_Toc1260919754)

[Consequences 2](#_Toc816053478)

[Local Database Storage ADR 2](#_Toc639110015)

[Title: 2](#_Toc1699700328)

[Context 2](#_Toc543150049)

[Decision Considerations 2](#_Toc2052040125)

[Considered Options 2](#_Toc109280959)

[Rationale 2](#_Toc488726984)

[Local (Unencrypted) Data Storage 3](#_Toc1643599989)

[Consequences 3](#_Toc1241908920)

[Notes 3](#_Toc1164999118)

[Local (Encrypted): 3](#_Toc875236930)

[Navigation Strategy ADR 3](#_Toc825058156)

[Title: 3](#_Toc506799068)

[Context 3](#_Toc205371461)

[Decision 3](#_Toc544467328)

[Rationale 4](#_Toc1202850783)

[Consequences 4](#_Toc1279334048)

[Positive: 4](#_Toc1347831091)

[Negative: 4](#_Toc1382252694)

[Conclusion 4](#_Toc305948194)

[UI (User Interface) Tool ADR 5](#_Toc1669477789)

[Status 5](#_Toc986929226)

[Context 5](#_Toc1033300147)

[Rationale 5](#_Toc1827642034)

[Consequences 5](#_Toc319826107)

[Notes 5](#_Toc283369284)

[Most popular UI tools 5](#_Toc697101127)

## **Hardware Integration ADR**

### **Status**

Proposed. The team needs to evaluate the decision

### **Context**

The goal of the "Codinggo" mobile app project is to give novices access to an engaging platform for coding instruction. It is necessary to take into account the integration of particular hardware components in order to improve the user experience and offer extra functionality. The following hardware components are proposed for integration: \* GPS \* Speaker \* Fingerprint scanner

### **Decision**

After careful consideration, our team decided to integrate the following hardware components into the "Codinggo" mobile app: \* GPS: To enable features depending on the user's geographic location and to offer location-based services for customized learning experiences. \* Speaker: The speaker's role is to support audio-based learning by giving voice guidance for coding tasks and quizzes. \* Fingerprint Scanner: To improve user data security and offer a practical means of authentication for gaining access to private data within the application.

### **Rationale**

- GPS integration:
  - Learning materials that are tailored to the user's location
  - Increased user involvement with events and challenges that are location specific.
  - By offering pertinent local coding resources, the user experience was enhanced.
- Speaker integration:
  - Serving users with visual impairments and those with a variety of learning preferences, such as auditory learners.
  - Making interactive audio-tutorials available for better understanding.
  - Offering people in diverse settings other forms of learning.
- Fingerprint Integration:
  - Strict user authentication and protection protocols for data.
  - Simplified app access improves user comfort and lowers friction.
  - An increase in user confidence in the security and privacy policies of the app.

### **Consequences**

The process of developing an app may become more difficult if hardware components are integrated, and more resources may be needed for testing and implementation. Additionally, it can result in a rise in battery utilization, particularly while using GPS. Furthermore, it is important to give careful consideration to compatibility difficulties with varying device types and operating systems in order to guarantee a smooth user experience across several platforms.

## **Local Database Storage ADR**

**Title:** Choosing local(encrypted) as Database Storage for "Codinggo".

**Status**

Proposed. Under evaluation by the team.

### **Context**

We need to decide the appropriate database storage solution to manage user data and progress for our app "Codinggo". The primary focus of the project is to teach coding concepts through interactive exercises and quizzes. Among various options available, we are considering local(unencrypted) as a possible choice.

### **Decision Considerations**

- Ease of use and maintenance
- Performance and scalability
- Offline Access
- Cost and licensing

### **Considered Options**

- Local (encrypted)
- Local (unencrypted)
- Remote
- None

### **Rationale**

#### **Local (Unencrypted) Data Storage**

Storing user data locally in an unencrypted format simplifies the data storage and implementation. It ensures offline access for the user and carries on with their learning journey, even when they are offline. Unlike encrypted storage, there are fewer data protection compliance concerns when data is stored locally in an unencrypted manner. Unencrypted data storage can be a better option as we are not dealing with any sensitive information like payment options. Moreover, it lowers the cost of server infrastructure which might be needed in remote storage. Remote storage can be more complex to set up and maintain as compared to local unencrypted data storage.

### **Consequences**

- Positive: It will require less development effort and complexity. Users can access their progress offline, improving the app's usability. It doesn't rely on faraway servers; it saves money on server infrastructure.
- Negatives: It may compromise data security and privacy, but in our app "Codinggo", we are not storing any sensitive user information. Additionally, if a user loses their device or the data is corrupted, their progress and information may be lost, as there are no remote backups.

### **Notes**

_Local (Encrypted):_ Encrypting user data before storing it locally on the user's device to protect it.
_Local Data Storage:_ This refers to storing user data locally, without encryption, on the user's device.
_Remote:_ Keeping user information on a distant server.
_None:_ Deciding against permanently storing user data.

## **Navigation Strategy ADR**

**Title:** Decision to Incorporate Conventional Navigation Strategy

### **Context**

Peaky Coders is considering a conventional development strategy to create a simple game application for android devices.

### **Decision**

The team will incorporate a navigation strategy in creating a simple game application for android mobiles, utilizing a standard approach by implementing conventional designs.

### **Rationale**

Navigation strategy will help solidify a practical yet user-friendly way for users to navigate through an application. If used correctly, this will simplify the overall design reducing the redundancy and navigation time while utilizing a modern interface. Additionally, it will better help users to visually digest the content of the application. This will enhance their experience and the quality of the application.

### **Consequences**

#### **Positive:**

- This will help with planning in the development stage
- Enhance user experience
- Simplified design will result in quicker access to the application's content
- Adequate design
- Can be designed for users with disabilities to become more accessible
- Wide range of elements that can be implemented
- Offers maintainability

#### **Negative:**

- Potential misuse of implementation can cause a cluttered design
- Potential confusion from overwhelming and inconsistent patterns in overall design
- Adding features with insignificant purpose or impractical use
- Color imbalances due to poor color choice
- Potential maintenance burden due to the growing complexity as the app grows

### **Conclusion**

Weighing the pros with the cons, incorporating a navigation strategy will further the development, planning and enhancement process in terms of quality and delivery of the application. Therefore, the team has decided to approve of this decision in order to utilize the navigation strategy.

## **UI (User Interface) Tool ADR**

## **Status**

Proposed. Under evaluation by the team.

### **Context**

Codinggo is the mobile app's name which is a project that aims to provide coding education for those learning how to code. The project focuses on teaching coding concepts through interactive exercises or quizzes. Therefore, making the user interface is a critical component of the project. And so, before starting the coding phase, we, as a team, need to decide on which UI Tools to use with react native.

### **Rationale**

React Native Elements seems the most suitable for the team and project codinggo:

1. Functionality: comprehensive and includes the standard UI elements. Offers an extensive set of components making development easier and faster.
2. Ease of use: It is said to be easy to use by many developers online. The library has ready to use components and are customizable; which allows the tools to be molded to match the branding and design of the app.
3. Community support: Since there is available documentation and discussions online, the team can find answers to questions and stay updated with the best practices of using React Native Elements.

### **Consequences**

Possible roadblocks and things to consider when using react native element:

1. Learning curve: We as a team will need to become proficient in using React Native Element components and their API. We will need initial learning and training.
2. Maintenance: Need to keep track of updates to ensure that the app remains compatible with the recent changes or bug fixes.
3. Code Complexity: Increasing customization of components or using many customized components may lead to more complexity in the codebase. We will have to find the balance for customization and maintainability.

### **Notes**

#### **Most popular UI tools**

1. [Native Base](https://nativebase.io/) is a component library for building UI in iOS, android, and even the web. It has the most common UI elements for apps. It is highly customizable. is a component library for building UI in iOS, android, and even the web. It has the most common UI elements for apps. It is highly customizable.
2. [React Native Elements](https://reactnativeelements.com/) is a react native framework, cross-platform and customizable.
3. [UI Kitten](https://akveo.github.io/react-native-ui-kitten/) is another react-native framework. It is open source, also has ready to use components, and is cross-platform.
4.  [React-native-paper](https://reactnativepaper.com/%22%20/o%20%22https://reactnativepaper.com/) is a library of customizable and production-ready components. Also, open source.
5. [Shoutem UI](https://github.com/shoutem/ui%22%20/o%20%22https://github.com/shoutem/ui) is a collection of components that can be styled to fit a react native app for iOS and/or Android.
6. [Restyle ](https://github.com/Shopify/restyle)is a library by shopify for building UI components in react native with typescript.
7. [Tamagui](https://tamagui.dev/) is a complete UI kit consisting of the most common components and some more. It is cross-platform, highly customizable, and open source. Seems new.