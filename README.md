# Bonky (Conky widgets) for Ubuntu Budgie 21.10
Conky widgets for Ubuntu Budgie 21.10 x86_64.

## Requirements
- conky (1.12.3_pre)

## How to install/use?

Unpack files from repository using:
    tar –xvzf bonky.tar.gz –C $HOME/
    sudo tar –xvzf bonky-configs.tar.gz –C /etc/.conky/

Load `conky` using `conky -c <config_path>`
Ta-dam! Widgets on the right side!

## How to configure?
Only one widget must be configured, that is weather widget.
Go to: `/home/<user name>/.conky/weather/` - in that folder, there are many bash scripts. You need to edit only one of them, that is `weather.sh`.
There are two variables: `API_KEY`, and `LOCATION_ID`.

**API_KEY **- which is reference to your account on openweathermap.org.
**LOCATION_ID** - your location ID on openweathermap.org.

## Additional notes.
Weather widget is coded in **polish-like** format. KM/H as wind speed, and celcius as temperature measurement unit.
Converting isn't necessary step to actually making this work. You don't have to convert those.
Just edit, `/etc/.conky/weather.conf`.

Same as time widget, but there is nothing much to change.
You could obviously change format of displayed time.
Using this: [strftime manual]https://www.php.net/manual/en/function.strftime.php

Base for weather widget was copied from: [Stevica Stojković]https://github.com/sstojkovic/eleg-weather-conky
