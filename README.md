# Emergency-Ambulance-APP-Doc

**Proposal:**
1. Introduction:
The Emergency Ambulance App is a software engineering project aimed at providing a user-friendly and efficient solution for individuals in need of immediate medical assistance. The app will enable users to call for an ambulance with a single tap, locate the nearest hospitals via Google Maps, and connect directly to the chosen hospital's emergency number.

2. Scope:
The scope of this project includes the development of a mobile application for both Android and iOS platforms using Flutter. The app will integrate Google Maps API to display nearby hospitals, and it will feature a user interface for initiating ambulance requests and making direct calls to the selected nearest hospital.

3. Goal:
The primary goal of this project is to create a reliable and user-friendly mobile app that can:
-	Quickly connect users to the nearest hospital in case of emergencies.
-	Provide essential information about nearby hospitals.
-	Improve the overall emergency response process.
-	Save lives by reducing response times during critical situations.

4. Problems:
The problems that this app aims to address are:
-	Delayed access to emergency medical services.
-	Inefficient communication between users and hospitals.
-	Lack of information about nearby medical facilities during emergencies.


5. Use:
The Emergency Ambulance App will be used by:
-	Individuals in need of immediate medical assistance.
-	Bystanders who can assist someone in an emergency.
-	Hospitals and medical facilities that can receive and respond to ambulance requests.

6. Identify Stakeholders:
Stakeholders for this project include:
-	App developers: The team responsible for app development.
-	Clients: People who we’re making this app for.

7. Tasks:
The major tasks to accomplish within this project are:
-	Requirement analysis and specification.
-	App design and development.
-	Integration of Google Maps API.
-	User interface development.
-	Ambulance request functionality.
-	Emergency contact integration.
-	Testing and quality assurance.
-	Ongoing maintenance and updates.

8. Roles:
Project Manager: Responsible for overall project coordination.
Developers: Front-end and back-end developers for app development.
UI/UX Designer: To design a user-friendly and appealing interface.
Support Team: Handle user queries and issues.

9. Cost Estimate:
The project cost estimate includes development, testing, deployment, and ongoing maintenance. It also includes server hosting, and software licensing costs. The cost of fetching Google API will also be there.

10. Time Efficiency:
The project timeline is estimated as follows:
-	Requirement analysis and design: 20 days
-	Development and testing: 40 days
-	Deployment and launch: 10 days
-	Ongoing maintenance and updates: Continuous

The Emergency Ambulance App project is essential in addressing critical issues in accessing emergency medical services. It will significantly improve response times and save lives in emergency situations. The team is committed to delivering a high-quality, efficient, and reliable solution.


**Software Requirements Specification (SRS):**

1. Introduction 
1.1 Purpose 
This document outlines the software requirements of the Emergency Ambulance App. The 
app aims to facilitate quick and efficient emergency assistance requests, enabling the 
system to identify the user's location and nearby hospitals for prompt medical attention. 
1.2 Document Conventions 
In this document, the term "must" signify a mandatory requirement, "should" indicates a 
recommended practice, and "may" represents an optional feature. 
1.3 Intended Audience and Reading Suggestions 
This SRS is designed for developers, project managers, testers, and documentation writers. 
Developers will focus on system features and implementation details, while project 
managers will find information about project scope and constraints. Testers can refer to 
functional requirements, and documentation writers will use this document to create user 
manuals. 
1.4 Project Scope 
The Emergency Ambulance App aims to supplement existing emergency services by 
providing users with a user-friendly interface for emergency requests, location tracking, 
displaying nearby hospitals, real-time communication with emergency services, and 
receiving emergency alerts.

