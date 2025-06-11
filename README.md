# FHIR® Connectathon – June 2025, Pasay City, Philippines

![Connectathon_Graphic](https://github.com/user-attachments/assets/1d6afce8-7200-45c0-a7ac-02913a0e1ba0)

The FHIR® Connectathon will be jointly co-hosted by The Standards and Interoperability Laboratory, under the University of the Philippines Manila National Institutes of Health’s National Telehealth Center (UPM SILab) and the [Commonwealth Scientific and Industrial Research Organisation (CSIRO), Australia](https://www.csiro.au/) in collaboration with The Philippines Department of Health and Philippine Health Insurance Corporation (PhilHealth). The Connectathon is part of the [Strengthening Standards Capability Project (SSCP)](https://sscp.health), for improved adoption of Digital Health Data Standards and Interoperability for the Southeast Asia and Pacific region co-funded by CSIRO and Australian Government Department of Foreign Affairs and Trade (DFAT).

The two-day Connectathon aims to foster interoperability across health systems by providing opportunities for healthcare system developers, business owners, and vendors to participate in critical use cases defined as tracks that focus on clinical and business use cases. The connectathon will also provide testing opportunities for FHIR® Implementation Guides (IGs) such as, NHDR FHIR® IG and Philippine Core FHIR® IG using public FHIR® Servers and Terminology. 

## Important Information

- [16-17 June 2025, FHIR® Connectathon Detailed Program](https://docs.google.com/document/d/1bhlvm3iZteKqJ0CvxhbOCvpamIPmssQcDVH_7WNZXGs/)
- [FHIR® Connectathon Logistic Note](https://docs.google.com/document/d/1gNo9n3zDkkLkM0lH3047BaK2q3t-Y2gyvlYvQ1_5fnw)
- [FHIR IG Technical Feedback Sheet](https://docs.google.com/spreadsheets/d/1FEyX8O-TSRJp9xOiwvb3-Jc_6K2GLbwwJtkGPNqSVI4/edit?usp=sharing). - Please add technical feedback and comments into the google sheet. It will be reviewed actively during the conenctathon. 

## Connectathon Objectives 

* Introduction of the HL7 FAST Healthcare Interoperability Resources (FHIR®) 
* Data exchange and testing of the draft NHDR FHIR® IG and PH Core FHIR® IG 
* Gather input and feedback on the development of specifications and infrastructure for the future FHIR® development including priority functionality that implementers and users require
* Develop a community of interest to enable participation in the future development of the service
  

## Tracks and Sample Data

- [Connectathon Track 1: Point-of-Service (POS) Data Submission](##connectathon-track-1-point-of-service-data-submission)
- [Connectathon Track 2: FHIR® Search and Retrieval](#connectathon-track-2-search-and-retrieval)
- [Postman Collections and Data](#sample-postman-collections-and-data)

---

### Connectathon Track 1: Point of Service Data Submission

This track will demonstrate how a Point of Service (POS) application can submit health data to a central health data repository. For this track simulation of a health data repository is implemented using the HAPI FHIR® Server. The track uses the draft NHDR FHIR® Implementation Guide (IG) defining the required profiles and value sets for core clinical data exchange such as Patient, Encounter, Medication, Observation; <!-- please review and add resources which are ready to use --> 

👉 [Click for track details](./track-1/) 

### Track goals

- Use the $validate operation for IG conformance.
- Successfully submit FHIR® resources to a central server.
- Successfully submit FHIR® bundle to a central server.
- Provide feedback to refine the IG and profiles.

### Track Leads

| Name  | Organisation    | 
|-----------------|-----------------|
| Cherrie Esteban      | Department of Health, Philippines |
| Teo Gallano      | Philippine Health Insurance Corporation |
| John Carter      | CSIRO (SSCP) |



### Connectathon Track 2: Search and Retrieval

This track builds on Track 1 by testing RESTful search and retrieval of clinical data submitted by POS applications. Using the same FHIR® server and resource profiles, participants will query the server to retrieve data for specific patients and observations. This supports key workflows like clinical review, analytics, and verification of submitted data.

👉 [Click for track details](./track-2/) 

### Track Goals

- Perform FHIR® search queries using standard parameters.
- Retrieve resources such as Patient and Observation using patient ID and filters.
- Verify content accuracy and completeness.
- Reinforce understanding of FHIR® REST API conventions.

### Track Leads

| Name  | Organisation    | 
|-----------------|-----------------|
| Cherrie Esteban      | Department of Health, Philippines |
| Teo Gallano      | Philippine Health Insurance Corporation |
| John Carter      | CSIRO (SSCP) |

---

### Sample Postman Collections and Data

To help participants get started quickly, we’ve prepared Postman collections and example data for each scenario. These include:

- Create & validate resources
- Submit transaction bundles
- Perform FHIR® search queries

📥 [Download Postman Collection](./sample-data/FHIR®_resources_collection.json)

---

Note: FHIR® is a registered trademarks of Health Level Seven International.  

For questions and queries regarding connectathon contact silab.upm@up.edu.ph
