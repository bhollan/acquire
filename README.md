# Acquire board game

This is the code for my Acquire board game program which can be played at [http://acquire.tlstyer.com/](http://acquire.tlstyer.com/).

## Install dependencies

Install nodejs. I followed the [official instructions](https://nodejs.org/en/download/package-manager/#debian-and-ubuntu-based-linux-distributions):

```bash
curl -sL https://deb.nodesource.com/setup_6.x | sudo -E bash -
sudo apt-get install -y nodejs
```

Install yarn. I followed the [official instructions](https://yarnpkg.com/en/docs/cli/install):

```bash
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt-get update && sudo apt-get install yarn
```

Install other dependencies.

```bash
sudo apt-get install mysql-server python3-pip python3-venv python3-wheel zopfli

python3 -m venv venv
source venv/bin/activate
pip3 install -r requirements.txt

yarn
```

## Download libraries for development use:

    cd lib
    curl http://cdnjs.cloudflare.com/ajax/libs/crypto-js/3.1.2/rollups/sha256.js > crypto-js.rollups.sha256-3.1.2.js
    curl http://cdnjs.cloudflare.com/ajax/libs/jquery/1.12.4/jquery.min.js > jquery-1.12.4.js
    curl http://cdnjs.cloudflare.com/ajax/libs/json3/3.3.2/json3.min.js > json3-3.3.2.js
    curl http://cdnjs.cloudflare.com/ajax/libs/history.js/1.8/native.history.min.js > native.history-1.8.js
    curl http://cdnjs.cloudflare.com/ajax/libs/sockjs-client/1.5.0/sockjs.min.js > sockjs-1.5.0.js
    curl http://cdnjs.cloudflare.com/ajax/libs/stacktrace.js/1.3.1/stacktrace-with-promises-and-json-polyfills.min.js > stacktrace-1.3.1.js
