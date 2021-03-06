# Letterboxd

`v0.1a` - **THE CODE IS CURRENTLY IN AN ALPHA STATE, AND MAY BE VERY BROKEN.**

A Python 3 implementation of the [Letterboxd API v0](http://api-docs.letterboxd.com/).
 
Currently a ***WORK-IN-PROGRESS,*** focusing first on retrieving watchlists and other lists.

## Usage

Instantiate the `Letterboxd` class, and provide it with the `api_base` URL for the API, your `api_key`, and your `api_secret`. You can pass it as a variable to the class init, or add it to your environment variables as:

```
export LBXD_API_KEY="YOUR_KEY_HERE"
export LBXD_API_SECRET="YOUR_SECRET_HERE"
```

If you do not provide an `api_base`, it currently defaults to `https://api.letterboxd.com/api/v0`.

For testing, you can also add environment variables for an account user name and password, and the location of your [Charles proxy SSL certificate](https://www.charlesproxy.com/documentation/using-charles/ssl-certificates/).

```
export LBXD_USERNAME="YOUR_USERNAME"
export LBXD_PASSWORD="YOUR_PASSWORD"
export CHARLES_CERTIFICATE="/path/to/charles-ssl-proxying-certificate.pem"
```