1.5 References - Lawrence Chung, "Software Engineering" - Amr Saafan - Requirements Specification Template - Online ambulance service 
2. Overall Description 
2.1 Product Perspective 
The Emergency Ambulance App is a standalone application that enhances emergency 
response by connecting users with nearby hospitals. It does not replace existing emergency 
services but complements them by providing timely information to users and healthcare 
providers. 
2.2 Product Features 
1. User-initiated Emergency Request 
Users can trigger an emergency request through the app. 
Priority: High 
2. Location Tracking 
The app will use GPS to determine the user's location. 
Priority: High 
3. Display Nearby Hospitals 
The app will identify and display a list of nearby hospitals. 
Priority: High
4. Real-time Communication with Emergency Services 
The app enables real-time communication between users and emergency services. 
Priority: High 
5. Emergency Alerts 
The app will let you set alerts for checkups at specific time. 
Priority: Low 
2.3 User Classes and Characteristics 
1. User Classes - General Users: Individuals using the app to request emergency assistance. 
2. Characteristics - Varying technical expertise. - Emergency situations may involve stress, so the interface should be simple 
and intuitive. 
2.4 Operating Environment 
The app will operate on both Android and iOS platforms. It requires Google map API to 
track locations and an internet connection for real-time location tracking. 
2.5 Design and Implementation Constraints 
The app must comply with local regulations regarding emergency services. GPS and 
internet connectivity are essential for location tracking and hospital information. 
Some constraints that we can face includes, Fetching google maps API and Finding the 
hospitals that are not present on the maps (This usually happens in the areas that are not 
fully developed.
2.6 User Documentation 
User documentation will include an onboarding guide that will guide you about usage of 
the app, explaining the app's features and emergency procedures. 
2.7 Assumptions and Dependencies 
The app assumes users have a functional GPS and internet connection. Dependencies 
include access to hospital databases for real-time information. 
3. System Features 
3.1 Emergency Request 
3.1.1 Description and Priority 
Users can trigger an emergency request through the app, signaling the need for 
urgent medical assistance. 
Priority: High 
3.1.2 Stimulus/Response Sequences - User clicks the emergency button. - App sends location data to the server. - Nearby hospitals will receive the request along with the location. - Confirmation message is displayed. 
3.1.3 Functional Requirements 
REQ-1: The app must provide a prominent and easily accessible emergency button.
3.2 Location Tracking 
3.2.1 Description and Priority 
The app will use GPS to determine the user's location for accurate emergency 
response. 
Priority: High 
3.2.2 Stimulus/Response Sequences - GPS is activated upon emergency request. - App continuously updates user location. 
3.2.3 Functional Requirements 
REQ-2: The app must access and use the device's GPS functionality. 
3.3 Display Nearby Hospitals 
3.3.1 Description and Priority 
The app will identify and display a list of nearby hospitals to assist users in 
emergencies. 
Priority: High 
3.3.2 Stimulus/Response Sequences - App sends location data to the server - Server returns a list of nearby hospitals - Hospitals are displayed on the app 
3.3.3 Functional Requirements 
REQ-3: The app must communicate with a server to obtain real-time hospital 
information.
3.4 Real-time Communication with Emergency Services 
3.4.1 Description and Priority 
The app enables real-time communication between users and emergency services, 
allowing users to speak directly to emergency personnel. 
Priority: High 
3.4.2 Stimulus/Response Sequences - User activates communication with emergency services. - Emergency services receive and respond to the user's communication. 
3.4.3 Functional Requirements 
REQ-4: The app must provide a real-time communication feature with emergency 
services. 
4. External Interface Requirements 
4.1 User Interfaces 
The app will have a simple and intuitive user interface with a prominent emergency button. 
A map displaying user location and nearby hospitals will be included. 
4.2 Hardware Interfaces 
The app requires access to the device's GPS functionality. 
4.3 Software Interfaces 
The app will communicate with a server to obtain hospital information.
4.4 Communications Interfaces 
The app will require internet connectivity for real-time communication with the server. 
5. Other Nonfunctional Requirements 
5.1 Performance Requirements 
The app must provide real-time location tracking with minimal latency. 
5.2 Safety Requirements 
The app must comply with local safety regulations for emergency services. 
5.3 Security Requirements 
User data, especially location information, must be securely transmitted and stored. 
5.4 Software Quality Attributes 
The app should prioritize reliability, usability, and responsiveness. 
6. Other Requirements 
6.1 Medical Information Input 
6.1.1 Description 
The app should incorporate a user-friendly interface that allows users to input and 
manage their relevant medical information. This feature is crucial for enhancing 
emergency response efficiency, as it equips emergency services with critical data 
during an incident.
6.1.2 User Interface 
The medical information input interface should be intuitive, guiding users to provide 
necessary details without confusion. It should include fields for key medical 
information, such as allergies, existing medical conditions, current medications, and 
emergency contacts. 
6.1.3 Data Security 
To ensure user privacy and comply with healthcare data regulations, the app must 
implement robust security measures. Medical information entered by users should 
be encrypted during transmission and storage, and access should be restricted to 
authorized personnel only. 
6.1.4 Accessibility 
The medical information input feature should be easily accessible from the app's 
main menu or user profile section. Users should be able to review and update their 
medical information at any time, ensuring the data remains accurate and up-to-date. 
6.1.5 Integration with Emergency Services 
The inputted medical information should seamlessly integrate with emergency 
services' systems. Emergency responders should have quick access to this 
information when responding to a user's emergency request, enabling them to make 
informed decisions about medical care. 
6.1.6 Notifications for Updated Information 
Users should receive periodic reminders to review and update their medical 
information. Timely updates are essential to ensure that emergency services have 
the most current and relevant data during an emergency.
6.1.7 Offline Functionality 
The app should allow users to input and save medical information even when 
offline. The data entered offline should sync with the server once the device regains 
an internet connection. 
Appendix A: Glossary 
GPS: Global Positioning System 
GPS is a satellite-based navigation system that provides location and time information 
anywhere on Earth where there is an unobstructed line of sight to four or more GPS 
satellites. 
Appendix B: Analysis Models 
No analysis models are included in this version of the SRS. The nature of the Emergency 
Ambulance App does not necessitate the inclusion of specific analysis models at this stage. 
However, as the project progresses, additional models may be introduced to enhance 
understanding and documentation. 
Appendix C: Issues List  
This is a dynamic list of the open requirements issues that remain to be resolved, including 
TBDs, pending decisions, information that is needed, conflicts awaiting resolution, and the 
like.


**Design Documentation**

Index
1. Introduction 
    1.1 Purpose
    1.2 Scope
    2. Activity Diagram 
    2.1 Overview
    2.2 Activity Diagram
        Figure 1: Activity Diagram
    3. Sequence Diagram
    3.1 Overview
    3.2 Sequence Diagram
        Figure 2: Sequence Diagram
    4. Object Diagram 
    4.1 Overview
    4.2 Object Diagram
        Figure 3: Object Diagram
    5. Class Diagram
    5.1 Overview
    5.2 Class Diagram
        Figure 4: Class Diagram
    6. Conclusion 

1. Introduction
1.1 Purpose
The purpose of the Emergency Ambulance App is to provide a seamless and efficient solution for users in need of immediate medical assistance. This document outlines the design details of the mobile application, focusing on user interactions, system processes, and data structures.
1.2 Scope
The scope of this project involves the development of a user-friendly Flutter-based mobile app for both Android and iOS platforms. Key functionalities include:
•	Initiating ambulance requests.
•	Utilizing Google Maps API for hospital location.
•	Enabling direct communication with selected hospitals.
•	
2. Activity Diagram
2.1 Overview

 The Activity Diagram for the Emergency Ambulance
App delineates the workflow for users during emergency scenarios. The process
initiates with the user triggering an emergency request, prompting the app to
verify the user's location through GPS. After determining the location, the app
proceeds to communicate with nearby hospitals, displaying a list of available
options. A decision point is incorporated, enabling users to choose a specific
hospital for assistance. Following this decision, the app establishes real-time
communication with the selected hospital, facilitating direct interaction
between users and emergency services. The process concludes after providing
confirmation to the user, ensuring a clear visualization of the sequential
activities in the emergency response system.

2.2 Activity Diagram
![image](https://github.com/Ammarxsaqib/Emergency-Ambulance-APP-Doc/assets/100796073/dedee803-ced7-4383-a53e-24e5979a1519)

 
3. Sequence Diagram
3.1 Overview
•	The sequence initiates with the user triggering the "Initiate Emergency Request" operation.
•	The Emergency Request Processor processes the request and sends a synchronous message to the location tracker component to "Determine User Location".
•	Upon receiving the "Determine User Location" message, the location tracker utilizes GPS to ascertain the user's current location.
•	The determined location is then forwarded to the Hospital locator component.
•	The Hospital Locator processes the user's location and sends a synchronous message to the Display Hospitals component to "Show Nearby Hospitals."
•	After the user views the nearby hospitals, a decision point allows the user to select a specific hospital for assistance.
•	The selected hospital information is then conveyed to the Emergency Services Communication component.
•	Real-time communication is established with the selected hospital, allowing direct interaction between the user and emergency services.
•	Following the communication, a synchronous message is sent to the user for confirmation.
•	The user decides whether to proceed with the chosen hospital or cancel the request.
•	The sequence concludes with a confirmation message or cancellation acknowledgment, providing a detailed technical overview of the emergency response system's dynamic interactions.

3.2 Sequence Diagram
![image](https://github.com/Ammarxsaqib/Emergency-Ambulance-APP-Doc/assets/100796073/b4f23335-3f9d-42bb-b9f3-ae1f6a38b4d8)

 
4. Object Diagram
4.1 Overview
The Object Diagram provides a static snapshot of the Emergency Ambulance App, emphasizing the relationships and interactions among key objects within the system. Objects such as users, image processors, medical images, and patient information are depicted, showcasing how they are related and interconnected. The Object Diagram offers insights into the structure of the system at a specific point in time, showcasing the associations and attributes of each object. This static view aids in understanding the relationships that contribute to the overall functionality of the app, providing a foundation for developers to implement and maintain the system.
4.2 Object Diagram
![image](https://github.com/Ammarxsaqib/Emergency-Ambulance-APP-Doc/assets/100796073/87389058-aac5-44d4-9435-d82c766a9f07)

 
5. Class Diagram
5.1 Overview
The Class Diagram presents a holistic representation of the structure of the Emergency Ambulance App, capturing the relationships, compositions, and generalizations among essential classes involved in the application. It outlines key classes such as User, Location Tracker, Hospital, and Communication Module, showcasing their attributes and associations. The Class Diagram serves as a blueprint for system implementation, providing a comprehensive overview of the entities and their interactions. It aids in understanding the organization of the application's components, facilitating modular development, and ensuring scalability. The Class Diagram is a foundational reference for developers, enabling them to implement the system with a clear understanding of its structure and relationships.

6. Conclusion
In conclusion, the design of the Emergency Ambulance App aims to prioritize simplicity, efficiency, and reliability. The outlined diagrams and structures ensure a user-friendly experience and seamless interactions during emergencies. Ongoing maintenance and updates will be crucial to adapting to evolving standards and user needs.


**Test Case Documentation:**

1. Introduction:
The Test Case Documentation for the Emergency Ambulance App is a comprehensive examination of various features to ensure the application's reliability, security, and efficacy. Test scenarios encompass emergency request initiation, location tracking, communication with hospitals, and user interface responsiveness.

**2. Test Case Scenarios (Black-box and Grey-Box Testing):**
**2.1 Emergency Request Scenario:**
Test Case ID	ERS_TC001
Test Case Description	Verify the functionality of initiating a successful emergency request in the Emergency Ambulance App from a user's perspective.
Module to be tested	Emergency Request (Requirement ID: REQ-EMR-001)
Test Data	Valid user login credentials, installed app, GPS-enabled device
Test Steps	
•	Open the Emergency Ambulance App. 
•	Ensure successful login.
•	Navigate to the "Emergency Request" module. 
•	Tap on the emergency button. 
•	Verify that the app accurately sends the user's location to the server.
•	Confirm nearby hospitals received the emergency request.
•	 Choose a hospital and verify the initiation of real-time communication.
•	Receive and confirm a confirmation message.
Expected Results	Immediate communication and a seamless start to the emergency request procedure. A confirmation message is received promptly, indicating the successful initiation of communication.
Actual Results	Actual Results matched the expected results.
Results	Pass
Comments	If the test fails, provide detailed information on the observed issues. Evaluate the user experience and ensure that the emergency request process aligns with usability standards. Verify that the system responds appropriately to different user inputs.
Test Case 1: This test case outlines the test steps, expected results, and actual results for verifying the initiation of a successful emergency request in the Emergency Ambulance App. The test focuses on the user's perspective, covering various steps from app opening to real-time communication initiation.

**2.2 Location Tracking Scenario:**
   
Test Case ID	LTS_TC001
Test Case Description	Verify the functionality of accurate position designation in the Emergency Ambulance App from a user's perspective.
Module to be Tested	Location Tracking (Requirement ID: REQ-LCT-001)
Test Data	Valid user login credentials, installed app, GPS-enabled device
Test Steps	•	Open the Emergency Ambulance App.
•	Ensure successful login.
•	Navigate to the "Location Tracking" module.
•	Verify that GPS location tracking is enabled in the app. 
•	Check to make sure the user's location is updated instantly.
Expected Results	Accurate and real-time location tracking. The user's location is consistently updated on the app interface without delays.
Actual Results	The location tracking should be real-time, and it matches the location every second.
Results	Pass

Comments	If the test fails, provide detailed information on the observed issues. Evaluate the user experience and ensure that the location tracking aligns with usability standards. Verify that the system responds appropriately to different location scenarios.
 Test Case 2 - This test case details the test steps and expected results for ensuring accurate position designation in the Emergency Ambulance App. It emphasizes the user's perspective and covers steps from app opening to real-time location updates.

**2.3 Hospitals Nearby List Scenario:**
Test Case ID	HNLS_TC001
Test Case Description	Verify the functionality of displaying an accurate list of nearby hospitals in the Emergency Ambulance App from a user's perspective.
Module to be Tested	Hospitals Nearby List (Requirement ID: REQ-HNL-001)
Test Data	Valid user login credentials, installed app, GPS-enabled device
Test Steps	
•	Open the Emergency Ambulance App. 
•	Ensure successful login.
•	Navigate to the "Hospitals Nearby List" module. 
•	Check if the application is transmitting the user's position to the server.
•	Verify that the app is sending the hospital's information to the server.
•	Confirm whether a list of nearby hospitals appears.
Expected Results	An accurate and current list of nearby medical facilities. The displayed list corresponds to the user's current location and includes relevant hospital information.
Actual Results	Actual Results matched the expected results.
Results	Pass

Comments	If the test fails, provide detailed information on the observed issues. Evaluate the user experience and ensure that the hospital list display aligns with usability standards. Verify that the system responds appropriately to different scenarios.
Test Case 3 - This test case outlines the test steps, expected results, and actual results for verifying the display of an accurate list of nearby hospitals in the Emergency Ambulance App. The test focuses on the user's perspective and covers steps from app opening to hospital list confirmation.


**2.4 Communication with Emergency Services Scenarios:**
Test Case ID	CWS_TC001
Test Case Description	Verify the functionality of skilful interaction with emergency services in the Emergency Ambulance App from a user's perspective.
Module to be Tested	Communication with Emergency Services (Requirement ID: REQ-CWS-001)
Test Data	Valid user login credentials, installed app, selected hospital
Test Steps	
•	Open the Emergency Ambulance App. 
•	Ensure successful login.
•	Navigate to the "Communication with Emergency Services" module.
•	Contact emergency services as soon as possible.
•	Monitor the user's real-time communication with emergency services.
Expected Results	Successful real-time communication was accomplished. The user experiences clear and effective communication with emergency services without interruptions.
Actual Results	Actual Results matched the expected results.
Results	Pass
Comments	If the test fails, provide detailed information on the observed issues. Evaluate the user experience and ensure that the communication process aligns with usability standards. Verify that the system responds appropriately to different communication scenarios.
Table 4 - This test case provides test steps, expected results, and actual results for verifying skilful interaction with emergency services in the Emergency Ambulance App from a user's perspective. The test covers steps from app opening to monitoring real-time communication.

**3. Note:**
The Emergency Ambulance App test cases employ black box and grey box testing for scenarios like emergency requests, location tracking, hospital information, and communication. Each scenario details specific steps, expected and actual results. The tests assume network stability, device compatibility, and user awareness.

**4. Conclusion:**
Thorough testing ensures the emergency ambulance app functions reliably and effectively in various conditions, meeting its goals. Comprehensive test plans and acceptance standards guarantee a close examination of every aspect. This ongoing testing not only identifies and fixes issues but also builds trust in the app's dependability, making it a strong emergency tool. Consistent updates, based on testing results, enhance flexibility and responsiveness to new requirements or technology advances. This continuous cycle of testing and updates improves the app's performance, aligning with changing user expectations and enhancing the overall user experience.

