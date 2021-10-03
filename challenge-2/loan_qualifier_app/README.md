**# Project Title **
** Qualifying Loans Application **
This project creates a command line application that searches a qualifying loan based on the applicant's financial profile
---

**## Technologies**

The project is written in python and uses CLI libraries (fire and questionary), and csv library to read and write csv data.
---

**## Installation Guide **

To install the program, download the git repo.

---

**## Usage **

To run change directory to the loan_qualifier_app folder, and execute "python app.py"

Sample Runs

No Qualifing Loan Example
% python app.py                     
? Enter a file path to a rate-sheet (.csv): data/daily_rate_sheet.csv
? What's your credit score? 700
? What's your current amount of monthly debt? 5000
? What's your total monthly income? 6000
? What's your desired loan amount? 50000
? What's your home value? 150000
The monthly debt to income ratio is 0.83
The loan to value ratio is 0.33.
Found 0 qualifying loans
Exit!

Qualifing Loan but the user opts to not save the file
% python app.py
? Enter a file path to a rate-sheet (.csv): data/daily_rate_sheet.csv
? What's your credit score? 700
? What's your current amount of monthly debt? 3000
? What's your total monthly income? 12000
? What's your desired loan amount? 50000
? What's your home value? 500000
The monthly debt to income ratio is 0.25
The loan to value ratio is 0.10.
Found 11 qualifying loans
? Do you want to save the qualifying loans?(Y/N): n
Exit!



Qualifing Loan and the user opts to save the file
% python app.py
? Enter a file path to a rate-sheet (.csv): data/daily_rate_sheet.csv
? What's your credit score? 700
? What's your current amount of monthly debt? 3000
? What's your total monthly income? 12000
? What's your desired loan amount? 50000
? What's your home value? 550000
The monthly debt to income ratio is 0.25
The loan to value ratio is 0.09.
Found 11 qualifying loans
? Do you want to save the qualifying loans?(Y/N): Y
? Enter a file path to save qualifying loans (.csv): data/qualifing_loans.csv

Sample qualifing loan data file
% cat data/qualifing_loans.csv
Lender,Max Loan Amount,Max LTV,Max DTI,Min Credit Score,Interest Rate
Bank of Big - Starter Plus,300000,0.85,0.39,700,4.35
West Central Credit Union - Starter Plus,300000,0.8,0.44,650,3.9
FHA Fredie Mac - Starter Plus,300000,0.85,0.45,550,4.35
FHA Fannie Mae - Starter Plus,200000,0.9,0.37,630,4.2
General MBS Partners - Starter Plus,300000,0.85,0.36,670,4.05
Bank of Fintech - Starter Plus,100000,0.85,0.47,610,4.5
iBank - Starter Plus,300000,0.9,0.4,620,3.9
Goldman MBS - Starter Plus,100000,0.8,0.43,600,4.35
Prosper MBS - Starter Plus,100000,0.9,0.38,640,3.75
Developers Credit Union - Starter Plus,200000,0.85,0.46,640,4.2
Bank of Stodge & Stiff - Starter Plus,100000,0.8,0.35,680,4.35
% 

---

**## Contributors **

Author: Sumeet Vaidya
Contributors: BootCamp for providing the base code.
---

**## License **

When you share a project on a repository, especially a public one, it's important to choose the right license to specify what others can and can't with your source code and files. Use this section to include the license you want to use.
