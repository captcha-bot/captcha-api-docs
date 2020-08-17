- Authored by: Zoro <zoro@captchabot.xyz>
- Date: 8/17/2020

The following endpoints are in use for [API Version 1](https://api.captchabot.xyz/v1/) accesible via https://api.captchabot.xyz/v1/

# v1/

- protected/ - **REQUIRES AUTHENTICATION**

	- ``config/``
		- ``GET :id`` ~ Returns the guild config of the specified ``id``. If none is found return the default config.
		- ``PATCH :id`` ~ Update the guilds config with the new data. Reading from body::config
		- ``GET :id/prefix`` ~ Returns the cached prefix, if none. Return `!`
		- ``PATCH :id/prefix`` ~ Updates the cache with the new prefix included in the bodies content.
- stats/
	- ``GET /`` ~ Returns the gathered stats. used for botlist posting etc.

- captcha/
	- ``GET /`` ~ Returns generated captcha with data: ```{ code: String, buffer: Buffer }```