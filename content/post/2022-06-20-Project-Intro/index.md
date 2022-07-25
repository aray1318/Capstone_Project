---

title: Intro to PGA Tour Metrics for Playoff Events

author: Andrew Raymond

---

## Abstract 

The sport of golf and specifically the PGA Tour and its players undervalue data surrounding player metrics. Other sports use metrics to give players a competitive advantage in certain situations, golf needs to do the same. My goal is to find out which metrics play the most significant role in the PGA's playoff tournaments. This can allow players to sharpen specific skills to give them the best advantage.

## Context 

The metrics used on the PGA Tour are incredibly in depth and powerful yet, they are undoubtedly not used to their fullest potential. Many of the articles on the internet and statistics shown on broadcasts inform the audience on general trends and overall metrics for players. However, shouldn't the players and audience know what metrics are best suited for specific tournaments on tour. The PGA Tour is very exploratory by simply looking at season long trends, this only tells part of the story. Certain tournaments and courses are undoubtedly tailored to specific play styles. All players should know what metrics are most important for a given tournament in order for them to prepare their game to the best of their ability.

Some high tier players may already have access to this sort of information solely due to their name and or resources. However, younger or newer players on tour do not they are fighting just to retain status for the coming year. Players regardless of status deserve equal access to course insides and information regarding which metrics are most important for not only the playoff events but for the other forty-five tournaments each year. Another aspect is the viewer. The viewer should have access to the information as well because it makes the avid golf fan more invested and interested in a golf tournament. By making the information public it allows equal access to players and can grow the game and take it to a place it never has before.

## Description of Data

The data I am using called pga_tour2.csv was located via kaggle from the user Jong. It has season by season data for players from years 2010-2018. The other data set called pga_tour.csv was from the website advancedsportsanalytics.com. This data set has tournament to tournament data ranging from 2015-2021. These data sets have various strokes gained metrics and placement for tournaments. These are the primary features that I will be using for my research. The excess columns were dropped as they are not relevant to my research. The limitations of the data is that there are tournaments such as major championships that have no data. Since there was missing data for a few tournaments I am focusing on the playoff events which had minimal data missing.

## Proposal 

What I am interested in researching is what player metrics have correlation with success for the PGA Tour's three playoff events. There are obvious metrics such as strokes gained which tells a player how well they performed in regards to all players for a specific tournament. But, I am interested in finding the more specific metrics that tell the little pieces of the whole story. For reference here are some metrics that will be used: GIR (green in regulation), driving distance, sg putting, scrambling, gir percentage form varying distances, scoring average, etc. For reference strokes gained lets players know how well they played in comparison to the rest of the field of players.

There are a few techniques that can be used to answer the research question. First, I will use logistic regression to predict a player's chance of making a cut, top twenty finish, etc. I will also use decision tree's specifically the random forest model for predicting winners. Along the way I will find what variables (metrics) are most important for different outcomes such as making the cut, top twenty, top ten, and winner.

The metrics for finish classification will undoubtedly not stay constant. The most significant metrics will change as the finishes get better and better. I also do not expect the metrics to stay constant throughout the three playoff tournaments given that each tournament has a different style. I do expect metrics such as sg putting, green in regulation percentage, and sg driving to be some of the most significant in determining a player's finish. 

## EDA

The PGA Tour Playoffs consists of three events. The first being the Northern Trust followed by the BMW Championship, and lastly the Tour Championship. For each tournament I filtered out past champions so I could see what metrics ranked the highest. I then took the average of each metric to get a general understanding of the historical trend. The metrics that were the most important for winning the Northern Trust were strokes gained total, strokes gained tee to green, and strokes gained approach. For the BMW CHampionship the most significant metrics were strokes gained total, strokes gained tee to green, and strokes gained putting. The metrics that were the most important for winning the Tour Championship were strokes gained total, strokes gained tee to green, and strokes gained off the tee.

For determining season long success I filtered out players with the most Fedex Cup Points each season. The metrics that were rated the highest for season long success were strokes gained total, strokes gained approach. I also created a basic model for determining if a player will win a tournament in a given season. The most significant indicators that were correlated with winning were points (which is fairly obvious because points are determined by how well you place in a tournament). Average score and number of top tens were also highly correlated (top tens essentially mean that a player has put themselves in more opportunities to win). Then lastly we had strokes gained total, strokes gained off the tee and scrambling (amount of times a player makes par or better when missing the fairway/green). 

## Conclusion 

The players on the PGA Tour obviously do not have equal access to resources such as research, coaching, and money. This fact alone leads to a bias for the higher tiered players in the game. Which is part of the reason why it is harder for new players to the tour to not only win but to maintain PGA Tour status. Players on the tour should have equal access to insight on tournament and golf course analysis. My goal is to find what metrics are most significant for the PGA Tour playoffs. Which will allow players to tune their game knowing specifically what they should be working on to give them the best chance at performing well. 

The metrics are a limitation for my research, the metrics are all predefined by ShotLink. I am bound to the previously recognized metrics for the game of golf. If I were to engineer new features or metrics they would not be recognized by the golf community. Another limitation is simply resources and time. There are forty-eight tournaments and I do not have the man power to perform analysis and provide insight for each and every tournament. Future directions would be to solve this very limitation and create a website that has analysis on every single PGA Tournament and provide insight for which metrics are most crucial for every tournament, along with which players are best suited for a specific event.




  
