# WorkingGame
A project to compute daily working hours and lucky draw as bonus for working. This project will be built in my spare time as part of my coding training:)

# Design (updating):
# This is written in pseudo code to demonstrate the design of this project
# Part 1. File List
Rules.csv: csv file, stores setting for the program.
History.log: text file, stores history of scores and tasks
Main.py: python main file

# Part 2. Workflow

# 2.1 Data import
# Read in history data
rawdata = read('History.log)

class Profile = HistoryParser(rawdata)

# Read in computing settings
rawdata = read('Constants.csv)# I do not want to use the csv module, for learning purpose

class sz_rules = DataParser(rawdata)# convert raw data spreadsheet into different fields of one structure

# 2.2 GUI Prep
# 1: history display (and some statastics)
# 2: task input and update
# 3: rule editor
# 4: backup and restore
# for part 2 and 3, there should be cancel and resume button effective for at least one step of change

# Specific function defining:
# 2.2.2 task input and update
# 1 Panels for data input
#   1 manual entry of task history
#   2 panel to import pomotodo xlsx file (from app pomotodo)
#       Specialized Data Parser Required
#   3 panel to import self-written text log of tasks
#       Specialized Data Parser Required
# 2 update the history based on input data and updating rules
Profile = DataUpdates(Profile,inputData,sz_rules)
