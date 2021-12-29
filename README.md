# Bonky (Conky widgets) for Ubuntu Budgie 21.10
Conky widgets for Ubuntu Budgie 21.10 x86_64.
![Preview image](https://raw.githubusercontent.com/lyan-pi/bonky-21.10/main/Screenshot%20from%202021-12-29%2019%3A55%3A38.png)

## Requirements
- conky (1.12.3_pre)

## How to install/use?

Unpack files from repository using:

    tar –xvzf bonky.tar.gz –C $HOME/
    sudo tar –xvzf bonky-configs.tar.gz –C /etc/.conky/

Load `conky` using `conky -c <config_path>`<br/>
Ta-dam! Widgets on the right side!<br/>

## How to configure?
Only one widget must be configured, that is weather widget.<br/>
Go to: `/home/<user name>/.conky/weather/` - in that folder, there are many bash scripts. You need to edit only one of them, that is `weather.sh`.<br/>
There are two variables: `API_KEY`, and `LOCATION_ID`.<br/>

**API_KEY** - which is reference to your account on openweathermap.org.<br/>
**LOCATION_ID** - your location ID on openweathermap.org.

## Additional notes.
Weather widget is coded in **polish-like** format. KM/H as wind speed, and celcius as temperature measurement unit.<br/>
Converting isn't necessary step to actually making this work. You don't have to convert those.<br/>
Just edit, `/etc/.conky/weather.conf`.<br/>

Same as time widget, but there is nothing much to change.<br/>
You could obviously change format of displayed time.<br/>
Using this: [strftime manual](https://www.php.net/manual/en/function.strftime.php)<br/>

Base for weather widget was copied from: [Stevica Stojković](https://github.com/sstojkovic/eleg-weather-conky)
