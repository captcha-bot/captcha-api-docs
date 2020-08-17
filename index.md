Authored by: Zoro <zoro@captchabot.xyz></br>
Date: 8/17/2020

The following endpoints are in use for [API Version 1](https://api.captchabot.xyz/v1/) accesible via https://api.captchabot.xyz/v1/
***
# v1/

- protected/ - REQUIRES AUTHENTICATION

	- ``config/``</br></br>
		- ``GET :id`` ~ Returns the guild config of the specified ``id``. If none is found return the default config.</br></br>
		- ``PATCH :id`` ~ Update the guilds config with the new data. Reading from body::config</br></br>
		- ``GET :id/prefix`` ~ Returns the cached prefix, if none. Return `!`</br></br>
		- ``PATCH :id/prefix`` ~ Updates the cache with the new prefix included in the bodies content.</br></br>
- stats/
	- ``GET /`` ~ Returns the gathered stats. used for botlist posting etc.</br></br>

- captcha/
	- ``GET /`` ~ Returns generated captcha with data: ```{ code: String, buffer: Buffer }```