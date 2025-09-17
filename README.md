# site-setting-override

Example plugin for overriding a Discourse site setting.

## Installation

Proceed with a normal [installation of a plugin](https://meta.discourse.org/t/install-a-plugin/19157?u=jomaxro).


## About

This is a basic example plugin. If installed, this plugin will override the `max_post_length` site setting so the default value becomes 1,000,000 characters (the core default is 32,000). During earlier testing we assumed the request package size would also need to be increased, but Discourse handled million-character posts without further tuning. If your hosting environment enforces lower payload limits you may still need to raise them accordingly.

To override other settings, fork this plugin and modify `config/settings.yml`. Discourse site settings are located at https://github.com/discourse/discourse/blob/master/config/site_settings.yml.
