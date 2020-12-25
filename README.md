# Reconsile-app
OHIP Billing reconciliation app

This R Shiny applicaiton was developed to automate billing reconsilation calculations and generate reports.
It takes OHIP "Ontario Health Insurance Plan" Remmitance advice files and Hype Med csv reports "for private billing and location tags" and generates a report that inculdes monthly payments per Doctor and some aggregated data for analtical porposes.
Creating those reports was done manually using Excel before this app was developed. It was a time consuming task that was prone to human error.
This app "with some modifications" can be used by most private medical professionals in Ontario, Canada. 

It contains 9 different files. A Windows batch file to run the app from windows desktop, a UI.r file that contains the front-end, a Server.R that directs the data to teh appropriet Rmd file for cleaning, calculations and gereting a pdf reprts. There are 4 Rmd files, 1 for each practioner. One of the practioners bills for 3 different locations, 2 of which are Hopitals, there is a seperate Rmd files that generates a report for hospital billing. In addition to that, there is an Run.r file that locates the app folder and connects the front  to the back end. 
