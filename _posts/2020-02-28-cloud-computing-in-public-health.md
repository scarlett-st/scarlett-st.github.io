---
layout: post
title: "Cloud Computing in Public Health: It's About Damn Time"
subtitle: Ditching the Spreadsheets and Embracing the Cloud
author: Scarlett Thomas
---

{: .box-success}
Imagine this: you're hired to help tackle the day-to-day public health response during one of the most impactful pandemics of your lifetime.  You put on your epi hat, ready to use your training to track and diminish disease spread.  You open your laptop and are given access to all of the tools available.  Cue dumbfounded blinking.  A Google Sheets spreadsheet whose data has been manually input by other epidemiologists combing through lab reports?  You've gotta be kidding me.  

These were my thoughts 4.5 years ago when I was hired as an analytical epidemiologist to help support the COVID-19 response in healthcare facilities.  The realities of how siloed and technologically behind the state department of health was set in quickly when I was asked to create dashboards and situation reports to communicate the impacts of the spread and our current containment efforts.  Here was the process: Depending on the level of exposure, each health facility would submit daily, weekly, or biweekly test samples of all of their staff and patients to the state public health laboratory - that's over 500 facilities submitting tests to be PCR'ed and analyzed.  

Every morning, my team and I would receive a large, secured zip file of all of the PCR COVID tests that were performed the day before at the state health laboratory.  These data were separated by health facility and included a list of all who were tested and whether or not their tests were positive.  These data were then manually input into a Google Sheets spreadsheet and further filtered for specific regions, etc.  We then developed the sit report and populated the dashboard with the relevant metrics.  To say that this was time-consuming was an understatement.  We were dealing with thousands of rows of data daily and did not have the advanced technology nor the know how to be able to maintain, analyze, and disseminate this much information to stakeholders in a timely manner.  It felt like fighting a wildfire with a water pistol, TBH.

