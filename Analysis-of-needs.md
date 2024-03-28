# Analysis of Needs
## Introduction
For my internship at Witteveen + Bos, I'm developing an application to enable users to provide feedback on 3D building or other objects, enhancing interaction and modernizing the experience. Currently, users can only respond on a 2D map, limiting the specificity of feedback. Transitioning to a 3D environment offers the potential for more precise feedback by visualizing structures in three dimensions.

The project primarily targets two stakeholder groups: governmental bodies, Witteveen + Bos, and other engineering advisory firms, along with their diverse clientele. By receiving feedback from these groups, the aim is to improve engagement with the 3D mapping interface compared to traditional 2D maps.

The overarching objective is to gain insights into the requirements and constraints of the project through a thorough analysis of needs. Anticipated challenges include aligning the envisioned functionalities with the capabilities of the ArcGIS application.

This initiative not only seeks to enhance user experience but also holds the potential to reshape stakeholder interaction with spatial data in urban planning and development contexts.

## Background information.
### Project Background:
The Inbeeld project, as introduced earlier, aims to empower users with the capability to provide feedback on 3D buildings and objects. Currently undergoing an overhaul with a new design, the project has long wished for an 3D functionality, which are now being pursued.

### Contextual Information:
In the realm of construction and infrastructure, there's a notable shift in the role of government bodies, which are now mandated to facilitate community participation. As such, the significance and potential of Inbeeld are heightened, with the opportunity to pioneer in this space. Although Inbeeld is currently utilized primarily for internal projects, its potential to serve external parties remains largely untapped for now.

### Stakeholder Context:
Key stakeholders in the project include internal stakeholders, such as Witteveen + Bos, the project owner, end users, and external stakeholders, including government bodies and other parties utilizing Inbeeld for their own clientele.

### Project Scope and Timeline:
The project adopts the Scrum methodology, with sprints occurring every two weeks and milestones tracked via GitHub. Scheduled to conclude by the end of my internship period around mid-July, the aim is to achieve project completion by the end of the 18th week.

### Resources:
For the project, resources include a company laptop and software tools such as Visual Studio Code, along with expertise in JavaScript, React.js, and ArcGIS. Given the internal (and internship) nature of the project, no specific budget allocation is required.

### Relevant Data:
Initially, the project will utilize 3D building models from Witteveen + Bos. After it completion, efforts will be made to engage internal parties working with ArcGIS or AutoCAD to test the application with diverse building models.


## Stakeholder Analysis
### Internal stakeholders (Witteveen + Bos):
Witteveen + Bos is embracing a Silicon Valley mentality with this project, aiming to invest in and create a product that will attract users in the future. It's crucial for them to pioneer a new way of participation in this field and potentially become a leading party. 

### Project Owner:
As the main link between our team and potential users, the project owner plays a pivotal role in communicating requirements, desires, and issues to us. It's a must to deliver a fully functional application that the project owner can promote to other parties. Balancing ideals with practical realities is essential for maintaining alignment throughout the project.

### End users:
Our end users, who will provide feedback on buildings/objects, will vary widely in technological proficiency. therefore, simplicity and intuitiveness are paramount to ensure accessibility for all users, including those with disabilities. 

### External stakeholders (Government Bodies and other parties):
For external stakeholders, such as government bodies, demonstrating the advantages of the project beyond mere compliance is crucial. Showing how the application can enhance their plans with valuable feedback and insights can garner long-term support and collaboration.

## Needs Assessment
### functional requirements (User)
| **Title**                              | **User Story**                                                                  | **Requirement**                                                                                           | **Priority** |
| -------------------------------------- | ------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | ------------ |
| Responding on the Map                  | As a user, I should be able to respond anywhere on the map                      | The application must allow users to place responses on the map and store them at the specified locations. | Must         |
| Responding on the Map without location | As a user, I should be able to respond on the map                               | The application must allow users to place and store them                                                  | Must         |
| Viewing Buildings in 3D                | As a user, I should be able to view buildings in 3D                             | The system must support 3D web scenes to render buildings in 3D.                                          | Must         |
| Viewing Responses on Buildings         | As a user, I should be able to see my response placed on the building           | The application must receive and display user responses accurately on the corresponding buildings.        | Must         |
| Viewing Building Details               | As a user, I should be able to view details about buildings and their objects   | The application should provide information about selected buildings and objects upon user interaction.    | Should have  |
| Viewing Construction Activities        | As a user, I should be able to view information about construction activities   | The application must allow users to view construction details, including start and end dates.             | Must         |
| Accessing Function Overview            | As a user, I should be able to access an overview of available functions        | The application should provide clear guidance to users and product owners about available functions.      | Could have   |
| Viewing Other Responses                | As a user, I should be able to see other responses around the building          | The application should display all nearby responses to enhance user awareness and interaction.            | Should have  |
| Receiving Confirmation for Feedback    | As a user, I should receive confirmation after successfully submitting feedback | The application must provide immediate feedback to users upon successful or failed feedback submission.   | Must         |
| Viewing Multiple Levels                | As a user, I should be able to view multiple levels within buildings            | The application should support navigation through multiple levels within ArcGIS buildings.                | Should have  |
|  Viewing Multiple Scenes               | As a user, I should be able to view multiple scenes (before/after)              | The application should offer multiple scenes for users to visualize different time periods or scenarios.  | Should have  |

