## Buster for Bots
This project is a fork of https://github.com/dessant/buster to support automation.

The DOM Shadow Root which wraps Buster solver button is now on open mode, this allow you to automate the interactions with this button.

When the Buster solver is ready to run the CSS class `idle` is added to the solver button `#solver-button` found on the shadow tree. When the solver is running the class `working` is added. When the solver fails the class `retry` is added, you should refresh the recaptcha challenge and try again.

## Building
Automatic speech recognition API configuration is available only for [wit.ai](https://wit.ai). Create a JSON file `secrets.json` on the project directory using `secrets.json.example` as template and fill the API keys for all languages you need, then build the extension with `yarn build:prod:chrome` for example.

Don't build the zip bundle since you need the unpacked extension to load on Chrome automatically through the `--load-extension` command line argument.

For full building instructions see the [wiki](https://github.com/dessant/buster/wiki/Building-the-extension-on-Ubuntu). 

## License

Copyright (c) 2018-2022 Armin Sebastian<br>
Copyright (c) 2022 Heraldo Lucena

This software is released under the terms of the GNU General Public License v3.0.
See the [LICENSE](LICENSE) file for further information.
