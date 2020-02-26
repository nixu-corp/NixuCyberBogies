## Gameplay instructions

Nothing motivates like a winning a game, right? If you want to compete against your workmates in finding threats actors and attack vectors, you can use the following instructions to play a time-boxed game and score your findings.
Amount of players

* minimum 2
* maximum: 12

### Preparations

* Shuffle the deck of Cyber Bogie cards
* Give a Cyber Bogie and Threat Discovery Template card and a pen to everybody
  * [nixu-cyber-bogies-scoring-template.pdf](https://github.com/nixu-corp/NixuCyberBogies/blob/master/Gameplay%20instructions/nixu-cyber-bogies-scoring-template.pdf)
* Introduce the system to be threat modeled to everybody
  * Explain the purpose of the system
  * Explain what kind of data is handled in the system
  * Show/draw architecture diagram (data stores, APIs, user interfaces, etc.)
  * Explain use cases of the system for different user roles; what they actually do with the system
  * This part is important. Otherwise, it is difficult to find threats
* Ideally: Everybody takes some time to familiarize themselves with the Cyber Bogie cards, so using them is faster.

### Gameplay

1. Select the first player (throw dice or whatever suits you)
2. The first player (Player in Turn) takes a Cyber Bogie card
3. The Player in Turn reads out loud /explains the card to others

  * If you can, show the Cyber Bogie card with a projector to everybody

4. In silence, everybody writes down the threats they come up with

  * 3 minutes max or until everybody is ready

5. The Player in Turn explains all threats (attacks + motivation) they came up with
6. Other players can comment if they know existing mitigations or that the threat is irrelevant
7. Players mark their points so far
8. Other player take turns, starting from the left of Player in Turn, explain additional threats they found
9. Other players can comment if they know existing mitigations or that the threat is irrelevant
10. Players mark their points so far
11. The second player (to the left) picks a Cyber Bogie card
12. Go to step 3

### Scoring

##### Scoring for Player in Turn

The Player in Turn is the one who picked the Cyber Bogie card and first listed the threats they discovered.

  * 1 point for each new attack vector
  * 1 point for each motivation
  * -1 point if another player finds a mitigation for your threats

##### Scoring for other players

Other players have their opportunity, one per time, to list new threats that the Player in Turn did not mention

  * 2 points for each new attack vector
  * 1 point for each new motivation
  * 1 point for each mitigation to someone else's threats


### After the game

We really recommend you to also continue working with the threats you discovered. If you haven't created a threat model earlier, this is a good point to start!

Be sure to check that you have existing mitigations for the threat scenarios. If you don't, do some investigation and add the mitigations to be implemented to your backlog.

And when you are designing new features, you can go back to the Cyber Bogies you identified and think about what harm they could do.

