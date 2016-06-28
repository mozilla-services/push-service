# Welcome to the Mozilla Push Service [![Build Status](https://travis-ci.org/mozilla-services/autopush.svg?branch=master)](https://travis-ci.org/mozilla-services/autopush)

Mozilla Push Service is the server-side project support Push Notifications in
the [Firefox browser][ffx] and [Firefox OS][fxos].

## Contributing to the Mozilla Push Service

Interested in contributing to the development of Mozilla's Push Service?
Complete documentation on the Push Service, History, and how to get involved
can be found at [the Push Service's documentation](https://mozilla-push-service.readthedocs.io/).

##### Bugs List: [waffle.io/mozilla-services/push-service](https://waffle.io/mozilla-services/push-service/)

## Building this Documentation

```
pip install mkdocs
```

Build:

```
mkdocs build
```

Server + File Watching:

```
mkdocs serve --dev-addr localhost:9032
```

Publishing to https://mozilla-push-service.readthedocs.io

```
# Documentation is built automatically from this repository.
git commit
git push origin/master
```

[fxos]: https://www.mozilla.org/en-US/firefox/os/
[ffx]: https://www.mozilla.org/en-US/firefox/
