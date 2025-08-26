# EXP-2 Welcome message in Message box with IF Condition and Switch case
## NAME : SANJITH.R
## REG.NO : 212223230191
## AIM :
to create a Welcome message in Message box with IF Condition and Switch case.

## PROCEDURE :
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

## WorkFlow:
<img width="1591" height="820" alt="Screenshot 2025-08-26 084507" src="https://github.com/user-attachments/assets/ac96e875-8ee2-4b24-96d8-6aa3885189f1" />
<img width="1589" height="830" alt="Screenshot 2025-08-26 084513" src="https://github.com/user-attachments/assets/6611a21d-593d-4275-923d-0916c05e1398" />

## Output:

## IF-ELSE:
<img width="1629" height="858" alt="image" src="https://github.com/user-attachments/assets/594f1e18-a28f-40ef-b027-3cd1920b62bd" />
<img width="1637" height="832" alt="Screenshot 2025-08-26 092709" src="https://github.com/user-attachments/assets/ccdab6bf-f197-4300-9b62-fb92ceb1869c" />

## SWITCH:
<img width="1598" height="820" alt="Screenshot 2025-08-26 084447" src="https://github.com/user-attachments/assets/68433c8d-8fe8-4d86-ac39-d586c09871ee" />
<img width="1594" height="831" alt="Screenshot 2025-08-26 084921" src="https://github.com/user-attachments/assets/6b85ce1d-e0b3-4183-866a-1652ebf68bbc" />

## RESULT:
Thus the process to display Welcome message in Message box with IF Condition and Switch case is created successfully.



