# LeadersChess
*C#, sql-server, api*
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
