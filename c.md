# USWDS, Rails 6, Webpacker, Heroku

Quickly create a modern marketing website based upon the [U.S. Web Design System (USWDS)](https://designsystem.digital.gov/) using
Rails 6. Use webpacker to import and package USWDS javascript and CSS.  Deploy to Heroku.

## Get started

Create a new Rails 6 app with no database, no action mailbox, no active storage, no action cable. Have webpacker setup for StimulusJS even though we won't be using it (yet).
```bash
$ rails new landing-vaxcalc --skip-active-record --webpack=stimulus --skip-action-mailbox --skip-active-storage --skip-action-cable
```

Create a main controller with a few basic pages that you may want. Do not generate stylesheets.
```bash
$ rails g controller main landing features pricing about resources --no-stylesheets
```

