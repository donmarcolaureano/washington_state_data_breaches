# Washington State Data Breaches


Washington law requires entities impacted by a data breach to notify the Attorney General’s Office (AGO) when more than 500 Washingtonians personal information was compromised as a result of the breach. This dataset is a collection of various statistics that have been derived from these notices, and is the source of data used to produce the AGO’s Annual Data Breach Report.

## Data Source
The <a href="https://data.wa.gov/Consumer-Protection/Data-Breach-Notifications-Affecting-Washington-Res/sb4j-ca4h/about_data"> data </a> for this project was provided by the <a href="https://www.atg.wa.gov/data-breach-notifications">Washington State Attorney General's Office</a>

## Data Dictionary

| Column Name | Description |
| ----------- | ----------  | 
| DateAware | The data the notifying entity became aware that a breach impacting Washington residents had occurred | 
| DateSubmitted | The date the notifying entity submitted their notice to the Attorney General’s Office | 
| DataBreachCause | The cause of the data breach. Three categories are available [^1] |
| DateStart | The known or estimated start date of the breach | 
| DateEnd | The known or estimated end date of the breach | 
| Name | The name of the entity providing notice to the Attorney General’s Office [^2] | 
| Id | Unique Key | 
| CyberAttachType | This is a sub-category of breaches caused by Cyberattacks [^3] | 
| WashingtoniansAffected | The estimated or known number of Washington residents whose information was affected by the data breach | 
| IndustryType | The industry type that the notifying entity belongs to [^4] |
| BusinessType | A sub-category of notifying entities who are categorized as Businesses [^5] | 
| Year | The “year” in which a data breach notice is submitted to the Attorney General’s Office (AGO) [^6] | 
| YearText | Year in text formatting for visualizations | 
| WashingtoniansAffectedRange | Range of Washingtonians Affected for visualizations | 
| BreachLifecycleRange | The lifecycle of a breach is the sum of the “Time to Identify”, and “Time to Contain” a breach [^7] | 
| DaysToContainBreach | The total number of days it takes a notifying entity to end the exposure of consumer data, after discovering the breach [^8] | 
| DaysToIdentifyBreach | The total number of days it takes a notifying entity to discover that a breach of consumer data has occurred after the breach has begun | 
| DaysBreachLifecycle | The lifecycle of a breach is the sum of the “Time to Identify”, and “Time to Contain” a breach. This data is measured in days. | 
| DiscoveredInProgress | Whether or not a notifying entity discovered a breach while it was still in progress | 
| DaysOfExposure | The total number of days that consumers’ information was exposed by a breach | 
| DaysElapsedBetweenEndAndDiscovery | The total number of days that elapsed after the exposure of consumers’ data ended, and when the notifying entity actually learned of the breached | 
| EndedOnDayDiscovered | Whether or not the exposure of consumers’ information ended on the same day that the notifying entity discovered the breach | 
| DaysElapsedBeforeNotification | The number of days that elapsed before the notifying entity submitted notice to the Attorney General’s Office | 
| DaysOfExposureRange | Range of Days of Exposure for visualizations | 
| EntityState | The US state of the entity if one was provided | 


[^1]: Cyberattack: when a third party deliberately attempts to access secured data, such as information stored on a server, using cyber technology. 
Unauthorized access: when an unauthorized person purposefully accesses data through means such as an unsecured network or sifting through sensitive documents left out on a desk. 
Theft or mistake: the mistaken loss of information, such as a clerical error, or the inadvertent theft of information

[^2]: This is nearly always the owner of the breached data, whether or not they were the entity to be breached. E.g. If Company A contracts with Company B to process their data, and Company B is breached, Washington law requires Company A to provide the notice.

[^3]: Tracked Types: Malware, Ransomware, Phishing, Skimmers, Other, and Unknown

[^4]: Options include: Business, Education, Finance, Government, Health, and Nonprofit or Charity.

[^5]: Options include: Accessories, Biotech, Cleaning, Clothing, Construction, Consumable, Cosmetic, Cryptocurrency, Entertainment, Fitness, Home, Hospitality, Human Resources, Legal, Manufacturing, Professional Services, Real Estate, Retail, Shipping, Software, Telecommunications, Transportation, and Web Services. There is also an “other” category to capture any businesses that do not fit into the above.

[^6]: As a result of the effective date of the law requiring notice to the AGO, a year starts on July 24 and ends on July 23 of the following year. In other words, a notice submitted on July 23, 2020 would be marked as a “2020” breach, while a notice submitted on July 24, 2020 would be marked as a “2021” breach.

[^7]: If one or both of these variables is unknown, then the Lifecycle is unknown as well. This data is measured in days, and categorized into one of the following buckets: 0 days, 1-99 days, 100-199 days, 200-299 days, 300-399 days, 400-499 days, 500+ days, and unknown. 

[^8]: If a breach ends before it is discovered, this column will be marked as “0”

## Annual Number of Washingtonians Affected by Data Breaches Since 2016
![Screenshot 2024-06-16 at 1 38 42 PM](https://github.com/donmarcolaureano/washington_state_data_breaches/assets/140132043/67b23acd-4ba0-475b-a728-3970df103e36)

<a href="https://github.com/donmarcolaureano/washington_state_data_breaches/blob/main/WA%20AOG%20Data%20Break%20Report%202023.pdf">Source</a>

## Data Breaches by Cause
![Screenshot 2024-06-16 at 1 32 29 PM](https://github.com/donmarcolaureano/washington_state_data_breaches/assets/140132043/487a8816-cd95-47c6-9cc9-c207aa44ab7a)

<a href="https://github.com/donmarcolaureano/washington_state_data_breaches/blob/main/WA%20AOG%20Data%20Break%20Report%202023.pdf">Source</a>


## Types of Personal Information Exposed
![Screenshot 2024-06-16 at 1 37 41 PM](https://github.com/donmarcolaureano/washington_state_data_breaches/assets/140132043/ee17e975-0938-46db-aa23-252fc71a0876)

<a href="https://github.com/donmarcolaureano/washington_state_data_breaches/blob/main/WA%20AOG%20Data%20Break%20Report%202023.pdf">Source</a>


