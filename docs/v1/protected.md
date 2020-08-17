__INTERNAL USE ONLY__

- ``config/``
	- ``GET :id`` ~ Returns the guild config of the specified ``id``. If none is found return the default config.
	- ``PATCH :id`` ~ Update the guilds config with the new data. Reading from body::config
	- ``GET :id/prefix`` ~ Returns the cached prefix, if none. Return `!`
	- ``PATCH :id/prefix`` ~ Updates the cache with the new prefix included in the bodies content.