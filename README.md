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

**Below consists of major key highlights of entire project**

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

# Insights Deep Dive

Here, we'll show the Total of all Outage Types (Forced, Consequential, Scheduled, Opportunistic) where the Status = Approved, that occurred for both 2016 and 2017, grouped by Year and Month. per month (i.e. 1 – 12). Order by Year, Month, Total_Number_Outages in Descending Order.

Also building on the query we wrote in i), group the results by Outage Type, Year and Month. This is so we can identify whether there is any outage type specifically increasing on a monthly basis when comparing 2016 to 2017.

<img width="271" alt="Screenshot 2024-10-27 at 2 50 20 PM" src="https://github.com/user-attachments/assets/66f17b52-c155-4353-a0b1-6f74451b5138">

Here, well calculates 1) The Total_Number_Outage_Events and 2) The Average Duration in DAYS for each Participant Code and Outage Type over the 2016 and 2017 Period where the Status = Approved. Order by Total_Number_Outage_Events in Descending Order, Reason and Year.

<img width="740" alt="Screenshot 2024-10-27 at 2 51 18 PM" src="https://github.com/user-attachments/assets/b6ade246-4cca-4cdc-9357-4a1756dfa6b2">

**We classify a participant based off the following criteria:**

High Risk - On average, the participant is unavailable for > 24 Hours (1 Day) OR the Total Number of Outage Events > 20
Medium Risk - On average, the participant is unavailable between 12 and 24 Hours OR the Total Number of Outage Events is Between 10 and 20
Low Risk - On average, the participant is unavailable for less than 12 Hours OR the Total Number of Outage Events < 10
If Outage Type is not forced, then N/A

Here, we'll classifies each participant code as either High Risk, Medium Risk or Low Risk in a column called Risk_Classification using the new classification criteria. Order the results using Average Duration Time In Days in descending order.

ONLY LIMIT TO 5 ROWS HERE:

<img width="878" alt="Screenshot 2024-10-27 at 2 57 29 PM" src="https://github.com/user-attachments/assets/74a00fb5-af2d-4214-99af-357e0721e0fd">


CONTINUE PART 2


