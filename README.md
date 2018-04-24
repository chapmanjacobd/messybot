# Messybot

Messybot is the opinionated interface for a building. 

### Requirements:

- A Raspberry Pi [setup instructions](https://github.com/dantaeyoung/messybot/blob/master/pi_setup.md)
- a Space

### Optional Requirements

- a Slack group
- Isy994 Z-wave controller and devices
- An Art-Net DMX controller
- An HDMI monitor attached


### Installation:

- Copy `config.js.example` to `config.js`, and edit the config to match.
- Copy `messybot.js.example` to `messybot.js`, and uncomment/comment lines as needed.
- `npm install`
- Test with `npm start`
- Install with `pm2 start app/messybot.js`
- Make sure that pm2 is running as a [service](http://pm2.keymetrics.io/docs/usage/startup/#generating-a-startup-script) on boot.
- Save scripts for startup: `pm2 save`


### App structure

- `app/messybot.js` initializes execution.
- Abilities are in the `app/abilities` directory. Controls such as Sonos or other things could be added here.
- Behaviors are in the `app/behaviors` directory.






