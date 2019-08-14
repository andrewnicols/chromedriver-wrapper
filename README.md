# chromedriver-wrapper
Basic wrapper for Chromedriver for MacOS and Linux

This wrapper will determine the correct version of Chromedriver for the installed version of Google Chrome.
If the required version of chromedriver is not found, then it will be fetched and cached for future uses.

## Usage
Just ensure that the bin directory is in your `$PATH`
You can test it's working correctly by running `chromedriver`

## Options
You can specify a couple of options here:

### Specify extra options to add to chromedriver
```
export EXTRA_OPTIONS="--verbose --log-path=/tmp/chromedriver.log"
```

### Specify an alternative location to store chromedriver binaries
```
export PATH_TO_CACHEDIR="/tmp/mycache"
```

### Specify an alternative path to Chrome itself
```
export PATH_TO_CHROME="/my/path/to/chrome/canary"
```

### Specify an alternative filename to download the file from Google
You may need this if you run a 32-bit version of Linux.
```
export CHROMEDRIVER_SOURCE_FILENAME="linux32.zip"
```
