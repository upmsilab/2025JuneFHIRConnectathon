# FHIR Connectathon – June 2025, Metro Manila, Philippines

The FHIR Connectathon will be jointly co-hosted by The Standards and Interoperability Laboratory, under the University of the Philippines Manila National Institutes of Health’s National Telehealth Center (UPM SILab) and the [Commonwealth Scientific and Industrial Research Organisation (CSIRO), Australia](https://www.csiro.au/) in collaboration with The Philippines Department of Health and Philippine Health Insurance Corporation (PhilHealth). The Connectathon is part of the [Strengthening Standards Capability Project (SSCP)](https://sscp.health), for improved adoption of Digital Health Data Standards and Interoperability for the Southeast Asia and Pacific region co-funded by CSIRO and Australian Government Department of Foreign Affairs and Trade (DFAT).

The two-day Connectathon aims to foster interoperability across health systems by providing opportunities for healthcare system developers, business owners, and vendors to participate in critical use cases defined as tracks that focus on clinical and business use cases. The connectathon will also provide testing opportunities for FHIR Implementation Guides (IGs) such as, NHDR FHIR IG and Philippine Core FHIR IG using public FHIR Servers and Terminology. 


## Connectathon Objectives 

* Introduction of the HL7 FAST Healthcare Interoperability Resources (FHIR) 
* Data exchange and testing of the draft NHDR FHIR IG and PH Core FHIR IG 
* Gather input and feedback on the development of specifications and infrastructure for the future FHIR development including priority functionality that implementers and users require
* Develop a community of interest to enable participation in the future development of the service
  

## Tracks and Sample Data

- [Connectathon Track 1: Point-of-Service (POS) Data Submission](#connectathon-track-1-pos-data-submission)
- [Connectathon Track 2: FHIR Search and Retrieval](#connectathon-track-2-fhir-search-and-retrieval)
- [Postman Collections and Data](#sample-postman-collections-and-data)

---

### Connectathon Track 1: Point of Service Data Submission

This track will demonstrate how a Point of Service (POS) application can submit health data to a central health data repository. For this track simulation of a health data repository is implemented using the HAPI FHIR Server. The track uses the draft NHDR FHIR Implementation Guide (IG) defining the required profiles and value sets for core clinical data exchange such as Patient, Encounter, Medication, Observation; <!-- please review and add resources which are ready to use --> 

### Track goals

- Successfully submit FHIR resources to a central server.
- Successfully submit FHIR bundle to a central server.
- Use the $validate operation for IG conformance.
- Provide feedback to refine the IG and profiles.

👉 [Click for track details](./track-1/) 

### Connectathon Track 2: Search and Retrieval

This track builds on Track 1 by testing RESTful search and retrieval of clinical data submitted by POS applications. Using the same FHIR server and resource profiles, participants will query the server to retrieve data for specific patients and observations. This supports key workflows like clinical review, analytics, and verification of submitted data.

### Track Goals

- Perform FHIR search queries using standard parameters.
- Retrieve resources such as Patient and Observation using patient ID and filters.
- Verify content accuracy and completeness.
- Reinforce understanding of FHIR REST API conventions.

👉 [Click for track details](./track-2/) 

---

### Sample Postman Collections and Data

To help participants get started quickly, we’ve prepared Postman collections and example data for each scenario. These include:

- Create & validate resources
- Submit transaction bundles
- Perform FHIR search queries

📥 [Download Postman Collection] <!-- (./POS_Postman_Collection_v2_with_Search.json) --> 
📥 [Download TestScript JSON] <!-- (./POS_FHIR_TestScript.json) --> 

---

_For questions, contact the Track Leads, or join Zulip Chat and Community of Practice WhatsApp group:_ <!-- add details -->
