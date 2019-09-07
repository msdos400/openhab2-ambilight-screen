# openHAB2 Ambilight Screen
![Release](https://img.shields.io/github/release/thedavesky/openhab2-ambilight-screen.svg?style=flat-square)
![Repo size](https://img.shields.io/github/repo-size/thedavesky/openhab2-ambilight-screen.svg?style=flat-square)
![Language count](https://img.shields.io/github/languages/count/thedavesky/openhab2-ambilight-screen.svg?style=flat-square)
![Top language](https://img.shields.io/github/languages/top/thedavesky/openhab2-ambilight-screen.svg?style=flat-square)
![Last commit](https://img.shields.io/github/last-commit/thedavesky/openhab2-ambilight-screen.svg?style=flat-square)
![License](https://img.shields.io/github/license/thedavesky/openhab2-ambilight-screen.svg?style=flat-square)
> A program that calculates average colour from the screen and sends it to the RGB strip connected to the openHAB server to do ambilight backlight.

This program written in Python 3 can do this same thing as Philips Ambilight, but using RGB strip connected to openHAB server. It's constantly calculates average color from one screen of computer and sends it to server. It uses most efficiency libraries to do screenshots and calculates, so its speed is about 10 FPS at 1080p resolution. It's multiplatform, so Windows, MacOS and Linux are supported.

## Installation
Install libraries to python environment by running:
```
pip3 install -r requirements.txt
```

Make config.json file by using config.sample.json as example:
```json
{
    "openhab_url": "<URL to openHAB panel without slash at the end>",
    "openhab_item_name": "<RGB strip's item name in openHAB panel>",
    "openhab_username": "<Username to openHAB panel, if auth is sets>",
    "openhab_password": "<Password to openHAB panel, if auth is sets>",
    "screen_number": "<Screen number which program has to recording (1 is first, 2 is second, etc..)>"
}
```

## Running
Just run it from command line:
```
python3 ambilight-screen.py
```

## Compatibility
- openHAB2
- Arduino Smart Home Gateway

## Status
Project is: **finished**

## Pictures
![Running program](https://raw.githubusercontent.com/thedavesky/openhab2-ambilight-screen/assets/images/running.jpg)
![Effect](https://raw.githubusercontent.com/thedavesky/openhab2-ambilight-screen/assets/images/effect.gif)

## Author
Copyright ⓒ 2019 Dawid Maliszewski (thedavesky) <dawid@thedavesky.com>

## License
This project is licensed under the **GNU General Public License v3.0** - see the [LICENSE](https://github.com/thedavesky/openhab2-ambilight-screen/blob/master/LICENSE) file for details.