My experience was not unique. State health departments across the country struggled with similar challenges in data management, analysis, and dissemination. The limitations of outdated systems became glaringly apparent during the pandemic, highlighting the urgent need for modernization. It was around this time that the CDC was awarded funding to overhaul its technological capabilities with the [Data Modernization Initiative (DMI)](https://www.cdc.gov/data-modernization/index.html). It provided money to state and local health departments to effectively revamp and overhaul their IT infrastructure and improve their bioinformatic capability. 

These funds were also allocated to training professionals in programming, informatics, and cloud computing. I know…I know…what do these have to do with public health? I’ve shown you how NOT having them kept me bogged down among rows and rows in spreadsheets instead of being out in the field and investigating cases and implementing interventions. Now I’d like to point to two case studies where public health professionals leveraged the power of cloud computing to surveil disease spread in community and hospital-based settings. Time to ditch the abacus and get with the times!

**Digital Health Dashboards and Public Health**
Cloud computing has revolutionized public health surveillance and decision-making, particularly in tracking infectious diseases across healthcare settings.  Prior to having the power of cloud computing, state and local health departments weren't easily able to timely share important and relevant data to help disease investigators work collaboratively.  The information was siloed within servers for each system and each system used software that might have differed from one health department to the next.  Maintaining the integrity and confidentiality of the data as it was shared among systems was a nightmare.    

Regardless, public health departments stepped up to the task and responded to the need for current, up-to-date information about COVID spread.  During the epidemic, we saw an explosion of public-facing dashboards the likes of which we had never before experienced.  I'm sure most concerned citizens, by the "end" of the pandemic, were well-versed in how to navigate simple dashboards that gave them up-to-date information about COVID.  Researchers Katapally and Ibrahim \[1] were also riding this wave, but instead of having a unidirectional transmission of information, their dashboard became a collaborative effort among the scientists and the public.  

## Cloud-Based Infrastructure for Public Health Surveillance

The authors of the study utilized Amazon Web Services (AWS) to create a secure and scalable infrastructure for their digital health dashboard, allowing citizens to manually input active outbreaks or food shortages in their area. This approach demonstrates the power of cloud computing in **passive** public health surveillance:

1. **Virtual Private Clouds (VPCs)**: Two VPCs hosted on AWS provided secure environments for data storage and communication between the database, Progressive Web Application (PWA), and digital health dashboard.  Basically, if this were a version of your "No girls/boys allowed" clubhouse, only people with the special door knocking pattern (authorized users) got in.

2. **Scalability**: Amazon Elastic Compute Cloud (EC2) servers provide the ability to scale resources up or down according to demand, essential in managing sudden outbreaks or high data loads. Some weeks would see more activity from test data results and community input, requiring more resources to store and analyze the data.  The EC2 servers provided that capability, because who wants their system to crash when everyone's trying to find out if they should take more precautions with their health?

3. **Secure Data Management**: Amazon Relational Database servers provide secure storage and management of sensitive health information.  Think Fort Knox, but for your PCR results.

## Tracking Infectious Diseases Across Healthcare Settings

Wang et al. set out to develop a "cross-system surveillance and control system for infectious diseases' \[2].  Their work led to the development of the Hospital Automated Laboratory Reporting (HALR) system.  For the purpose of tracking the spread of infectious diseases, particularly Multi-Drug Resistant Organisms (MDROs), between various healthcare settings, cloud computing has the following benefits:

### Real-Time Data Collection and Analysis

Cloud-based systems like the HALR system \[2] can report targeted pathogens early, enabling early outbreak detection and trend analysis. This real-time feature is especially important when patients are transferred between various healthcare settings so that the physicians, nurses, and staff providing their care can decide whether to isolate or quarantine the patient and implement appropriate infection prevention and control protocols, thereby effectively isolating the pathogen and eliminating it from circulation.

### Interoperability and Data Sharing

Cloud platforms facilitate easy exchange of information among different healthcare facilities. As a patient is transferred from an OR to recovery, and then to a nursing home, his or her infection status can be updated in real time and shared with all of the systems involved.  No more faxes, no more playing telephone with patient data!

### Advanced Analytics and Machine Learning

Cloud computing allows one to take advantage of advanced analytics and machine learning algorithms that can help to predict the spread of MDROs based on patient movement patterns and facility characteristics.  It's like having a crystal ball that can tell you, with some confidence, how, when, and where the next outbreak will be so you can stop it before it even starts. Cool, right?


## Future Directions

The CDC's new $189 million cloud computing initiative is designed to update its current IT infrastructure, create more sophisticated analytic capabilities, and provide more effective cybersecurity. This initiative will probably improve the capacity to monitor and respond to infectious diseases across a variety of healthcare and community settings.  Furthermore, the CDC's National Healthcare Safety Network (NHSN) \[3], the nation's most used healthcare-associated infections tracking system, was just moved to Microsoft Azure Cloud.  This move allows increased coverage (over 37,000 healthcare facilities use this system), a 41% decrease in cost, increased security, and faster development of new systems, such as the hospital respiratory data reporting system.  

By leveraging cloud computing, public health officials can create a more interconnected, responsive, and effective system for tracking and controlling the spread of infectious diseases, including MDROs, as patients move through different healthcare settings. This approach not only improves patient safety but also contributes to more efficient and targeted infection control strategies.  So, let's raise a glass (of hand sanitizer, of course) to the cloud - it's about damn time public health got this upgrade.

**References**

1.  Katapally, T. R., & Ibrahim, M. A. (2023). Digital health dashboards for decision-making: A case study of community-based participatory research. *JMIR Formative Research*, *7*(12), e46810. [https://doi.org/10.2196/46810](https://doi.org/10.2196/46810)
2.   Wang, J., et al. (2019). Development of a Cloud-Based Healthcare-Associated Infection Surveillance System. *JMIR Public Health and Surveillance*, *5*(4), e10886. [https://doi.org/10.2196/10886](https://doi.org/10.2196/10886)
3.  Schnaidt, M. (2024, December 16). Modernizing CDC's information technology to meet growing public health needs. *Leidos*. \[https://www.leidos.com/insights/modernizing-cdcs-information-technology-meet-growing-public-health-needs]

