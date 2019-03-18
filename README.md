# grain_reports

These scripts pull the jogr112 report text and parse the data. They are to be run daily as windows task scheduled / chron jobs at ~8:00am and ~11:30am respectively

jogr112_close is to be run in the morning and will parse the report from the day before
jogr112_intra is to be run ~ 11:30 and will parse the 11:30 report data

jogr112_combine will evaluate the difference between the both parts (seperated by "to") of the Basis and change data between the 
morning (jogr112_close) and the afternoon (jogr112_intra) data pulls. 

Scripts created with: 
Python    3.6.7
requests  2.21.0
pandas    0.24.1
