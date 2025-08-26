# EXP-2 Welcome message in Message box with IF Condition and Switch case
## NAME : SANJITH.R
## REG.NO : 212223230191
AIM :
to create a Welcome message in Message box with IF Condition and Switch case.

PROCEDURE :
IF Condition Robot (special for RAM)

IF:
if name = RAM → say Welcome Mr. Ramachandran

else → say Welcome

steps
open UiPath Studio → make new Process → open Main.xaml.

drag a Sequence.

create variable → userName (String).

drag Input Dialog:

Title: Enter Name

Label: Please type your name:

Result → userName

drag an If activity:
Condition → userName.ToUpper = "RAM"

inside Then → add Message Box:
Text → "Welcome Mr. Ramachandran"

inside Else → add Message Box:
Text → "Welcome " & userName

Run ▶ → try with RAM and with other names.
2) SWITCH Case Robot (different greeting for every name)
RAM → Welcome Mr. Ramachandran

SITA → Welcome Ms. Sita Devi

JOHN → Welcome Mr. John Carter

anything else → Welcome

steps
add variable userName (String).

drag Input Dialog →

Title: Enter Name

Label: Type your name:

Result → userName

drag a Switch activity:
TypeArgument → String

Expression → userName.ToUpper

Add Case "RAM" → Message Box:
"Welcome Mr. Ramachandran"

Add Case "SITA" → Message Box:
"Welcome Ms. Sita Devi"

Add Case "JOHN" → Message Box:
"Welcome Mr. John Carter"

Add Default → Message Box:
"Welcome " & userName

Run ▶ → type different names.
