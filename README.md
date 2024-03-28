> [!IMPORTANT]
> This is an internship project conducted in partnership with Witteveen + Bos and for the academic institution Saxion University of Applied Sciences. It represents a collaborative effort between industry and academia to develop innovative solutions.
>
> All rights to the project and its associated materials are reserved by Witteveen + Bos, Saxion University, and the author (your name). Any unauthorized use or reproduction of the project content without explicit permission is prohibited.

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
