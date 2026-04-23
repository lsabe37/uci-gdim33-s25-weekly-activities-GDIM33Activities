# GDIM 33 In-Class Activities
## W1
### Activity 1
[Inspiration Board](https://docs.google.com/drawings/d/1zFPV6EeXjZNqpYmVUOlbokhXd3I6e1T33Lh5B-8W4HU/edit?usp=sharing)

1. I am interested in difficult games. Specifically, these include 2D-platformers and or bullet hell games like Cuphead, Hollow Knight, and Touhou. In these games, the player needs to dodge/parry a large number of complex enemy attacks. The games I am interested mainly feature a line up of complicated and memorable boss fights. The aesthetic I am interested in are vintage and child-like. These aesthetics contribute to creating a dream-like world. 

2. Eric enjoys playing souls games like Elden Ring. I also enjoy playing souls games.

3. Josh enjoys playing competitive games (ex. League, R6, Apex Legends, Overwatch). His tastes are not similar to mine.


### Activity 2
Original Concept: This game will be a combination of two different game modes. There will be an anomaly hunt / cooking game mode and a 2D platformer / bullet hell mode. The game will start off in the cooking game mode. This mode is mainly here to tell the story. The game switches to 2D platformer when the player triggers a battle. The core gameplay loop wil be as follows: the player identifies whether the customer they are serving is real or an imposter. If they are real, the player will serve the customer. If they are fake, the player will shoot the customer. When the player shoots a fake customer, they will trigger a boss fight which will take place in the form of a 2D platformer. Once the boss is defeated, the player returns to the anomaly hunt cooking game mode. The player needs to find and defeat enough fake customers to win the game.

[Breakdown](https://docs.google.com/presentation/d/1V5xXVmgtFbwtfhezYsHWtT8_yKYKTivaR_gJYe6Lf6Y/edit?usp=sharing)


## W2



## W3

### Activity 1

[Breakdown](https://docs.google.com/presentation/d/1V5xXVmgtFbwtfhezYsHWtT8_yKYKTivaR_gJYe6Lf6Y/edit?usp=sharing)


### Activity 2

1. It is useful to save the vent name for explore-to-dialogue state transition as a Scene variable so that it can be accessed from any part of the scene.

2. Using Debug.Log() nodes helped me check to see if the transitions between the dialogue state and explore state were working. It also allowed me to check early on if the onclick() function was working.

3. The Set Cursor Lock state is irrelevant to my vertical slice since my game will be 2D and the camera will either be fixed (during the anomaly hunt mode) or it will automatically follow the player (during the 2D platformer mode).

4. The concept of game states is relevant to my vertical slice since I plan to change certain visual elements of the background depending on actions that the player takes (such as turning the lights off). I can use game states to determine which apperance the background will take. 


## W4

### Activity 1

The in-store gameplay is partially playable at the moment. The playtest build includes two NPC customers that will arrive one after another. When a customer arrives, their unique intro dialogue will play. Then, the player can select between two questions to ask the NPC and they will answer. There are 4 action buttons that the player can click on. The first pulls up an ID card with the Sprite of the corresponding NPC in front of them. The second button turns off and on the lights, which is achieved by adjusting the rgb values of the background sprite. The third button will cause the player to give a spicy donut to the NPC, which triggers their reaction dialogue. The fourth button will bring up the gun reticle, and then the player can press "S" to shoot the NPC. When shot, the background will turn red and the NPC will give their reaction dialogue and then leave. The player can also switch between the donut view and store view using the navigation buttons. On the donut side, there are 4 donuts that the player can click on to give to the customer. If the player clicks on the correct donut, the customer will provide a positive reaction dialogue. If the player gets the order wrong, the camera will shake and the customer will give their incorrect dialogue. When the player gets an order wrong, their sanity meter goes down. When they get an order right, their sanity meter goesn up. When the NPC's give different responses and reactions, their sprite will change to the corresponding emotion.

My playtesting goal is to see whether or not the button UI's are easy to understand and use. Another goal is to see whether or not the NPC's dialogue are interesting or bland. The third goal is to see if the NPC's give the correct dialogue responses depending on the player actions without any issues.

I playtested with Eric and Han.

Playtesting notes: The rainbow effect on the sanity bar created an interesting visual aesthetic. The background changing adds emphasis to the reactions. The dialogue system sometimes had bugs where the dialogue box gets disabled early.

### Activity 2

If the programmer programs a branching dialogue system which utilizes dialogueObjects, then the writer should be able to add more dialogue to the game without having to write any code. However, if not, then the writer would need to write more code in order to add more dialogue.

There is no limit to the number of dialogue nodes that the writer could create without writing any code. 

The purpose of the "Regenerate Nodes" button is to provide an easy way to add new nodes to the node library.