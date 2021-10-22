# Software-design-document
created for the client, The Gaming Room

 The Gaming Room wants to develop a web-based game that serves multiple platforms based on their current game, Draw It of Lose It, which is currently available in an Android app only. The game is similar to the 1980s television game Win, Lose or Draw, where teams compete to guess what is being drawn. The game application will render images from a library of stock drawings as clues. The time limit for this game is 15-seconds, and if the player does not answer, the chance is passed to the opposing team. 

 The client has requested the software requirements above. We will apply the above requirements requested by our customers to our codes. In addition to this requirement, the client wants the game to be able to run on multiple platforms just as it currently runs on Android. In order to accomplish desired result, we can reuse the code that is already running on Android in java that works across multiple platforms.
 
 The diagram consists of a total of 7 classes. The Entity that is a superclass has three child classes: Game, Team, and Player. You can see that the state variables and constructor of the entity class are set to private to prevent direct changes. The rest of the getters are set to public for the use in the child classes. 
 Child classes are related to each other and can form zero to multiple relationships with each other. We can see this association by looking at the links and a number to each other.  And this is one of the constraints requested by the client. The other constraints can be achieved by using the GameService class associated with the Game. As you can see in the attributes of the GameService class, all their attributes are set to static. This allows us to make only one instance of the game can exist in memory at any given time.  Also, program driver class and singletonTester Driver exist to allow us to test programs according to customer requirements. 

