
## MIST 4610 - Group 6, Project 2

| Name | Email | GitHub link |
| :---- | :---- | :---- |
| Askari, Ali | [aa60263@uga.edu](mailto:aa60263@uga.edu) | [https://github.com/AwpDemon/MIST-4610-2](https://github.com/AwpDemon/MIST-4610-2) |
| Paul, Ryan | [rp78264@uga.edu](mailto:rp78264@uga.edu)   | [https://github.com/ryanpaul434/MIST-Group-6-Project-2](https://github.com/ryanpaul434/MIST-Group-6-Project-2)  |
| Bloom, Kate | [kab64157@uga.edu](mailto:kab64157@uga.edu) | [https://github.com/kateabloom/MIST4610project2](https://github.com/kateabloom/MIST4610project2)  |
| Stewart, Whitman | [wls32139@uga.edu](mailto:wls32139@uga.edu)  | [https://github.com/whitnotmax/MIST4610-Group6-Project2](https://github.com/whitnotmax/MIST4610-Group6-Project2) |
| Oggu, Stephen	 | [sao16391@uga.edu](mailto:sao16391@uga.edu)    | [https://github.com/SpeedRacerAMG/MIST4610TAB](https://github.com/SpeedRacerAMG/MIST4610TAB) |

			

**Describing your dataset and what data it contains:**

This dataset provides records of crime incidents in the City of Los Angeles dating back to 2020\. The records were provided by the Los Angeles Police Department’s Records Management System, and the dataset was obtained from data.gov.

![columns and datatypes](https://i.imgur.com/9xPD0jZ.png)

## Question 1: What locations in Los Angeles are experiencing the highest levels of crime, and what factors about these areas might affect the crime rates?

![LA crime heatmap](https://i.imgur.com/35OpwHZ.png)

**Analysis and Results:**

Identifying crime hotspots helps communities understand which neighborhoods are more vulnerable, helping residents take precautions or advocate for better policing and resources. Wealth inequality likely contributes to this trend, since areas with high crime rates often see decreased property values, struggling businesses, and fewer investment back into the community. Downtown Los Angeles is home to skid row, and the area suffers from widespread homelessness, similarly to Hollywood, as it is also home to many high-earning stars but is unaffordable for the average person.

**The manipulations applied to the data set as part of the analysis:**

We had to overlay the location of each neighborhood, so we overlaid a second map visualization with the dual-axis feature, having the second map showing the median latitude and longitude of each neighborhood represented in the dataset. While each crime was committed in a unique geographical latitude and longitude, each crime also includes the information on the nearest neighborhood that the crime occurred in, so this approach allowed us to find the approximate location of each neighborhood and include it in the visualization.

## Question 2: At what times is criminal activity most impacting the safety of Los Angeles communities, and how can this inform preventative crime measures?

![Crime hourly visualization](https://i.imgur.com/uXvGjdv.png)

**Analysis and Results:**

Understanding the timing of a crime, like the time of day, day of week, and season can inform urban planning strategies, such as improving lighting and security in public spaces during peak crime times, and help community organizations plan prevention programs that address specific hours of higher risk. This data is reported from the LAPD Records Department Systems, and therefore includes reports of crimes, not necessarily all the crimes themselves. Since crimes are more likely to be reported when witnesses are present or when access to authorities is easier, which often occurs during daylight or work hours, this might contribute to the spike in crime during the day. Additionally, in this dataset, men are most frequently victims, and this may be due to the fact that men may feel a stronger sense of responsibility to take action when witnessing a crime, especially when other men are victims, as societal norms often associate masculinity with assertiveness and protection.

**The manipulations applied to the data set as part of the analysis:**

* For the second graph, since the data is obtained from the Los Angeles Police Department Records Management System, a lot of the data from 2024 and 2025 was incomplete, so we excluded those years from the data set.   
    
* Additionally, to get our x-axis on an hourly basis, we created an HourOcc calculated field from the Time Occ field. It pulls the first two digits, which represent the hour, from the four-digit TimeOcc number using this formula: INT(\[ Time Occ \] / 100). 

## Packaged Tableau Workbook File
https://drive.google.com/file/d/1r7tSyTPmHMEqjn-N01tOoMBKlTgKPHFF/view?usp=sharing

