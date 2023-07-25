# chromedriver-wrapper

Basic wrapper for Chromedriver for MacOS and Linux

This wrapper will determine the correct version of Chromedriver for the installed version of Google Chrome.
If the required version of chromedriver is not found, then it will be fetched and cached for future uses.

## Installation

This package requires python3. Dependencies can be installed using:

```sh
pip install -r requirements.txt
```

After installing dependencies, ensure that the `bin` directory is in your `$PATH`.

Bash:

```sh
if [ -d "/home/example/git/chromedriver-wrapper/bin" ]; then
    export PATH="/home/example/git/chromedriver-wrapper/bin:$PATH"
fi
```

zsh:
```zsh
if [ -d "/home/example/git/chromedriver-wrapper/bin" ]; then
    path="/home/example/git/chromedriver-wrapper/bin $path"
    export PATH
fi
```

## Usage

Just ensure that the bin directory is in your `$PATH`
You can test it's working correctly by running `chromedriver`

## Options

You can specify a couple of options here to the chromedriver wrapper. These can be specified in the `.env` file.

### Specify extra options to add to chromedriver

```
EXTRA_OPTIONS="--verbose --log-path=/tmp/chromedriver.log"
```

### Specify an alternative location to store chromedriver binaries

```
PATH_TO_CACHEDIR="/tmp/mycache"
```

### Specify an alternative path to Chrome itself

```
PATH_TO_CHROME="/my/path/to/chrome/canary"
```
