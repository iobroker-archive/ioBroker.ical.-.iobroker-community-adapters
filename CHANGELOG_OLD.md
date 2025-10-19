# Older changes
## 1.15.0 (2024-04-30)
* (mcm1957) Adapter requires node.js >= 18 and js-controller >= 5 now
* (mcm1957) Dependencies have been updated

## 1.14.3 (2024-02-28)
* (jens-maus) update node-ical to latest 0.18.0

## 1.14.2 (2024-01-29)
* (jens-maus) update node-ical to latest 0.17.2

## 1.14.1 (2024-01-29)
* (klein0r) Create dummy file in files tab
* (klein0r) Fixed recurring events

## 1.14.0 (2024-01-07)
* (klein0r) Allow to set custom http user agent
* (klein0r) Added option to use files tab for calendar files

## 1.13.6 (2023-12-25)
* (mcm1957) Incorrect jsonConfig has been fixed [#602]
* (mcm1957) Dependencies have been updated

## 1.13.5 (2023-12-15)
* (jens-maus) updated node-ical to latest 0.17.1

## 1.13.4 (2023-12-10)
* (jens-maus) updated node-ical to latest 0.17.0
* (jens-maus) updated dependencies

## 1.13.3 (2023-06-20)
* (jens-maus) updated node-ical to latest 0.16.1
* (klein0r) Use color picker in adapter settings
* (klein0r) Dropped Admin 4 UI
* (klein0r) Added Ukrainian language

## 1.13.2 (2022-08-29)
* (Apollon77) fix strange log messages by downgrading RRule again

## 1.13.1 (2022-06-27)
* (klein0r) Changed request library

## 1.13.0 (2022-06-17)
* (klein0r) Added Admin 5 UI
* (klein0r) Translated all object names

## 1.12.2 (2022-06-03)
* (Apollon77) Fix displaying rest-time of event in one case

## 1.12.1 (2022-03-22)
* (Apollon77) Adjust colorize of dates to also show dates started in the past with today's color

## 1.12.0 (2022-03-21)
* (Apollon77/Scrounger) Add option to choose the ack flag set when updating foreign objects on events
* (HSE83) use a color field from the calendar entry as color for display
* (Apollon77) When no Arrow for already running events is shown and dates are not replaced with words display the start date in the list and not the end date
* (Apollon77) When not replacing date with words and entry ends at 0:0:0 show the day before as end
* (Apollon77) Fix issues when no end date is provided in the calendar entry (start and end are the same)
* (Apollon77) Correctly calculate length of multi day events
* (Apollon77) Respect DST changes in some calculations to prevent strange effects
* (Apollon77) Parse ics Files with different line endings again

## 1.11.6 (2021-12-17)
* (jens-maus) fixed incorrect recurrence event processing

## 1.11.5 (2021-11-09)
* (jens-maus) updated node-ical to latest 0.14.1
* (jens-maus) fix another issue where an already ended event is still listed

## 1.11.4 (2021-09-02)
* (Apollon77) fix cases where already ended entries where still listed
* (Apollon77) fix reported sentry crash cases (IOBROKER-ICAL-S, IOBROKER-ICAL-N)

## 1.11.3 (2021-08-04)
* (jens-maus) fixed timezone related handling

## 1.11.2 (2021-08-01)
* (Apollon77) Change one logline to debug

## 1.11.1 (2021-07-30)
* (Apollon77) Adjust date length for full day events to the full day

## 1.11.0 (2021-07-30)
* (Apollon77) Locally cache remote calendars to be used in case of request errors

## 1.10.4 (2021-07-30)
* (Apollon77) Make sure daysPast is correctly initialized if not provided
* (Apollon77) When no calendar could be read then no events are updated/cleanup
* (Apollon77) Respect HTTP statuscode from server response too to detect errors

## 1.10.3 (2021-07-30)
* (Apollon77/Feuersturm) Fix other timezone issues
* (Apollon77) Fix setting external States when events are active
* (Apollon77) Also list recurring entries from the past
* (Apollon77) Fix the event states for the days in future

## 1.10.2 (2021-07-25)
* (Apollon77/Feuersturm) Fix wrong times and dates introduced in 1.7.5.
* (Feuersturm) Allow Setting daysPast to be decreased to zero with button again

## 1.10.1 (2021-07-22)
* (Apollon77) Make sure all Event objects are created before values are written

## 1.10.0 (2021-07-16)
* IMPORTANT: data.table is now a stringified array!! Consider when using this value!
* (Apollon77) Optimize for js-controller 3.3
* (BasGo) added analysis for events marked as private in Google Calendar
* (jens-maus) updated dependencies

## 1.9.3 (2021-04-01)
* (Apollon77) Better handling of some ical cases

## 1.9.2 (2021-03-07)
* (Apollon77) Prevent crash case when summary is not provided (Sentry IOBROKER-ICAL-K)

## 1.9.1 (2021-01-30)
* (Apollon77) try to make sure all code is executed before adapter is ended

## 1.9.0 (2021-01-12)
* (christofkac) Added option to ignore case when events are searched in calendars
* (Apollon77) Prevent crash case (Sentry IOBROKER-ICAL-F)

## 1.8.5 (2021-01-01)
* (Apollon77) update ical library to prevent problems with RRULE parsing

## 1.8.4 (2020-12-27)
* (Apollon77) Prevent crash case (Sentry IOBROKER-ICAL-D)

## 1.8.3 (2020-12-24)
* (Apollon77) Prevent crash case (Sentry IOBROKER-ICAL-C)
* (Apollon77) Upgrade node-ical

## 1.8.2 (2020-11-29)
* (klein0r) Several fixes and optimizations

## 1.8.1 (2020-11-20)
* (klein0r) Fixed past event calculation in html view

## 1.8.0 (2020-11-14)
* (klein0r) Moved html options to separate tab
* (klein0r) Added option to hide "arrow" on for running events
* (klein0r) Added feature to include past events (in days)

## 1.7.5 (2020-11-08)
* (Apollon77) Only handle events with a start date (Sentry IOBROKER-ICAL-1, IOBROKER-ICAL-2, IOBROKER-ICAL-4)
* (jens-maus) Update dependencies, fix some more issues

## 1.7.4 (2020-08-26)
* (Apollon77) Fix multiple parsing

## 1.7.3 (2020-08-26)
* (foxriver76) we pin a specific dependency version, because "rrule" package broken
* (foxriver76) added eslint

## 1.7.2 (2019-12-02)
* (bluefox) Documentation was changed

## 1.7.1 (2019-01-08)
* (twonky4) Fixed issue with UTC of until in recurring appointments
* (twonky4) Fixed possible empty color

## 1.7.0 (2018-11-27)
* (twonky4) Add filter option
* (twonky4) Add support of events for configured date period; changed state names from `events.*` to `events.0.today.*`
* (twonky4) Add Count of events for tomorrow - state `data.countTomorrow`
* (twonky4) Events without time part and same start and end are interpreted as full day events
* (twonky4) Remove special chars from event states

## 1.6.6 (2018-10-22)
* (twonky4) Fixed html for disabled colorize
* (twonky4) Fixed timezone handling for events during change from daylight saving time back to standard time
* (twonky4) Fixed events without end date moved to different day

## 1.6.5 (2018-10-13)
* (twonky4) Simplify timezone solution
* (twonky4) Fix calendars without timezones

## 1.6.4 (2018-10-12)
* (twonky4) Support windows timezones
* (twonky4) Don't fail on invalid timezones

## 1.6.3 (2018-10-10)
* (twonky4) Fixes timezone issue in fullday recurring appointments

## 1.6.2 (2018-10-08)
* (twonky4) Fixes timezone issue in recurring appointments

## 1.6.1 (2018-06-04)
* (Apollon77) Several fixes and optimizations

## 1.6.0 (2018-04-13)
* (Apollon77) Several fixes and optimizations
* (Apollon77) Upgrade node-ical library to allow big files to work
* (Apollon77) Better handling of full day events
* (Apollon77) Allow "Replace 0:00" to have 30 characters

## 1.5.3 (2018-03-24)
* (Apollon77) Also make location available in data table

## 1.5.2 (2018-03-23)
* (Apollon77/BuZZy1337) Fix several display issues

## 1.5.0 (2018-03-07)
* (bluefox) ready for Admin3

## 1.4.2 (2018-02-21)
* (Apollon77) Also display events that started before today

## 1.4.1 (2018-02-05)
* (Apollon77) also allow events without end parameter and assume an 0minute event then and set end = start

## 1.4.0 (2018-01-01)
* (Apollon77) allow multiple Events to be contained in one calendar entry. Make sure the names are unique enough because the search only checks for existance of the event name in the text.
* (Apollon77) correctly detect events that started before 0:00
* (Apollon77) also show events with no duration (sometimes used as reminders)
* (Apollon77) correctly show end times for events that are longer then 1 day (including "+x" to show day duration)
* (Apollon77) many enhancements and optimizations in formatting the infos (especially when event has already started but not ended)
* (Apollon77) add option to hide year numbers
* (Apollon77) add own CSS classes to each entry with the names iCal-<calendername> and iCal-<calendername>2 to be able to really design it as needed
* (Apollon77) Known issue: For recurring events it works to delete single events, but it do not work to move them

## 1.3.3 (2017-10-30)
* (DutchmanNL) Translate to Netherlands

## 1.3.2 (2017-02-24)
* (jens-maus) added singular form for 'days'

## 1.3.1 (2017-02-20)
* (jens-maus) implemented support for date excludes for recurring events

## 1.3.0 (2017-02-17)
* (jens-maus) switched ical module to use 'node-ical' which should improve ics format compatibility

## 1.2.2 (2017-02-17)
* (jens-maus) added changes to show "Noch X Tage" for fullday events (e.g. school holidays)

## 1.2.1 (2017-02-11)
* (jens-maus) applied workaround of ics files with TZID before DATE in DTSTART/DTEND

## 1.2.0 (2016-07-23)
* (bluefox) allow read from files
* (bluefox) add tests
* (bluefox) fix all day indication

## 1.1.3 (2016-07-19)
* (bluefox) fix error if entry is invalid
* (bluefox) use newer ical packet version

## 1.1.2 (2015-06-30)
* (jens-maus) implemented some more text replacement terms
* (jens-maus) we only colorize the date+time for imminent appointments
* (jens-maus) added cloneextend dependency definition and fix for dayafter mods
* (jens-maus) ported the "dayafter" change of the ccu.io ical adapter to the iobroker

## 1.1.1 (2015-08-16)
* (bluefox) enable auth only if user set.

## 1.1.0 (2015-08-13)
* (elmars) Added ability to provide username/password to authenticate against protected ics files. Tested with owncloud.

## 1.0.2 (2015-07-21)
* (bluefox) fix error if ICS file has empty lines

## 1.0.1 (2015-07-21)
* (bluefox) change readme title

## 1.0.0 (2015-07-21)
* (bluefox) fix error with set event to false

## 0.1.1 (2015-06-14)
* (bluefox) add additional fields for ioBroker.occ

## 0.1.0 (2015-03-24)
* (bluefox) make it compatible with new concept

## 0.0.2 (2015-02-22)
* (bluefox) fix error with configuration
* (bluefox) fix error with event object creation

## 0.0.1 (2015-02-17)
* (bluefox) initial commit
