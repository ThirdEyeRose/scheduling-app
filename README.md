# Scheduling App [WIP]

An app which takes multiple schedules and calculates a possible schedule for maximum coverage, taking into consideration preferred working hours and weighted hours for coverage.

## Project Constraints

A manager should be able to input a schedule which needs coverage and assign weights to different parts of the day, indicating that more people are needed during one time of the week than another.

An employee should be able to choose which hours they prefer to work, which hours they can work, and which hours they absolutely cannot work. Preferred work hours should have more weight than hours they are simply available, schedules should not be created which include hours that an employee absolutely cannot work.

The app should natively account for different timezones and end-users should not have to translate their own timezone to UTC.

Each employee should be able to select whether or not they want to work 5 8-hour days, 4 10-hour days, or 3 12-hour days every week. An employee should be able to indicate that they would be open to one or more of these schedule strategies for scheduling flexibility.

Schedules should be scored as a whole and for each employee individually. Full schedules should be given bonus points for evenly weighting the schedule of each employee. Individual schedules should be scored based on preferred work hours, consecutive work days, and not working more than one weekend day per week.

## Tasks

The following tasks need to be completed to make this project a success. Each task will become an issue to flesh out the details and discuss implementation before becoming a pull request.

1. User Interface - Manager's scheduling screen: This screen should be a grid of days and times that a manager can assign a numeric value to in order to indicate how much coverage is needed for a specific time period. Numbers will be multiples and not the number of specific people needed to cover the schedule to allow for team expansion. Once the manager is finished editing the schedule, they should be able to hit a button indicating that they are finished.

2. User Interface - Employee's scheduling screen: This screen should be a grid of days and times where a user can indicate the times that they are available to work and when they prefer to work. Each hour will default to unavailable until a user chooses otherwise. An employee should also indicate whether they are available to work 5 8-hour days, 4 10-hour days, or 3 12-hour days or if they are open to multiple scheduling strategies. Once they have selected their preferences, they should be able to hit a button to signal that they have finished editing.

3. User Interface - Proposed working schedule: This screen will be a visual representation of who is working when. The manager should be able to accept the schedule, adjust the schedule, or re-roll the schedule entirely.

4. Controller - A controller needs to be created to tie the user interfaces into the database and the algorithm for building schedules.

5. Algorithm Design - An algorithm needs to be designed that can create random schedules and score them according to input from the manager and employees.
