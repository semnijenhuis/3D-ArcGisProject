> [!IMPORTANT]
> This document is part of the main file. Please ensure that you are referring to the complete document for comprehensive information and context.

# Introduction
For my internship at Witteveen + Bos, I'm developing an application to enable users to provide feedback on 3D building or other objects, enhancing interaction and modernizing the experience. 

Currently, users are confined to offering feedback solely within a 2D map interface, which inherently limits the specificity and depth of their input. By transitioning to a 3D environment, we envision unlocking the potential for more nuanced and precise feedback. Visualizing structures in three dimensions not only enriches the user experience but also provides a more comprehensive understanding of the architectural landscape.
In the preceding document, the Analysis of Needs, we explored the overarching requirements, risks, and aspirations for the project on a broad scale. Now, in the Requirements Analysis phase, our focus shifts towards a more in depth examination of the details necessary for project realization.

# Scope definition
The primary objective of this project is to enable users to provide feedback on 3D buildings or objects interactively. The application will leverage React.js and JavaScript for frontend development, while utilizing the ArcGIS Web API for mapping functionalities.

Key deliverables include comprehensive developer manuals for Witteveen + Bos developers and product owners. These manuals will provide detailed instructions on implementing and customizing the application according to specific project requirements.

End users will have the capability to provide feedback anywhere on the 3D model, view existing responses, and interact with the building in a three-dimensional environment.

Project owners will have limited customization options, primarily focusing on ease of implementation and usability. While they won't be able to modify the building itself, they will have access to essential functionalities for managing user responses and interactions.

The project's dependency on the ArcGIS API necessitates alignment with their functionalities, with consideration for potential changes or removals in the API's features.

Stakeholders anticipate a novel approach to user participation, presenting both exciting opportunities and challenges for the project's success.

Potential risks include limitations imposed by the ArcGIS platform, which may require adjustments to meet project requirements effectively.

The project's success will be determined by the ability of users to seamlessly place responses in 3D space on or within a building, ensuring accessibility and usability for a wide range of users.

# Functional requirements
| **ID** | **User Story**                                                                  | **Requirement**                                                                                         | **Priority** | **Testing**                                            |
| ------ | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------- | ------------ | ------------------------------------------------------ |
| FR1    | As a user, I should be able to respond anywhere on the map                      | The application must enable users to place responses on the map and store them at specified locations   | Must         | Cypress testing to verify response placement           |
| FR2    | As a user, I should be able to see my response placed on the building           | The application must accurately display user responses on corresponding buildings                       | Must         | Cypress testing to verify response visibility          |
| FR3    | As a user, I should be able to view buildings in 3D                             | The system must support 3D web scenes to render buildings in three dimensions                           | Must         | Cypress testing to verify 3D building rendering        |
| FR4    | As a user, I should be able to view information about construction activities   | The application must allow users to view construction details, including start and end dates            | Must         | Cypress testing to verify construction details display |
| FR5    | As a user, I should receive confirmation after successfully submitting feedback | The application must provide immediate feedback to users upon successful or failed feedback submission  | Must         | Cypress testing to verify feedback submission feedback |
| FR6    | As a user, I should be able to see other responses around the building          | The application should display all nearby responses to enhance user awareness and interaction           | Should have  | Cypress testing to verify display of nearby responses  |
| FR7    | As a user, I should be able to view multiple levels within buildings            | The application should support navigation through multiple levels within ArcGIS buildings               | Should have  | Cypress testing to verify multi-level navigation       |
| FR8    | As a user, I should be able to view multiple scenes (before/after)              | The application should offer multiple scenes for users to visualize different time periods or scenarios | Should have  | Cypress testing to verify scene functionality          |
| FR9    | As a user, I should be able to view details about buildings and their objects   | The application should provide information about selected buildings and objects upon user interaction   | Should have  | Cypress testing to verify display of building details  |
| FR10   | As a user, I should be able to access an overview of available functions        | The application should provide clear guidance to users and product owners about available functions     | Could have   | Cypress testing to verify visibility of all functions  |

# Non-Functional requirements
| **ID** | **User Story**                                                                                             | **Requirement**                                                                     | **Priority** | **Testing**                                                                  |
| ------ | ---------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | ------------ | ---------------------------------------------------------------------------- |
| NFR1   | Users should understand that their public response will be visible for others                              | The application should clearly inform users about the visibility of their responses | Must         | Conduct field testing to assess user comprehension of privacy settings       |
| NFR2   | As a user, I should have response time within 20 seconds for all interactions under normal load conditions | The application should respond within 20 seconds under normal load conditions       | Could have   | Use Cypress testing along with Chrome performance tools for benchmarking     |
| NFR3   | As a user, I should need the minimum required technical knowledge                                          | The application should be intuitive and user-friendly for users with any expertise  | Should have  | Conduct field testing with individuals of varying technical backgrounds      |
| NFR4   | The application should adhere to accessibility standards                                                   | The application should be accessible to users with different abilities              | Should have  | Conduct field testing with individuals with disabilities to assess usability |
| NFR5   | The application should have compatibility testing to ensure consistent performance                         | The application should undergo compatibility testing for stability                  | Should have  | Use Cypress testing to assess compatibility across different platforms       |
| NFR6   | As a product owner, I shouldn’t need a lot of technical knowledge for basic changes                        | The application should have an intuitive interface for product owners               | Would have   | Conduct field testing with product owners to assess usability                |

# External interfaces
## ArcGIS WebScene Integration
Inbeeld 3D will rely mostly on ArcGis WebScene for the rendering of the buildings/ objects in 3D. The ArcGis JavaScript API interacts with WebScene and SceneView components so that it can visualize a building in 3D.

## Data Exchange with ArcGIS
For all responses the application is connected to our database that is already build for the 2D map, it will adjust some minor details to make it compatible with the extra data needed. But it will all be RESTful APIs with Django.

## SceneView Configuration
SceneView is the backbone of displaying immersive 3D scenes (buildings/ objects). With customizing the SceneView your able to change specific settings such as the camera position, lighting effects and layers so we can enhance the user experience.

## Performance Optimization
To optimize performance when interacting with ArcGIS services, we are going to use different strategies such as data caching, lazy loading of resources, asynchronous data fetching and changing which objects needs to be render. This way we try to improve the responsiveness of our application.

## Error Handling and Recovery
Our application will include error handling mechanisms to manage exceptions and recover from failures when a user tries different things than expected. 

## Privacy Considerations
We are going to store only the data that we are allowed to store with GDPR and other ruling

## Integration Testing
We conduct testing with cypress to verify the seamless interaction between our application and ArcGIS services. These testing scenarios include validating data exchange and simulating various error conditions to ensure robustness and reliability.

# Conclusion
