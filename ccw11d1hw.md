Episode 1 :
My expected result:
The murderer is Miss Scarlet

Reason:
Because when the const verdict is called it will call the const declareMurderer which will look into the const scenario and extract the value of they key 'murderer', which is Miss Scarlet.

Actual result: "The murderer is Miss Scarlet"

------------------------------------------------

Episode 2:
My expected result:
The murderer is Professor Plum

Reason:
Because murderer is defined as a const, it is unchangeable, so the changeMurderer function will not alter it.

Actual result: error on trying to change a const

-------------------------------------------------

Episode 3:
My expected result:
First verdict: The murderer is Mrs. Peacock
Second verdict: The murderer is Mrs. Peacock

Reason:
Because murderer is defined as a let, the declareMurderer function will change the value to "Mrs. Peacock", on the second verdict, although declareMurderer is not run again the value of murderer has already been changed so it will give the result of Mrs. Peacock again.

Actual result:
First Verdict:  The murderer is Mrs. Peacock.
Second Verdict:  The murderer is Professor Plum.

--------------------------------------------------

Episode 4:
My expected result:
The suspects are Miss Scarlet, Professor Plum, Colonel Mustard
Suspect three is Mrs Peacock

Reason:
Because all three suspects are defined as let, they are changeable, the declareAllSuspects will change third suspect to Colonel Mustard.

The final line is printing out the suspects without calling the function that changes the third one so it should be Mrs. Peacock

Actual result:
The suspects are Miss Scarlet, Professor Plum, Colonel Mustard.
Suspect three is Mrs. Peacock.


--------------------------------------------------

Episode 4:
My expected result:
The suspects are Miss Scarlet, Professor Plum, Colonel Mustard
Suspect three is Mrs Peacock

Reason:
Because all three suspects are defined as let, they are changeable, the declareAllSuspects will change third suspect to Colonel Mustard.

The final line is printing out the suspects without calling the function that changes the third one so it should be Mrs. Peacock

Actual result:
The suspects are Miss Scarlet, Professor Plum, Colonel Mustard.
Suspect three is Mrs. Peacock.


--------------------------------------------------

Episode 5:
My expected result:
The weapon is the Candle Stick

Reason:
scenario is defined as a const so cannot be changed.

Actual result:
The weapon is the Revolver.


--------------------------------------------------

Episode 6:
My expected result:
The murderer is Mrs. White

Reason:
murderer is defined as a let so it can be changed, the changeMurderer function changes it to Mr Green and then calls the plotTwist function which changes it to Mrs White.

changeMurderer is called and then the murderer is declared so Mrs White is my expected output

Actual result:
The murderer is Mrs. White.



--------------------------------------------------

Episode 7:
My expected result:
The murderer is Colonel Mustard

Reason:
murderer is initially defined as a let, as Professor Plum, the changeMurderer function changes it to Mr Green, then defines plotTwist (which when called will change to Colonel Mustard), then defines unexpectedOutcome (which when called changes the murderer to Miss Scarlet), THEN it calls unexpectedOutcome but ends wit calling plotTwist which I think will result in the final outcome of Colonel Mustard

Actual result:
The murderer is Mr. Green.


--------------------------------------------------

Episode 8:
My expected result:
The weapon is Candle Stick

Reason:
scenario is initially defined as having Mrs. Peacock as the murderer and the Conservatory as the room. The changeScenario function (which is called before the verdict is printed in log) changes the room to the dining room, and has a plotTwist function inside it that when the room is a certain room the murderer changes to Colonel Mustard and there is an unexpectedOutcome function which changes the weapon to the Candle Stick, plotTwist is called on the Dining Room, thus invoking the unexpectedOutcome and changing the weapon to Candle Stick



Actual result:
The weapon is Candle Stick.

--------------------------------------------------

Episode 9:
My expected result:
The murderer is Professor Plum

Reason:
murderer is defined as a let so it can be changed and is set to Professor Plum, the conditional statement states that if the murderer is Professor Plum it will define a new let called murderer as Mrs. Peacock but it's not the same as the original one, when the verdict is called it declares the original murderer, Professor Plum

Actual result:
The murderer is Professor Plum.
