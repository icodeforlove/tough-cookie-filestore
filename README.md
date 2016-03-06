# File Cookie Store

tough-cookie-filestore is a File store for tough-cookie module. See 
[tough-cookie documentation](https://github.com/goinstant/tough-cookie#constructionstore--new-memorycookiestore-rejectpublicsuffixes) for more info.


## installation

    $ npm install tough-cookie-filestore

## Options

  `path` file path of cookiejar.

## Usage

  var FileCookieStore = require("tough-cookie-filestore");
  var CookieJar = require("tough-cookie").CookieJar;

  var store = new FileCookieStore("./cookie.json");
  store.load(function () {
  	var jar = new CookieJar(store);
  });

## License

 MIT
