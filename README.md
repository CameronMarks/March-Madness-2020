# March-Madness-2020
Logistic regression model I put together to predict NCAA 2020 March Madness results 

In March of 2019, before I started learning about data science, I wanted to compete in a bracket challenge at work and like most people, I hoped to win. I have always enjoyed the excitement around March Madness even though I normally do not watch basketball and have not played since I was a kid. I love thinking about what it would take to select the winner of all 63 games and having perfect bracket (odds are 1 in 9.2 quintillion). So as an uninformed, non-basketball watcher, with a lot of Excel knowledge, I started looking for ways to help me better predict the NCAA 2019 March Madness results. After some google searched and not understanding much of what I was reading about, I decided to create a simple formula using 3 features I could easily find online for each team based on the 2019 season: Average Points For, Average Points Against, and Strength of Schedule. I weighted these three features evenly and used these scores I had generated to pick the team with the higher score for each matchup. In the end, as I had hoped I won the bracket challenge I had participated in at work without watching a single basketball game that season. My coworkers were extremely disappointed to have been beat by someone who hardly knows anything about basketball.

After the success in 2019, and after completing the Microsoft's Professional Program for Data Science on EdX in November of 2019, I set out to use my newly learned skills to see if I could do better in 2020 by developing a logistic regression model. 

Here is the logistic regression model I came up with based on tournament results from 2015 - 2019 to hopefully predict NCAA 2020 March Madness results. I used an 80% train, 20% test split and I was able to achieve a classification rate accuracy of 75.5%. This seemed rather good, but the ultimate test was going to be the always unpredictable NCAA 2020 March Madness Tournament. Unfortunately, as we all know today that the 2020 tournament ultimately got cancelled due to COVID-19. I hope to be able to use this again for the upcoming NCAA 2021 March Madness Tournament to see how it performs and so I can continuously make improvements for future tournaments. I had planned to submit my predictions into the official 2020 March Madness Kaggle competition as well to see how I performed in that competition. 

The source for this model is an CSV file I created using Excel and is based on information from the official 2020 March Madness Kaggle competition. I also pulled strength of schedule information from one of the major sports networks. Unfortunately, I don’t remember which one.

In the Kaggle competition, each team is given a unique ID number and the goal of the submission file is to predict the outcome (1 or 0) for every possible game combination that could happen in the tournament. The outcome of a 1 means the team with the higher ID beat the team with the lower ID. 
My dataset has the following 23 features. 12 are statistics about one of the teams in the matchup, 6 are comparison calculations between the teams in the matchup, and the rest are either categorical or necessary for the Kaggle competition submission.

Here are some details about each feature: <br>
•	Year<br>
•	Min Team<br>
•	Min Team Average For<br>
•	Min Team Average Against<br>
•	Max Team<br>
•	Max Team For<br>
•	Max Team Against<br>
•	Delta Average Points<br>
•	Delta Average Against<br>
•	Min Team Seed<br>
•	Max Team Seed<br>
•	Delta Seed<br>
•	Min Wins<br>
•	Min Losses<br>
•	Max Wins<br>
•	Max Losses<br>
•	Delta Wins<br>
•	Delta Losses<br>
•	Min SOS<br>
•	Max SOS<br>
•	Net SOS<br>
•	Combine Game<br>
•	Outcome<br>

