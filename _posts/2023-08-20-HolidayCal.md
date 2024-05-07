---
layout: post
title: Subscribe to Holiday Calendars
---

Apple and Google's holiday calendar feed.

## Apple's

Apple don't provide a way to manually subscribe to the holiday calendars you want, they just automatically add a holiday calendar according to region and display language in Settings, but you can still do so by directly subscribing to the iCloud URL. Those URL look like below:

`https://calendars.icloud.com/holidays/${YourChoice}.ics`

Just replace `${YourChoice}` with `RegionCode_LanguageCode`, such as US holiday in English > `us_en` > `https://calendars.icloud.com/holidays/us_en.ics`. Please note that not all of the combination is available, and none SSL waring will show up in those cases.

Region Code is as defined in ISO 3166–1 alpha-2, and Language Code is as defined in ISO 639–2.

## Google's

You can easily subscribe to Google's holiday calendar in Google Calendar service under interest calendars. If you want to use these calendars outside of Google, the simplest way is to subscribe to the desired calendar, navigate to settings for other calendars, then at the bottom of the subscribed calendar you can find the public address in iCal format, copy this URL and paste it to any calendar service you want. But if you don't want a google account, it becomes more complex.

All of Google's public calendar URL look like  
`https://calendar.google.com/calendar/ical/${CalendarID}/public/basic.ics`

The holiday calendars' ID look like `LanguageCode.RegionName(.official)%23holiday%40group.v.calendar.google.com`, Language Code is the same as ISO, and the optional `.official` indicates only official holidays from government will be included.

The Region Name is a little confusing, as they don't have any law. Here's some: `german`, `japanese`, `south_korea`, `taiwan`, `usa`.

There're also some religious calendars available from Google, just change RegionName to `christian`, `hinduism`, `judaism`, `islamic`, `orthodox_christianity`.
