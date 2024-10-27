# American Energy Market Regulator | SQL & Jupyter Notebook

Full in-depth project can be found [here](https://github.com/Kahvedzic/American-Energy-Market-Regulator/blob/main/AEMR.ipynb)

<img width="866" alt="Screenshot 2024-10-24 at 5 13 58 PM" src="https://github.com/user-attachments/assets/5498e84c-a13b-4677-936e-b964c2fb8aa2">

# Project Background

The American Energy Market Regulator (AEMR) oversees the reliability of the USA's domestic energy network, minimizing disruptions known as outages. Of the four types of outages, the AEMR penalizes only forced outages, as they can threaten network reliability if energy supply cannot meet demand. Recently, the AEMR has noted an increase in outage submissions for 2016 and 2017. The management team has two primary concerns, energy stability and market outages, and energy losses and market reliability. As an analyst, you are tasked with addressing these concerns by using SQL and Tableau to extract and analyze relevant data, answering queries, and providing additional insights for the management team.

What's the Business Problem? 💰

The American Energy Market Regulator (AEMR) is responsible for looking after the United States of America’s domestic energy network. The regulator’s responsibility is to ensure that America’s energy network remains reliable with minimal disruptions, which are known as outages.

There are four key types of outages:

● Consequential

● Forced

● Opportunistic

● Planned

Insights and recommendations are provided on the following key areas:

Recently, the AEMR management team has been increasingly aware of a large number of energy providers that submitted outages over the 2016 and 2017 calendar years. The management team has expressed a desire to have the following two areas of concern addressed:

A) Energy Stability and Market Outages

B) Energy Losses and Market Reliability

As an analyst within the data and reporting team, we've been asked to address these two immediate areas of concern

Below consists of major key highlights of entire project

# Data Structure & Initial Checks

<img width="827" alt="Screenshot 2024-10-27 at 2 26 11 PM" src="https://github.com/user-attachments/assets/50f1908e-8842-4d49-9beb-19b3c65743ef">

<img width="466" alt="Screenshot 2024-10-27 at 2 26 31 PM" src="https://github.com/user-attachments/assets/9ecc979c-b8fe-40f7-b0d6-e45d21199626">

Prior to beginning of analysis, familiarization with the datasets was used for quality control

# Executive Summary 

Overview of findings:

Having identified the top 3 participants by Total Energy Loss being GW, MELK and Auricon; we now need to calculate the Total_Energy_Lost each of these three Participant Codes and the Facility_Code. Additionally, identify the Description_Of_Outage associated with the highest Total_Energy_Lost for each of the Participant_Codes and Facility_Code for each of the three participants.

<img width="883" alt="Screenshot 2024-10-27 at 2 35 01 PM" src="https://github.com/user-attachments/assets/15f5559a-d961-4a98-ae6f-5f12952d4a09">

We've indentified the top 3 participants attributing to total energy loss

* Auricon had a total of 6033.97 energy loss
* GW had a total of 28687.54 energy loss
* MELK had a total of 1100.00 energy loss 














