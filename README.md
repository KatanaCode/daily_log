# DailyLog

Provides a simple framework for keeping a daily log of the work you do on a project

## Usage

Call the binary `daily_log` to open today's log.

Pass in the option `--help` to see the other options available.

## Installation

``` bash
cd /usr/local
git clone https://github.com/KatanaCode/daily_log.git
alias /usr/local/bin/daily_log /usr/local/daily_log/bin/daily_log
```

## Example

At the end of a working day, you run from your console

$ daily_log

This opens a text file in your editor that looks like this:

``` text
# Daily Entry - Wed 01 January, 2020

## Today I worked on:

- Thing one

## Next time, you should continue with:

- Thing two

## Notes:

Some optional notes here...

<!--
  Automatically generated by DailyLog https://github.com/KatanaCode/daily_log
  Date: 2020-01-01
  Project: dailylog
  By: Yourname
-->
```

You edit the file to say:

``` text
# Daily Entry - Wed 01 January, 2020

## Today I worked on:

- Adding two-factor authentication for admins

## Next time, you should continue with:

- Password management for admins

## Notes:

We need to rethink how we handle password resets when user has 2FA enabled

<!--
  Automatically generated by DailyLog https://github.com/KatanaCode/daily_log
  Date: 2020-01-01
  Project: dailylog
  By: Yourname
-->
```

### A few days later

Some time has passed since you last worked on the project. You aren't quite sure where to pick up from the last time you worked on it.

You type:

```
$ daily_log -l # short for daily_log --last
```

...to print out your log to the console.

## Why bother?

Managing a log file like this can help you keep your train of thought when interrupted on a project for a few days or longer.

This is a simple, non-invasive way to leave notes to your future self.

It's also a great way to take full stock of a project once it's complete. Were your time estimates as accurate as you thought they would be?
