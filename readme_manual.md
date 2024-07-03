# InBeeld 3D Portal Manual

# Table of Contents
1. [Introduction](#introduction)
2. [Overview](#overview)
3. [Features for the User](#features-for-the-user)
4. [Features for End-Users](#features-for-end-users)
5. [System Requirements](#system-requirements)
6. [Getting Started](#getting-started)
    - [Installation](#installation)
    - [Machine Requirements](#machine-requirements)
    - [Setup](#setup)
7. [User Interface](#user-interface)
    - [Main Interface](#main-interface)
    - [3D Page Body](#3d-page-body)
8. [End-User Interface (Using Portal3D)](#end-user-interface-using-portal3d)
9. [Common Issues](#common-issues)
10. [Best Practice (Tips)](#best-practice-tips)

# Introduction

Now that you have a better understanding of the wonders of 3D, or perhaps you're just intrigued, let me explain how 3D works to give you insights into creating responsive and interactive 3D objects or buildings.

## Overview

The 3D InBeeld application enables users to interact with 3D objects such as buildings or bridges. Users can view these objects from different angles, zoom levels, and headings. The application utilizes Typescript, React, Python, and ArcGIS to achieve this functionality.

## Features for the User

- **Object Display**: Displaying objects in 3D.
- **Feedback Form**: Allowing users to provide feedback on 3D objects.
- **Project Information**: Providing basic project details.
- **Element Block Display**: Displaying additional elements available within Wagtail.

## Features for End-Users

- **Interactive Feedback**: Providing responses on 3D objects.
- **3D Viewing**: Viewing objects from various angles.
- **Layer Visualization**: Viewing different layers surrounding the object.
- **Phases/Slides Viewing**: Viewing different phases or slides of the object.

## System Requirements

The 3D InBeeld application has similar system requirements to its 2D counterpart. However, it is recommended to use a machine capable of efficiently handling 3D objects, beyond basic laptop capabilities. While InBeeld 3D strives for accessibility across all devices, slower machines may experience rendering challenges, impacting application responsiveness and usability.

# Getting Started

## Installation

### For Developers:

1. Follow the steps in the general README to access localhost with Portal3D.
2. No additional installation is required.

### For Users:

1. Refer to general information on setting up the CMS.
2. Once the CMS setup is complete, you'll have access to the 3D portal.
3. To add the 3D portal to a new page, create a new underlying page in the root or under an existing page.

### For End Users:

- No installation required.

## Machine Requirements

### For Developers:

- No special requirements.
- Recommended to use a machine capable of handling average 3D modeling tasks, especially when testing the 3D portal with Blender icons.
- Despite API calls handling, using a device with average or above-average CPU and RAM is recommended.

### For Users:

- No special requirements.
- Average or above-average device recommended.

### For End Users:

- No special requirements.
- Average or above-average device recommended.

# Setup

## For Developers:

1. Refer back to the standard README for InBeeld setup.
2. To edit parts of the 3D portal, access the following files:

   - **frontend/components/EsriScene/EsriScene.tsx**: Main entry point defining HTML, CSS, and functions. Organized into multiple files for better structure.
   - **frontend/types/components/esriscene.ts**: Interfaces created, defining properties required for EsriScene.
   - **frontend/containers/PortalPage3d/PortalPage3d.tsx**: Calls EsriScene and creates standard three widgets, passing necessary information.
   - **src/main/pages/portal3d.py**: Manages item creation for database and Wagtail portal3d page fields, accessible when creating a new 3D portal.

   For detailed code breakdown, refer to comments within each file.

## For Users:

1. Set up a new underlying page as desired.
2. Populate information with or without a reaction form to establish a 3D portal page.
3. Refer to detailed information below on user interface functionality.

## For End Users:

- No additional setup required.
- Simply choose the page from the options in the top right menu.

# User Interface

## Main Interface

Assumes basic understanding of Wagtail CMS and familiarity with InBeeld. For those new to Wagtail/InBeeld, refer to the other README for basic elements.

### Creating 3D Pages:

1. In Wagtail, navigate to "Pages" and add a new or underlying page by clicking the "+" icon.
2. Select Portal3D from the options provided.

### Structure Overview:

1. Similar to 2D portal with minor differences.
2. **Title**: Name visible in navigation, linking to the page.
3. **ID**: Functions like 2D portal ID, but crucial distinction:
   - **WebMap**: Used for 2D maps.
   - **WebScene**: Used for 3D scenes.

   Choosing between WebMap and WebScene determines user interaction with 2D or 3D content.

### Host Selection:

1. Mirror host requirements of 2D portal.
2. Select server (Witteveen+Bos or ArcGIS) for hosting object, aligning choice with project needs.

### Reaction Form:

1. **Enabling**: Allows users to provide feedback directly on the 3D object, enhancing user engagement.
2. **Disabling**: Allows interaction with 3D object (e.g., rotation, zoom) without feedback capability.

### Basic 3D Page Information:

1. **Title**: Clear, descriptive project name.
2. **Description**: Overview of project purpose and details.
3. **Project Label**: Flexible field indicating project timeline or other relevant label.

### Portal Description:

- Elaborate on portal, including:
  - Additional information about 3D objects/models.
  - Background details on project or data.
  - Screenshots or visual aids enhancing understanding.
  - Other context descriptions improving user experience.

### Widgets:

- Customize standard widgets based on project needs:
  - **Enabling/Disabling Widgets**: Activate widgets as per project requirements.
  - **Widget Placement**: Position widgets in top left/right corners for optimal user interaction.

## 3D Page Body

- Customize main body with:
  - **Wagtail Tools**: Format and organize content using Wagtail’s standard tools.
  - **Customization**: Add elements to create unique, functional 3D page meeting project requirements.
  - **Saving and Publishing**: Save as draft or publish live for user interaction.

By following these instructions, set up and customize the 3D portal to meet project needs, offering engaging user experiences.

# End-User Interface (Using Portal3D)

## Standard Situation

Upon opening InBeeld 3D portal, users see main page with customized body and blocks.

### Navigation and Widgets:

- Navigate through available widgets and blocks.
- Widgets provide additional information or interactive elements related to 3D object.

### Interacting with 3D Object:

- Use WebScene directly with 3D object displayed on created page.
- Change object view via rotation, zoom, or pan for different perspectives and details.

### Fullscreen and Interactive Options:

- Maximize 3D object to Fullscreen mode for enhanced experience.
- Additional options may include:
  - **Viewing Different Angles (Bookmarks)**: Access created viewpoints (bookmarks) within 3D scene, switching perspectives easily.

### Providing Feedback:

- **Enabling Reaction Form**: Users click on 3D map point to provide feedback.
- Modal appears for entering feedback/comments on specific location/object.
- Enhances user engagement via direct interaction with 3D model.

With these new features/functions, users explore, interact, and provide feedback on showcased objects in Portal3D application. 3D interaction aims to enhance user engagement and deepen understanding of presented projects or objects.

# Common Issues

## Why Isn't the Modal Form Popping Up?

Common fixes:
- Check if reaction form is selected; without form, users can view but not respond.
- Verify reaction form dates; invalid dates prevent functionality.
- Confirm page language; ensure translation for form elements.
- Ensure all required parts (privacy statement, moods, etc.) are present.

## Why Is My Map Not Loading?

- Ensure correct API string usage for WebScene.
- Verify API string accessibility; use public WebScene part for application.
- Check if WebScene is used, not WebExperience; they differ in environment and URL.

## Why Can't I See the Slides?

- Confirm slides creation via WebScene link.
- If URL loads but slides aren't visible, they may not be created; contact ArcGIS portal admin.

## Why Is the Map Empty?

- Similar to loading issue; ensure correct object loading into 3D portal.
- Contact InBeeld team if issues persist.

# Best Practice (Tips)

To test a 3D scene:
- Copy the code after the “=” from a public WebScene link.
- Paste into a new portal to test.
- Swap scene codes for similar 3D buildings if public.
- Troubleshoot for private keys, improper WebScenes, or string errors.