### functional requirements (Product owner)
| **Title**                            | **User Story**                                                                   | **Requirement**                                                                                                    | **Priority** |
| ------------------------------------ | -------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ------------ |
| **Responding to Reactions**          | As a product owner, I should be able to respond to a reaction                    | The application should allow a response from a user and store the information                                      | Must         |
| **Setting Application Password**     | As a product owner, I should be able to set a password for the application       | The application should have a restricted version                                                                   | Should have  |
| **Making Design Changes**            | As a product owner, I should be able to make minor design changes                | The application could have the ability for a product owner to make basic design changes such as color              | Could have   |
| **Changing Buildings**               | As a product owner, I should be able to change the building                      | The application should work with all correctly filled buildings within ArcGIS                                      | Must         |
| **Managing Widget Visibility**       | As a product owner, I should be able to choose which widgets are visible         | The application should provide a list of widgets and the ability for the product owner to control their visibility | Should have  |
| **Customizing Surrounding Elements** | As a product owner, I should be able to change basic elements of the surrounding | The application should provide the ability for end-users to toggle certain elements in the surrounding area on/off | Should have  |
| **Adding Images**                    | As a product owner, I should be able to add images to the application            | The application should be able to receive and store images                                                         | Could have   |
| **Adding Layers**                    | As a product owner, I should be able to add layers to the application            | The application should support the addition of layers                                                              | Could have   |
| **Placing Icons on Buildings**       | As a product owner, I should be able to add icons to buildings                   | The application should accept material icons from Google and display them on the map                               | Would have   |
| **Adding Points of Interest (POI)**  | As a product owner, I should be able to place POI on buildings                   | The application should allow product owners to add points of interest (POI) to buildings                           | Must         |

### Non-functional requirements
| **Title**                          | **User Story**                                                                                             | **Requirement**                                                                     | **Priority** |
| ---------------------------------- | ---------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ------------ |
| **Response Time**                  | As a user, I should have response time within 20 seconds for all interactions under normal load conditions | The application should run within 20 seconds                                        | Could have   |
| **Technical Knowledge**            | As a user, I should need the minimum required technical knowledge                                          | The application should be understandable for all levels of technical knowledge      | Should have  |
| **Accessibility Standards**        | The application should adhere to accessibility standards                                                   | The application should work with different types of accessibility standards         | Should have  |
| **Visibility of Responses**        | Users should understand that their public response will be visible to others                               | The application should clearly inform users about the visibility of their responses | Must         |
| **Compatibility Testing**          | The application should undergo compatibility testing to ensure consistent performance                      | The application should be thoroughly tested to ensure stability                     | Should have  |
| **Ease of Use for Product Owners** | As a product owner, I shouldn’t need a lot of technical knowledge for basic changes                        | The application should provide easy access and usability for product owners         | Would have   |

By meeting these requirements, the application aims to facilitate user interaction with 3D buildings and objects, enhancing the overall user experience and potentially driving increased sales for inBeeld. Additionally, the project seeks to expand the availability of 3D building models, thereby enriching the platform's database and attracting a broader user base. The primary focus remains on empowering end users to provide feedback directly on the map interface, ensuring their engagement and satisfaction with the application.

## Gap Analysis
### Current State
InBeeld recently underwent a major redesign and functional update, transitioning from an older interface to a more modernized design. Presently, users interact with a 2D map interface, where they can place responses, view a legend, zoom in/out, and access a list of all responses.

### Desired State
The desired state involves upgrading the InBeeld platform to incorporate a 3D building environment, providing users with the ability to place 3D objects as markers, navigate through the building using multiple scenes, and visualize construction progress over time.

### Gap
The primary challenge lies in integrating 3D functionality using the ArcGIS API. ArcGIS presents complexities in understanding and implementing 3D models within the platform. The gap exists in navigating these complexities to effectively incorporate 3D capabilities into the application's interface.

### Mitigation Strategies
To address this gap, the development team will focus on enhancing their understanding of the ArcGIS API's 3D capabilities through targeted training, research, and collaboration with experts. Additionally, they will engage with the ArcGIS community and leverage available resources, such as documentation and support forums, to troubleshoot issues and optimize implementation. Continuous testing and iteration will be conducted to refine the integration of 3D functionality and ensure a seamless user experience.

## Constrains and limitations

