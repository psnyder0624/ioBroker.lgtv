![Logo](admin/lgtv.png)
# ioBroker.lgtv
=================

[![NPM version](http://img.shields.io/npm/v/iobroker.lgtv.svg)](https://www.npmjs.com/package/iobroker.lgtv)
[![Downloads](https://img.shields.io/npm/dm/iobroker.lgtv.svg)](https://www.npmjs.com/package/iobroker.lgtv)

[![NPM](https://nodei.co/npm/iobroker.lgtv.png?downloads=true)](https://nodei.co/npm/iobroker.lgtv/)


#LG WebOS SmartTV adapter for ioBroker

Remote controlling an LG WebOS SmartTV (2013 models and higher) from [ioBroker](https://www.iobroker.net).


---




## Some examples:
```setState('lgtv.0.popup', 'Some text!');```

This will show a popup with the text "Some text!" on the TV.
You can use HTML linebreaks (br) in the text.


```setState('lgtv.0.turnOff', true);```

Switching off the TV.


```setState('lgtv.0.mute', true);```

Mute the TV.

```setState('lgtv.0.mute', false);```

Unmute the TV.


```setState('lgtv.0.volumeUp', true);```

This will increase the volume of the TV.

```setState('lgtv.0.volumeDown', true);```

Decreasing the volume of the TV.


```setState('lgtv.0.3Dmode', true);```

Activates the 3D mode on the TV

```setState('lgtv.0.3Dmode', false);```

Deactivates the 3D mode on the TV.


```setState('lgtv.0.channel', '7');```
```setState('lgtv.0.channel', 7);```

Switching the live TV to channel number 7.


```setState('lgtv.0.launch', 'livetv');```

Switching to Live TV mode.

```setState('lgtv.0.launch', 'smartshare');```

Opening the SmartShare App on the TV.

```setState('lgtv.0.launch', 'tvuserguide');```

Runs the TV User Guide App on the TV.

```setState('lgtv.0.launch', 'netflix');```

Opening the Netflix App on the TV.

```setState('lgtv.0.launch', 'youtube');```

Opens the Youtube App on the TV.

```setState('lgtv.0.launch', 'prime');```

Opens the Amazon Prime App on the TV.

```setState('lgtv.0.launch', 'http://www.iobroker.net');```

Opens the Webbrowser on the TV and navigates to www.iobroker.net.

```setState('lgtv.0.input', 'AV_1');```

Switches the iput oh the TV to AV1.

```setState('lgtv.0.input', 'SCART_1');```

Switches the iput oh the TV to Scart.

```setState('lgtv.0.input', 'COMP_1');```

Switches the iput oh the TV to Component.

```setState('lgtv.0.input', 'HDMI_1');```

Switches the iput oh the TV to HDMI 1.

```setState('lgtv.0.input', 'HDMI_2');```

Switches the iput oh the TV to HDMI 2.

```setState('lgtv.0.input', 'HDMI_3');```

Switches the iput oh the TV to HDMI 3.


---

## States

channel - holds the current chanel
on - is true when TV is on and false if TV is off

---


## Changelog

### 1.0.2 (2017-05-23)
* (SMundt) added support for launching Amazon Prime app
### 1.0.0 (2016-09-26)
* (SMundt) added channel polling
* (SMundt) added switching input

### 0.0.4 (2016-09-12)
* (SMundt) solved saving IP address within adapter configuration

### 0.0.3 (2016-09-05)
* (SMundt) added volumeUp true|false
* (SMundt) added volumeDown true|false
* (SMundt) added 3Dmode true|false
* (SMundt) added launch livetv|smartshare|tvuserguide|netflix|youtube|<URL>
* (SMundt) added channel <channelNumber>
* (SMundt) some code cleaned

### 0.0.2 (2016-09-02)
* (SMundt) removed reconnect function, not used
* (SMundt) improved error handling and logging

### 0.0.1 (2016-08-31)
* (SMundt) initial commit


---


## License

The MIT License (MIT)

Copyright (c) 2016 SMundt

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
