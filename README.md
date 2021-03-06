# Crowdsourcerer: Data Collector
#### A Custom Integration for the Home Assistant Community Store (HACS)

This integration was developed in the context of the final project for Licenciatura em Engenharia Informática (Bachelors in Informatics Engineering) at University of Aveiro. 
It collects the data generated by a Home Assistant installation, filters it to remove personal data and sends it to a data lake, where we collect data from a number of smart houses. This data will then be available for further use, such as academic research.

For the best experience, pair this with the respective Dashboard Card available at [CrowdSourcerer Lovelace Card](https://github.com/CrowdSorcerer/crowdsourcerer-card).

## How to Install via HACS

First, you need to have HACS installed in your Home Assistant environment. More information [available here](https://hacs.xyz/docs/setup/prerequisites).

#### 1 - Add repository to HACS
  1. Open the HACS screen, via the sidebar.
  
  ![image](https://user-images.githubusercontent.com/56603542/172457746-cadcd118-6d27-4a77-af87-ccd335320b82.png)
  
  2. Click on Integrations
  
  ![image](https://user-images.githubusercontent.com/56603542/172458033-27bd09ef-b997-4482-993c-df9ee905f613.png)
  
  3. Click on 'Custom Repositories' (On Top Left⋮)
  
  ![image](https://user-images.githubusercontent.com/56603542/172460056-d57a7a24-b1b5-4146-bfc8-7f1ba0313f0a.png)
  
  4. Insert the link for this repository in 'Repository' text box, and pick the 'Integration' category. Press Add.
  
  5. Press the big blue button "Explore & download repositories", and then search for data_collector or Crowdsourcerer. Select Crowdsourcerer, and then press "Download this repository with hacs"
  
  ![image](https://user-images.githubusercontent.com/56603542/172461082-d75a8daa-5618-478f-91e6-21bb3e5911a5.png)

  6. Restart Home Assistant (this can be done via Settings -> System->Restart (top right))
  
 
#### 2 - Add Integration to Home Assistant
  This proceeds as any other integration.
  1. Go to Settings-> "Devices & Services"
  2. Click "Add Integration"
  3. Search for "Crowdsourcerer" or "Data Collector"
  4. Select "Crowdsourcerer"
  
#### 3 - Configure initial install
  Here, you can select which sensor groups' data to send. You can also select either "All" to send all data or "None", and don't send any data.
  
Please keep in mind that the "None" and "All" options will override everything, with "None" taking precedence. (If both "All" and "None" options are selected, no data will be collected).
  
##### You're done! 
  You can always change the configuration by returning to the "Devices & Services" screen and pressing "Configure" on the Crowdsourcerer integration.
