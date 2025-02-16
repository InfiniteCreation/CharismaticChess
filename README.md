# LeadersChess
*C#, sql-server, api*
## Table of Contents
* [Data Stored](#data-stored)
* [Data Source and Usage](#data-source-and-usage)
*  [User Stories](#user-stories)
*  [Use Cases](#use-cases)
*  [Table of Requirements](#table-of-requirements)
## Data Stored
There will be a lot of data stored, and each one will be used in different ways. The biggest part of
the data will come from the chess game itself. There will have to be data stored that distinguishes
both of the players. This will allow the game to know which player is making which move. This will
make it easier for the game mechanics to utilize other data as well.
The next piece of data that would need stored is if there is a time component or not and the exact
amount of time. This would allow for the game to have a timed component to the players turns.
Another piece of data that follows is a piece of data that tracks the decision of whether the game is
timed or not. Lastly a piece of data that tracks the time per game if it is decided the game is timed.
This will probably be the most amount of data that needs to be stored. The amount of possible
legal moves needs to be stored in data for each given position. This will easily be the largest
amount of data stored because theoretically there can be a maximum of 256 legal moves given the
right position.
## Data Source and Usage
The data that is stored will mostly be stored from API’s and the User Interface. The type of data that
will be taken from these sources will consist of things such as data storing which user is moving
currently, whether there is a time component to the game, the time if there is a time component,
the legal moves available for any position, the types of pieces, and the ways each piece can move.
This is just some of the stored data that will be retrieved from these two sources.
The data that is retrieved will be used in many ways. The data retrieved for the time component will
be used to slowly tick down the time each player has to play the game if a time component is used
in the game. The data retrieved regarding the possible legal moves will be used to determine what
moves the player can make and whether the move they choose to make is a legal move or not. This
will be used to allow each player to move their pieces in the game legally.
The data that is retrieved from the test to determine the player’s charisma will be the component
that gives this game of chess a twist. This component will be used to determine how loyal each
piece is to its king, and it will determine whether the king will be able to still do sacrifice plays in a
chess game where losing a piece is almost inevitable. For example, the player is given a rating of 9
for charisma. This will be used to determine each of the piece's loyalty ratings. The pieces with
higher points like the bishops, rooks, knights, and the queen will have higher loyalty ratings than
the pawns given their position as more important. This would be akin to the generals and
leadership in an army being more loyal compared to the foot soldiers. However, for the pawn, as it
gets closer to the other side its loyalty rating will increase because of its proximity to the finish line
for promotion. If the loyalty is below a certain rating, then sacrifice plays with that piece will not be
an option and removed from possible legal moves.
## User Stories
### First
- As a player
- I want something to spice up the traditional game of chess
- So that I can enjoy playing a game of chess with a fresh twist
### Second
- As a candidate screener
- I want something that can demonstrate a persons critical thinking and their ability to lead
- So that I can successfully screen the applicants and find the best ones for the role
### Third
- As a military instructor
- I want something that can test a soldiers critical thinking, their ability to lead, and their ability to function in dire straits
- So that I can determine what further training they need and where best to place them
### Fourth
- As a player
- I want something that is more realistic in regards to war
- So that I can experience playing a game of chess realistically how it would play out in a battlefield
### Fifth
- As a military instructor
- I want something that can test how a soldier is progressing with their training in being able to function in dire staits and lead under pressure
- So that I can further train and help my men grow
## Use Cases
### First
- Military Instructor Initial Inspection
- The soldiers will play a game of Leaders Chess
- This will be part of their initial examination
- During the game how they operate under dire straits and how they lead in such circumstances will be noted
- The results will be used to determine the best training and initial position
### Second
- Military Instructor Training and Assessment
- The soldiers will play a game of Leaders Chess
- This will be part of a reexamination to assess growth
- During the game how they operate under dire straits and how they lead in such circumstances will be reassessed
- The results will be used to determine how their training is progressing and what might need to be changed for further training
### Third
- Candidate Screener for Leadership position
- The candidates will play a game of Leaders Chess
- This will be part of their screening process
- During the game how they strategize and lead will be assessed in relation to the charisma score they get after assessment for the game
- The results will be used to screen the candidates and determine which ones are more suitable for a leadership position
### Fourth
- Player seeking an adeventurous twist
- The players will play a game of Leaders Chess
- This will give them something new and adventurous to play
- During the game they will have fun playing the game of chess with the added elements
- The results will be a player that will have fun playing a new thrilling game that takes strategy to a new level
### Fifth
- Player seeking to play something more realistic
- The players will play a game of Leaders Chess
- This will give them a more realistic simulated battle between kings (players)
- During the game they will be able to experience how it is to lead their pieces in a more realistic battle with their openents
- The result will be a more realistic battle of chess that is more realistic to how it would be in war
## Table of Requirements
ID | Requirements
:---:|:---:
1 | The software shall allow the user to interact with a UI that controls the movement of the chess pieces. The view will display the chess pieces of both players as well as the timer for both players if applicable.
2 | The software shall allow the user to interact with a UI to select whether they want a timer for their game or not. The view will display a menu with buttons that the user can interact with to make their choice.
3 | The software shall allow the user to interact with a UI to complete a questionnaire that will determine the charisma level of the player. The view will consist of text and some form of selection option like a radio button or a checklist.
4 | The software shall allow the user to see the possible moves of a piece upon clicking on it. The view will display the chess pieces of both players, the timer for both players if applicable, and the highlighted squares on the board that show the possible moves for the piece clicked.
5 | The software shall flash a notification when the user tries to make a sacrifice play but they can't because their charisma level is too low. The view shall contain a dimmed view of the game in the background with a big notification in the foreground that will tell the user to click to continue.
