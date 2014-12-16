Libscore.com
===========

### Learn

To learn about Libscore, read the [full overview](https://medium.com/@Shapiro/be93165fa497).

For Libscore's API documentation, see below.

--

### Contribute

To help us locate the Github page for a JavaScript library, see [this thread](https://github.com/julianshapiro/libscore/issues/1).

To help us whitelist a popular library that Libscore is failing to detect, see [this thread](https://github.com/julianshapiro/libscore/issues/2).

Take a moment to thank Libscore's sponsors on Twitter: @[Stripe](https://twitter.com/stripe) and @[DigitalOcean](https://twitter.com/digitalocean)!

--

### Badges

Feel free to embed a Libscore badge which uses the [shields.io](http://shields.io) API. Create an issue to give feedback on badges.

Simply replace `{{library}}` with a matching name from [libscore.com](http://libscore.com)

`http://api.libscore.com/badge/{{library}}.svg`

#### Embed just the badge and no link

![](http://api.libscore.com/badge/jQuery.svg)

```
![](http://api.libscore.com/badge/jQuery.svg)
```

#### Link to Libscore results

[![](http://api.libscore.com/badge/jQuery.svg)](https://libscore.com#jQuery)

```
[![](http://api.libscore.com/badge/jQuery.svg)](https://libscore.com#jQuery)
```

#### Embed badge on HTML page

```html
<a href="http://libscore.com#jQuery"><img src="http://api.libscore.com/badge/jQuery.svg" /></a>
```

### API

The Libscore API is freely available to use within constraints due to the project being a non for profit. The API is relativly simple so we don't expect to release breaking changes often, when we do the API will be shifted to v2.

#### Endpoints

Endpoint | Description | Example
------- | ----------- | -------
GET - [/v1/libraries](#libraries) | Get a full list of libraries | [Example](http://api.libscore.com/v1/libraries)
GET - [/v1/libraries/:library](#individual-library) | Get an individual library | [Example](http://api.libscore.com/v1/libraries/jQuery)
GET - [/v1/sites](#sites) | Get a full list of sites | [Example](http://api.libscore.com/v1/sites)
GET - [/v1/sites/:site](#individual-site) | Get an individual site | [Example](http://api.libscore.com/v1/sites/tumblr.com)
GET - [/v1/scripts](#scripts) | Get a full list of scripts | [Example](http://api.libscore.com/v1/scripts)
GET - [/v1/scripts/:script](#individual-script) | Get an individual site | [Example](http://api.libscore.com/v1/scripts/cdnjs.cloudflare.com)

----

#### Libraries

To get the full list of libraries

```
GET http://api.libscore.com/v1/libraries
```

##### Parameters:

* **limit** - Specify the number of results to return e.g. `?limit=500`
* **skip** - Specify the number of results to skip, useful for pagination e.g. `?limit=0`

----

#### Individual Library

To get the full details of a library

```
GET http://api.libscore.com/v1/libraries/:library
```

##### Parameters:

* **limit** - Specify the number of top sites to return e.g. `?limit=500`

##### Examples:

```
GET http://api.libscore.com/v1/libraries/jQuery
// Get full data about JQuery

GET http://api.libscore.com/v1/libraries/$.fn.velocity
// Get full data about Velocity.js

```

----


#### Sites

To get the full list of sites

```
GET http://api.libscore.com/v1/sites
```

##### Parameters:

* **limit** - Specify the number of results to return e.g. `?limit=500`
* **skip** - Specify the number of results to skip, useful for pagination e.g. `?limit=0`


----


#### Individual Site

To get the full list of sites

```
GET http://api.libscore.com/v1/sites/:site
```

##### Parameters:

* **limit** - Specify the number of results to return e.g. `?limit=500`
* **skip** - Specify the number of results to skip, useful for pagination e.g. `?limit=0`

##### Examples:

```
GET http://api.libscore.com/v1/sites/tumblr.com
// Get full data about the website tumblr.com
```

----


#### Scripts

To get the full list of scripts

```
GET http://api.libscore.com/v1/scripts
```

##### Parameters:

* **limit** - Specify the number of results to return e.g. `?limit=500`
* **skip** - Specify the number of results to skip, useful for pagination e.g. `?limit=0`


----


#### Individual Script

To get the full list of scripts

```
GET http://api.libscore.com/v1/scripts/:script
```

##### Parameters:

* **limit** - Specify the number of results to return e.g. `?limit=500`
* **skip** - Specify the number of results to skip, useful for pagination e.g. `?limit=0`

##### Examples:

```
GET http://api.libscore.com/v1/scripts/cdnjs.cloudflare.com
// Get full data about the website cdnjs.cloudflare.com
```