### Technical Complexity with ArcGIS API:
Working with the ArcGIS API presents a significant learning curve due to its technical complexity. This may necessitate thorough documentation to facilitate project handover and ensure continuity in development efforts.

### Dependency on Evolving Esri Technologies:
The project relies on Esri technologies, such as Sceneview, which are subject to change or discontinuation by the provider. Continuous monitoring of Esri's updates and potential shifts in technology is essential to adapt project strategies accordingly.

### Solo Development Efforts:
With the project being developed solo, there may be challenges in managing workload and addressing unforeseen complexities. Flexibility is key to adjusting project requirements and resource allocation as needed throughout the development cycle.

### Data Management and GDPR Compliance:
Data handling, particularly concerning user feedback, requires careful consideration to ensure compliance with GDPR regulations. Balancing the desire for comprehensive feedback analysis with legal obligations regarding data privacy and consent is critical.

### Time Constraints of Internship Duration:
The project timeline is constrained by the duration of the internship, spanning 20 weeks. While aiming for ambitious project goals, it's essential to maintain a realistic perspective and prioritize tasks effectively within the allocated timeframe.

## Risk Analysis
### Dependency on ArcGIS for Building Viewer:
The primary reliance on ArcGIS for building visualization poses a significant risk. Any downtime or service interruptions from ArcGIS could lead to the entire application being inaccessible. This dependency underscores the importance of closely monitoring ArcGIS's performance and having contingency plans in place to mitigate disruptions.

### Risk of Data Loss:
With users providing numerous responses, the risk of data loss during updates or deployments is a critical concern. Implementing robust backup procedures prior to deploying new versions can safeguard against potential data loss and ensure continuity of user interactions.

### Optimization for Resource Efficiency:
While budget constraints are not a direct concern, resource efficiency remains paramount. Striving for lightweight application design minimizes server costs and enhances the end-user experience. Prioritizing efficiency in resource utilization ensures scalability and sustainability in the long run.

### Compliance with GDPR Regulations:
Non-compliance with GDPR regulations poses a substantial risk, potentially leading to severe financial penalties. Clear protocols must be established to ensure transparent data handling practices, including explicit consent from users regarding data storage and usage. Adhering strictly to GDPR guidelines mitigates legal and reputational risks associated with data privacy breaches.

### Competitive Landscape and Innovation:
Staying ahead of the market in building visualization and user interaction tools is critical. As a niche concept, the application's success hinges on its ability to offer innovative features and a superior user experience. Proactive innovation ensures that the application remains competitive and maintains its position as a leading platform for 3D response participation.

## Recommendations
### Utilize Commonly Used Objects for Reliability:
Incorporate widely-used 3D objects and components to enhance the reliability and compatibility of the application. Prioritizing common objects ensures easier collaboration with other developers and facilitates future maintenance.

### Implement Robust Backup Procedures:
Establish comprehensive backup procedures to safeguard data integrity during updates or migrations. Consider scripting solutions to automate data conversion processes and minimize the risk of data loss during transitions between old and new versions.

### Optimize ArcGIS Performance:
Explore optimization techniques to improve the performance of ArcGIS applications. Strive for a balance between data quality and loading times by selectively importing necessary details. Prioritize optimizing performance to enhance user experience and minimize loading delays.

### Review Data Storage Requirements for Feedback:
Evaluate the necessity of storing all feedback information and consider options for anonymized responses. Determine whether certain data points are essential for analysis or if anonymization can be implemented to protect user privacy while still providing valuable insights.

### Continued Learning and Skill Development:
Commit to ongoing learning and skill development in ArcGIS and JavaScript to refine proficiency and build a better end product. Invest time in exploring advanced features, attending training sessions, and engaging in hands-on practice to enhance expertise and capabilities.

## Conclusion
Working on the development of an interactive 3D building application with dynamic objects is both exhilarating and demanding. With the analyzing needs, identifying requirements, and acknowledging constraints and limitations, the project has established a robust foundation poised for design initiation.

With a keen focus on meeting stakeholders' needs, 3D InBeeld is dedicated to delivering a solution that is both valuable and user-centric. By prioritizing both functional and non-functional requirements, the project aims to craft a seamless and intuitive user experience while ensuring compliance with regulatory standards, notably GDPR.

As we navigate through the project, it's imperative to remain vigilant in identifying risks and challenges, including reliance on external APIs and safeguarding data privacy. By addressing these concerns proactively, we can fortify our project against potential setbacks and ensure smooth progress.

Undoubtedly, the path to realizing a novel 3D participation application presents its share of obstacles. However, with unwavering dedication, innovative thinking, and steadfast commitment, I am confident in the project's potential to redefine the future landscape of InBeeld.

> [!IMPORTANT]
> This document is part of the main file. Please ensure that you are referring to the complete document for comprehensive information and context.