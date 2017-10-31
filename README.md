# Scheduling App [WIP]

An app which takes multiple schedules and calculates a possible schedule for maximum coverage, taking into consideration preferred working hours and weighted hours for coverage.

## Project Constraints

A manager should be able to input a schedule which needs coverage and assign weights to different parts of the day, indicating that more people are needed during one time of the week than another.

An employee should be able to choose which hours they prefer to work, which hours they can work, and which hours they absolutely cannot work. Preferred work hours should have more weight than hours they are simply available, schedules should not be created which include hours that an employee absolutely cannot work.

The app should natively account for different timezones and end-users should not have to translate their own timezone to UTC.

Each employee should be able to select whether or not they want to work 5 8-hour days, 4 10-hour days, or 3 12-hour days every week. An employee should be able to indicate that they would be open to one or more of these schedule strategies for scheduling flexibility.

Schedules should be scored as a whole and for each employee individually. Full schedules should be given bonus points for evenly weighting the schedule of each employee. Individual schedules should be scored based on preferred work hours, consecutive work days, and not working more than one weekend day per week.
