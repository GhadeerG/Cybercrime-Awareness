
# Phishing Websites EDA
This if the first Project of T5 Data Science Bootcamp

# Abstract
The Aim of This analytical project is to find out the similar characteristics of links that are suspicious to be phishing links, and measure the awareness toward this common cybercrime method.

<img width="528" alt="Screen Shot 2021-11-21 at 3 05 10 AM" src="https://user-images.githubusercontent.com/93079431/142744445-ccf960d5-0ccd-457f-a5ed-9111929e2872.png">

# Design
**I used two datasets:**
1. [Phishing Websites Dataset](https://www.sciencedirect.com/science/article/pii/S2352340920313202) [click to find the source]

It was challenging to find out a local dataset of phishing websites, therefore I used a worldwide dataset extracted from ScienceDirect website.

2. [Cybercrime Awareness among Saudi Nationalities](https://www.sciencedirect.com/science/article/pii/S2352340921002493) [click to find the source]

In light of the lack to find a local cyber dataset, I was lucky to find one! it's also from ScienceDirect to measure the cybercrime awareness of Saudis, although it's a simple sample but it was very useful.

# Data Cleaning

**1. Phishing Websites Dataset Cleaning**

The dataset got 112 Features and 58,646 rows Divided into 6 tables, Each table indicates a specific part of the link.

We must know in advance that any link is divided into 4 parts as we can see in the figure below.

<img width="785" alt="Screen Shot 2021-11-21 at 3 34 35 AM" src="https://user-images.githubusercontent.com/93079431/142744908-10b4ee0a-4900-4e3c-8aec-65bc43bc3c14.png">

The dataset divided the symbols allocated in each part, some data Scientists want to check the domain, Some want to check the dictionary while
my main goal was checking the whole URL, so I shrinked the dataset to meet the goal expectation.

Here i just extract the 

I used only the feature that includes "URL" in the header, such as "URL length", "Quantity of $ in URL", "Quantity of & in URL" and so on..
All numbers should be 0>=, while some values were -1 which doesn't make sense! either there will be a symbol or not.
                                                                

**2. Cybercrime awareness among Saudi nationalities Cleaning**

It's a survey about cybercrime awareness that got 64 features and 1,211 rows, the only two questions that meet my project goal "How much do you check the source of a website before accessing it ?" and "Have you been a victim of cyber crime?"

# Data Analysis

At first, I was curious About how many users from the local sample that I have that make sure they check the legitimacy (source) of the link before accessing it.



<img width="588" alt="Screen Shot 2021-11-21 at 12 16 16 AM" src="https://user-images.githubusercontent.com/93079431/142745675-1a04c4b6-36b9-4224-b842-f02c11f66383.png">

The result was satisfying enough to indicate the high awareness of cybercrime that may accrue by phishing links.

let's check how much of them got phished.

<img width="549" alt="Screen Shot 2021-11-21 at 12 49 39 AM" src="https://user-images.githubusercontent.com/93079431/142745780-0c0a2abb-88e4-4654-acd1-ad4e90e8a46f.png">

Almost 22% of the users got phished at least once, why? 
let's check if even those who make sure to check the source of the link are included in the the area of users who got phished?

<img width="500" alt="Screen Shot 2021-11-21 at 4 36 23 AM" src="https://user-images.githubusercontent.com/93079431/142745899-9c214327-14aa-43ef-9f3f-e313c40ce154.png">


Yes they got phished and even the number of users who always make sure to check the source of the link are near to those who often check it.

how we can avoid such a thing from happening in the future?

# Communication and Deliverables

I took all the symbols that potentially stuffed in the phishing links and represented them in the bar chart to see which factor will be the red flag to the user, As we can see below that the the URL length is the most likely factor considered.

<img width="580" alt="Screen Shot 2021-12-02 at 10 29 22 AM" src="https://user-images.githubusercontent.com/93079431/144377164-80bfcecb-acd6-4d81-8c0c-fa81e76b80e0.png">

the length of URL was the highest so it will be a big red flag to any user who is willing to click on a link.

and let's see more..

<img width="646" alt="Screen Shot 2021-12-02 at 10 33 34 AM" src="https://user-images.githubusercontent.com/93079431/144377700-009c369b-0189-43eb-bd5a-0ed1d3be4f2e.png">

However, the repetition of these symbols should notify the user to be careful.

# Future Work

Due to the limited time that we have in this bootcamp to deliver the outcomes of this project which is only 2 weeks, i stopped tell this point, in future work:
1. Make a module that will allow the user to insert any link that he/she is suspicious about and the module will represent how much out of 100% it's suspicious to be phishing.
2. Making a huge local dataset of phishing websites similar to [PhishTank.org](https://phishtank.org/)
