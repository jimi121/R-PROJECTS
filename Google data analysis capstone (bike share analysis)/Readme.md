# Cyclistic Bike-Share: Google Data Analytics Capstone Project
![image](https://github.com/jimi121/R-PROJECTS/blob/main/Google%20data%20analysis%20capstone%20(bike%20share%20analysis)/bike-share.png)
This repo contains the Google Data Analytics Capstone - Case Study 1 project, which is the final stage of the Google Data Analytics course on coursera. I hope this repo will help everyone who wants to do this project. thanks.

## Introduction and Scenerio

**Google Data Analytics Capstone Project: How Does a Bike-Share Navigate Speedy Success?**

The Cyclistic case study is part of the Google Professional Data Analytics Certification. In this case study, I play the role of a junior data analyst at Cyclistic. I will follow basic data analysis process steps to solve core business problems.
I'm a junior data analyst working on the marketing analyst team at Cyclistic, a bike-sharing company in Chicago. The marketing manager believes the company's future success will depend on maximizing annual memberships. Therefore, as a marketing team, he wants to understand how cyclistic bikes are used in different ways according to membership types. Here, my task will be to review and analyze 12 months of data, to obtain insights from this data through certain visualizations and present it to the team. I have analyzed very specific data and tried to support these insights with clear graphs so that my suggestions can be taken into account.

**About the Company**

In 2016, Cyclistic launched a successful bike-share offering. Since then, the program has grown to a fleet of 5,824 bicycles that are geotracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system anytime. Until now, Cyclistic’s marketing strategy relied on building general awareness and appealing to broad consumer segments. One approach that helped make these things possible was the flexibility of its pricing plans: single-ride passes, full-day passes, and annual memberships. Customers who purchase single-ride or full-day passes are referred to as casual riders. Customers who purchase annual memberships are Cyclistic members. Cyclistic’s finance analysts have concluded that annual members are much more profitable than casual riders. Although the pricing flexibility helps Cyclistic attract more customers, Moreno believes that maximizing the number of annual members will be key to future growth. Rather than creating a marketing campaign that targets all-new customers, Moreno believes there is a very good chance to convert casual riders into members. She notes that casual riders are already aware of the Cyclistic program and have chosen Cyclistic for their mobility needs. Moreno has set a clear goal: Design marketing strategies aimed at converting casual riders into annual members. In order to do that, however, the marketing analyst team needs to better understand how annual members and casual riders differ, why casual riders would buy a membership, and how digital media could affect their marketing tactics. Moreno and her team are interested in analyzing the Cyclistic historical bike trip data to identify trends.
In this case-study, I will be drawing upon the 6 phases of the analysis process, namely Ask, Prepare, Process, Analyze, Share and Act.

I downloaded the datasets from the link below.

[2022 Cyclistic trip data](https://divvy-tripdata.s3.amazonaws.com/index.html)

## Phase 1 – ASK 

Three questions will guide the future marketing program: 

1.	How do annual members and casual riders use Cyclistic bikes differently? 
2.	Why would casual riders buy Cyclistic annual memberships? 
3.	How can Cyclistic use digital media to influence casual riders to become members?

**1.1	Business Task**

Analyze data to gain insights into how users use Cyclistic's bikes by membership type and to identify trends based on Cyclistic's marketing strategy. 

**1.2	Key Stakeholders**

•	Cyclistic: A bike-share program that features more than 5,800 bicycles and 600 docking stations. Cyclistic sets itself apart by also offering reclining bikes, hand tricycles, and cargo bikes, making bike-share more inclusive to people with disabilities and riders who can’t use a standard two-wheeled bike. The majority of riders opt for traditional bikes; about 8% of riders use the assistive options. Cyclistic users are more likely to ride for leisure, but about 30% use them to commute to work each day.

•	Lily Moreno: The director of marketing and your manager. Moreno is responsible for the development of campaigns and initiatives to promote the bike-share program. These may include email, social media, and other channels.

•	Cyclistic marketing analytics team: A team of data analysts who are responsible for collecting, analyzing, and reporting data that helps guide Cyclistic marketing strategy. You joined this team six months ago and have been busy learning about Cyclistic’s mission and business goals — as well as how you, as a junior data analyst, can help Cyclistic achieve them.

•	Cyclistic executive team: The notoriously detail-oriented executive team will decide whether to approve the recommended marketing program.

**1.3	A clear statement of the business task**
The main purpose in this job role is to analyze Cyclistic data and gain insights for marketing trends based on user orientation and driving data and share them with key stakeholders. Specific and clear visualizations should be made and ready for sharing so that all stakeholders can understand the data.

## Phase 2 – PREPARE
The data is available at the address I gave the link above. The data I have downloaded from this address have been handled in a way to cover 12 months, January 2022 and December 2022. Many tools and programs can be used to edit data. I chose the R programming language for my work. In the R programming language, I combined 12 months of data into a single data frame, then added the necessary columns and removed the columns that would not be useful to us in our analysis. 

The data appears to be ROCCC (Reliable, Original, Comprehensive, Current, Cited). There don't seem to be any issues with bias or credibility in the data, as it consists of trip data from Cyclistic's own bike riders and is made available under license by Motivate International Inc. Additionally, the data appears to be reliable, original, comprehensive, current, and cited, meeting the criteria for ROCCC.

It is important to adhere to any licensing restrictions when using publicly available data. As mentioned in the prompt, the data is made available under a specific license, and users should review and comply with any requirements or restrictions specified by the license. To address privacy and security concerns, any personally identifiable information should be removed or obscured from the data. Additionally, it is important to ensure that the data is accessible and usable by anyone who needs to work with it.


## Phase 3 – PROCESS
I used the R programming language to process the data and make it ready for analysis. Thanks to its simple syntax and fast usage, I both consolidated my knowledge and analyzed and organized the data.
I managed to ensure the integrity of the data. I added 12 months of data to a single data frame, making it ready for a year's analysis.I have documented these operations and analysis process using R markdown

## Phase 4 – Analyze
First of all, the driving data had to be grouped according to user types, hours, time zones of the day, days of the week, months and seasons, and I organized the data to be that way. As can be seen in the R markdown document that I just shared during the process phase, time columns were created and the driving data of the users were classified according to the time type. In addition to examining the average and total driving times of the user types, the driving time lengths were also extracted from the data in the data frame, such as the end and start time, and included in the analysis, and important insights were obtained.

## Phase 5 - SHARE

Of course, after analyzing this data, visualizing it and sharing it with stakeholders is a very important step. 

## Phase 6 – ACT

### Summary of insights 

Members and casual riders differ in how long they use the bikes, how often they use the bikes, and on which days of the week does every group peak:

* Casual rides peak during weekends. There is a high probability they are tourists visiting and sightseeing the city, or that they are ordinary Chicago residents who are riding bike in their leisure time during the weekend. The longer average ride time for casual rider, also peaking at the weekend,  provides evidence for this point.

* Ride length for members are relatively shorter compared to casual riders. This could clarified as such, that most members use the bikes to commute on workdays. This clarification would also explain the short riding durations of members. They ride from point A to B, namely roughly always the same ride lengths and the same distance

* Ridership start to pick up from February (from Spring through Summer)and start to decrease in August (from Fall through winter). This correlation is due to the seasonal changes. As the weather start to get warmer and more pleasant in February (start of Spring), more people starts to cycle, and inversely when the weather  becomes less warm cold around September (start of Fall).

* More than 50% of the riders are annual members, suggesting that the company have already achieved a certain level of loyalty among its bike users. This indicates a positive message, namely that the company is going to be able to convince many casual riders to convert to members, and to keep the new members satisfied. 

# Conclusion and Recommendation

Final Conclusion and Recommendation

My answers to the three questions that will guide the future marketing program are as follows, based on my analysis and visualizations:

**How do annual members and casual riders use Cyclistic bikes differently?**

• Our annual members use the Cyclistic bike sharing service frequently and consistently in terms of total ride and ride time. It has shown that users prefer bicycles to other types of vehicles on issues such as cost, environmental pollution and traffic to use for certain jobs. 

• On the other hand, casual riders do not use the bike frequently and consistently. Therefore, it is understandable that they do not prefer to switch to the annual membership plan. Despite this, casual riders like to cycle inconsistently compared to annual members, with long rides on weekends that we think are for fun and relaxation.

• Annual members are very likely to opt for the annual membership plan, as their daily and weekly routines are set. The fact that users have school, work and other activities at certain time intervals seems to push them to use a certain means of transportation in a planned way. Due to this planned use, annual membership seems quite reasonable to meet the needs of such members.

•	As a result, usage differences give us information about drivers' tendencies and behaviors. These differences vary according to the drivers' behaviors and perceptions of use.

**Why would casual riders buy Cyclistic annual memberships?**

In the light of the analysis and visualizations I have made, the suggestions I can give to the marketing team on how casual riders can be converted into annual members are as follows:
• The advertising and marketing strategy to get casual riders to get their annual subscription plan should be around very specific issues. These issues are the cost of cycling, health, environmental health, traffic, etc. It should be noted that the benefits in these subjects are more than other tools.

• In the light of the analyzes I have made; it has been observed that the reason for the annual members to use the service stems from their instincts to stick to their planned and routines in their lives. For this reason, mobile applications can be developed to encourage casual riders to move on to a planned life, and advertisements can be made for users to create routines at certain times of the day and use Cyclistic bicycles as a means of travel to these routines.

• It is a known fact that time and money are very important in today's societies. For this reason, the transition to the annual plan can be encouraged by reducing the costs of the annual membership plans and by making special campaigns, sweepstakes, coupons and discounts for people who switch to the annual membership plan. Thanks to the agreements to be made with different establishments (food restaurants, cafes, book stores, entertainment centers, etc.), a system can be developed in which users can use the points they earn according to the number and frequency of driving in these establishments.

• A system where driving time and number can be tracked would be very useful. Thanks to the application to be integrated into smart devices, it can be connected to other mobile applications such as Google fit and Apple Health, and the data can be created in the minds of users to create the perception that they are doing an activity to protect their health with their daily driving goals.

**How can Cyclistic use digital media to influence casual riders to become members?**

• The impact of social media on marketing and campaign processes in recent times is an undeniable fact. For this reason, encouraging campaigns can be organized using social media platforms. YouTube, Facebook, Twitter, TikTok etc. With the community and activity groups to be created on social media platforms, it can be ensured that members can share in these groups. In these community and group events where existing members will register, activities such as cycling and collective trips to certain points can be organized and shared on social media accounts. Especially with the planned activities to be held on social media, effective communication can be ensured between our current users and this communication can be met on social media and attract new users to our structure.

• Various agreements are made with the faces known to the public from social media phenomena, and the sharing of these people about the Cyclistic company in their accounts can cause a significant increase in the number of members.

• Especially in media sharing tools such as YouTube and TikTok, agreements with influencers who have a channel on travel will be very effective, and the owners of these channels will use their Cyclistic bikes on their trips and make special coupons and discount draws for people watching their videos. Historical, cultural, touristic, etc. Collective trips to places can be organized through these channels and shared on social media, thus attracting the attention of more users.

This comprehensive analysis provides actionable insights for Cyclistic to tailor marketing strategies and enhance annual memberships, ensuring sustainable growth.
