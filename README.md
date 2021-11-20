# Phishing-Websites EDA

In this repository, I'll be gladly sharing all the materials i worked on for the first Project in SDAIA (Saudi Authority for Data and Artificial Intelligence) T5 Data Science Bootcamp.

<img width="379" alt="Screen Shot 2021-11-20 at 11 24 59 PM" src="https://user-images.githubusercontent.com/93079431/142739984-29716bd9-5f51-4220-9b91-e14f0a897745.png">

This project is about how to recognize and differentiate between links that are considered suspicious "Phishing" links or not and how much people are aware of that.

Could this link be a phishing link?

To catch that goal, first, I analyzed a local dataset that used to measure the level of cybersecurity awareness of cybercrime in Saudi Arabia.
The most important question was: How much do you check the legitimacy of a website before accessing it? the answer in the pie chart down.

<img width="588" alt="Screen Shot 2021-11-21 at 12 16 16 AM" src="https://user-images.githubusercontent.com/93079431/142741659-860c05a6-9ac7-4149-b686-feec028ec813.png">

Almost 42% of Saudis in this sample check the source of the link which is a good indication of the cybercrime awareness but let's see how much of them got phished at least once since they started using the internet.

<img width="549" alt="Screen Shot 2021-11-21 at 12 49 39 AM" src="https://user-images.githubusercontent.com/93079431/142741869-ef88de61-98e7-408f-afbf-c653158d4188.png">

22% got phishsed! How can I -As a tech savvy/Data Scientist- notify them?

I took all the symbols that potentially stuffed in the phishing links and represented them in the bar chart to see which factor will be the red flag to the user, as we can see below that the the URL length is the most likely factor considered, then top 5 symbols come right after are: slash (/), dot (.), and (&), tld (.com) and hyphen (-) as you can see in the below bar chart.

<img width="475" alt="Screen Shot 2021-11-21 at 12 22 36 AM" src="https://user-images.githubusercontent.com/93079431/142741366-761cf687-a26c-4a35-92a4-832492d40571.png">

However, the repetition of these symbols should notify the user to be careful.


Good protection from phishing comes first by educating myself and people around me.
