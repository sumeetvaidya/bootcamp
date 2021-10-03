# Project Title : Qualifying Loans Application <br/>
This project creates a command line application that searches a qualifying loan based on the applicant's financial profile
<br/>


## Technologies <br/>

The project is written in python and uses CLI libraries (fire and questionary), and csv library to read and write csv data.
<br/>

## Installation Guide  <br/>

To install the program, download the git repo.

<br/>

## Usage  <br/>

To run change directory to the loan_qualifier_app folder, and execute "python app.py" <br/>

### Sample Run <br/>

#### No Qualifing Loan Example <br/>

% python app.py<br/>
? Enter a file path to a rate-sheet (.csv): data/daily_rate_sheet.csv<br/>
? What's your credit score? 700<br/>
? What's your current amount of monthly debt? 5000<br/>
? What's your total monthly income? 6000<br/>
? What's your desired loan amount? 50000<br/>`
? What's your home value? 150000 <br/>
The monthly debt to income ratio is 0.83<br/>
The loan to value ratio is 0.33.<br/>
Found 0 qualifying loans<br/>
Exit!<br/>
<br/>


#### Qualifing Loan but the user opts to not save the file<br/>
% python app.py<br/>
? Enter a file path to a rate-sheet (.csv): data/daily_rate_sheet.csv<br/>
? What's your credit score? 700<br/>
? What's your current amount of monthly debt? 3000<br/>
? What's your total monthly income? 12000<br/>
? What's your desired loan amount? 50000<br/>
? What's your home value? 500000<br/>
The monthly debt to income ratio is 0.25<br/>
The loan to value ratio is 0.10.<br/>
Found 11 qualifying loans<br/>
? Do you want to save the qualifying loans?(Y/N): n<br/>
Exit!<br/>
<br/>


#### Qualifing Loan and the user opts to save the file<br/>
% python app.py<br/>
? Enter a file path to a rate-sheet (.csv): data/daily_rate_sheet.csv<br/>
? What's your credit score? 700<br/>
? What's your current amount of monthly debt? 3000<br/>
? What's your total monthly income? 12000<br/>
? What's your desired loan amount? 50000<br/>
? What's your home value? 550000<br/>
The monthly debt to income ratio is 0.25<br/>
The loan to value ratio is 0.09.<br/>
Found 11 qualifying loans<br/>
? Do you want to save the qualifying loans?(Y/N): Y<br/>
? Enter a file path to save qualifying loans (.csv): data/qualifying_loans.csv<br/>
<br/>
#### Sample qualifing loan data file<br/>
% cat data/qualifying_loans.csv<br/>
Lender,Max Loan Amount,Max LTV,Max DTI,Min Credit Score,Interest Rate<br/>
Bank of Big - Starter Plus,300000,0.85,0.39,700,4.35<br/>
West Central Credit Union - Starter Plus,300000,0.8,0.44,650,3.9<br/>
FHA Fredie Mac - Starter Plus,300000,0.85,0.45,550,4.35<br/>
FHA Fannie Mae - Starter Plus,200000,0.9,0.37,630,4.2<br/>
General MBS Partners - Starter Plus,300000,0.85,0.36,670,4.05<br/>
Bank of Fintech - Starter Plus,100000,0.85,0.47,610,4.5<br/>
iBank - Starter Plus,300000,0.9,0.4,620,3.9<br/>
Goldman MBS - Starter Plus,100000,0.8,0.43,600,4.35<br/>
Prosper MBS - Starter Plus,100000,0.9,0.38,640,3.75<br/>
Developers Credit Union - Starter Plus,200000,0.85,0.46,640,4.2<br/>
Bank of Stodge & Stiff - Starter Plus,100000,0.8,0.35,680,4.35<br/>
% <br/>


## Contributors <br/>

__Author: Sumeet Vaidya__<br/>
__Contributors: BootCamp for providing the base code.__<br/>
---

## License <br/>
The code is licensed using Educational Community License v2.0
