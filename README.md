# GoPolyCal
A first attempt to use Google Calendar from Polybar utilizing the API.

***Please note this is _not_ usable in its current state. It is a proof of concept and study repository.***

## Requirements

- polybar
  ```
  baph -i polybar
  pacman -S polybar
  ```

- gem: google-api-client
  ```
  gem install google-api-client
  ```


## Install

```
git clone http://github.com/moonwitch/gopolycal.git
```


## Setup

### Obtain a Client ID and Secret

  1. Go to the Google Developers Console.
  2. Select a project, or create a new one (at the top of the page).
  3. In the sidebar on the left, select Library.
  4. Type in 'Google Calendar' in the search box and click on 'Google Calendar API' in the results.
  5. Click on the 'Enable' link at the top of the page.
  6. In the sidebar on the left, select Credentials.
  7. If you haven't done so already, create your 'OAuth client ID' by clicking Create Credentials'.

  Note: you need to set your 'Product name show to users' on the OAuth consent screen before you can create your client ID.

  8. Select the 'Other' option and click create.

  _Take note of the Client ID and Client Secret as you'll need to add it to your code later._

### Find your calendar ID

  1. Visit Google Calendar in your web browser.
  2. In the calendar list on the left, click the down-arrow button next to the appropriate calendar, then select Calendar settings.
  3. In the Calendar Address section, locate the Calendar ID listed next to the XML, ICAL and HTML buttons.
  4. Copy the Calendar ID.
