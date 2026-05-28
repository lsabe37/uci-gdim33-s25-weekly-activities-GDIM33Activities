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


## W5

### Activity 1

#### Step 1: Create and import tilemap assets

Part A: Draw the Sprites on a separate sofware and upload the file asset to Unity.

Part B: Slice the Sprite into separate tiles.

Part C: Import the tilemap asset to the Tile Palette.

#### Step 2: Set up tilemaps in Scene

Part A: Add the regular tiles to the Scene to build the ground and walls.

Part B: Add the hazard tiles to the Scene to represent the traps. Adjust the Tilemap color to red to indicate that these tiles are dangerous.

Part C: Create a Hazard script for the hazard tiles which will reduce the player's HP by 5 points when collided with. This will be done using an OnCollisionEneter2D() method. When this method runs, it subtract 5f from the health float variable in the PlayerHealth script. Add a Debug log which shows how much HP the player has remainning.

### Activity 2

I created the tilemap assets and built the ground and walls for the boss room. I added in the hazardous tiles and created the Hazard script which reduces the player's HP. I also created the PlayerHealth script and the PlayerLocator script, which are used in this system. I currently have set up a debug log which shows the player's current HP upon taking damage.


## W6

### Activity 1
The new build includes 7 different customer NPC's for the anomaly hunt mode. This build has improved the UI for the anomaly hunt mode and fixed the dialogue system bugs. This build also includes the 2D platformer mode with a player and boss enemy. The player can move with WASD, jump, dash, and attack. The boss has a varied moveset.

[Itch build](https://masterfrog1.itch.io/vertical-slice-milestone-2)

The goal of this week's playtest is to see if the UI is easy to navigate in the 2D platformer section and to get the player's input on the customer designs and dialogue lines. Another goal is to get feedback on the 2D platformer section. This game mode is still largely in progress, so the main goal would be to get input on what boss moves feel to easy and what moves feel unfair or confusing.

Playtest notes: The UI is easy to navigate. The characters look interesting. There should be more windows to attack the boss (boss attacks too often). 

### Activity 2

1. The Multiply setting makes the color darker because it multiplies the rgb values which are values between 0 and 1 (which are fractions). Thus, the values will be smaller and results in a darker color.


2. If Multiply is used to combine the alpha values, it will result in a more translucent color. This is because it will multiply two fractions together, which will result in a smaller number.

3. The shader gets the UV values from the mesh data.

4. I found it interesting how I could use math to manipulate colors.

## W7

1. The data for the Vertex Color node comes from the mesh vertex.

2. The color of the shiba is blended at the edges of different regions of color because Unity is calculating the color for the pixels between the different regions.

3. The shiba is less detailed when using vertex color because the colors are only stored at each vertex point and then are interpolated across the surface. Vertex color is useful for optimization because of this. One use of vertex color would be to render a horde of enemies that are supposed to be seen by the player from a distance. Since there are many enemies and they don't need to be very detailed, vertex colors should be used.

4. The mesh's vertex normals appear awkward because they are not blended at the edges.

5. One other piece of vertex data that can be tested is the UV coordinates. UV coordinates would be useful to test because it will help debug issues that are related to the UV map.

6. There is an error in the lighting in step 5 because the light direction vector is pointing towards the shiba, however, the normal vectors are pointing away. This causes the lighting effect on the shiba to be inverted.

7. The Blend mode was set to Additive so that the texture will appear brighter. Since the texture is supposed to represent fire, changing the Blend mode to Additive can achieves a glowing effect that helps enhance the appearance.

## W8

### Activity 1

The new build includes a more fleshed out 2D platformer mode. The hitboxes for the boss' melee attacks have now been added, so the player will take damage when they get hit by any of the boss' attacks. The game over screen is now added to the 2D platformer mode. This screen will appear when the player's HP reaches 0. The game over screen features a retry button which will allow the player to reattempt the fight. The boss now has a mini familiar which flies around and shoots at the player when they are near it.

[Itch build](https://masterfrog1.itch.io/verticalslicetest3)

The main goal of this playtest is to see if the boss is too difficult. I would like to see if there are any attacks from the boss that are too hard to dodge/parry or feel unfair. The playtest will also be used to see if there are any bugs in the 2D platformer mode that I may have overlooked.

Playtest notes: It is unclear at first which healthbar is the player's and which is the boss'. It is unclear whether the boss angel familiar or the boss gameobject is the actual boss. The familiar should appear later.

### Activity 2A

1. The stencil buffer is being used to create the outline only around the shiba object. This is done by setting the layer mask to Outline only. By doing this, the Renderer feature can only draw GameObjects on the Outline layer.

2. The object is being drawn twice becuase there are two different zones: the one with the base texture and the one with the base texture multiplied with the DarkGraph being applied. 

3. All the lighting sections are added together in order to create the cel shaded effect. By adding the result of the shadowed aread with the result of the lit area, the final color creates this effect.

4. Changing the layer the Shiba is on enables or disables the outline effect because the stencil write pass has the layer mask set to Outline only. Thus, when the Shiba's layer is moved out of the Outline layer, it no longer draws the outline.

## W9

### Activity 1

The game Sekiro Shadows Die Twice uses many rendering techniques to create immersive effects. One effect that the game uses is a full-screen post processing effect to create a red, throbbing effect that obscures the screen when the player is at low HP. I can try to implement something similar by creating a full-screen red, throbbing effect when the player is at low HP during the boss fight or when the player is at low sanity in the store management mode. I can implement this using a texture for the red effect and a URP sample buffer within the shader graph.

### Activity 2
<img width="644" height="752" alt="Screenshot 2026-05-27 185033" src="https://github.com/user-attachments/assets/8cacca41-44b7-4d45-baac-6d630b3f93b3" />

One problem I solved today was setting up my shader graph so that it works on 2D sprites. Intiially, I was following along with the activity from last week (which was for 3D) and noticed that my shaders weren't working. I solved this issue by creating a shader graph for 2D sprites and setting up MainTex so that the shader material can be used on sprites.
