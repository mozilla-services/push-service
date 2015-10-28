# Mozilla Push Service

Mozilla Push Service is the server-side project support Push Notifications in
the [Firefox browser][ffx] and [Firefox OS][fxos].

## People and Places

* [Ben Bangert](https://github.com/bbangert) - Engineering (San Francisco, UTC-8)
* [JR Conlin](https://github.com/jrconlin) - Engineering (Mountain View, UTC-8)
* [Kit Cambridge](https://github.com/kitcambridge) - Engineering (Mountain View, UTC-8)
* [Richard Pappalardo](https://github.com/rpappalax) - QA (Mountain View, UTC-8)
* [Jeremy Orem](https://github.com/oremj) - Operations (Portland, UTC-8)
* [Chris Karlof](https://github.com/ckarlof) - Identity Services Manager (San Francisco, UTC-8)

We meet for a weekly stand-up, as well as a larger meeting on Wednesday's to
discuss Push specification details and client coordination.

Additional ways to get in contact with the team:

* The [Push mailing list](http://groups.google.com/a/mozilla.com/group/push/)
* The `#push` channel on [Mozilla IRC](https://wiki.mozilla.org/IRC)

## Code

The current production deployment of Push is a Python-based websocket server
named **autopush**, developed on Github.

- [autopush](https://github.com/mozilla-services/autopush)

Legacy Go-based Push server (no longer developed/running)

- [pushgo](https://github.com/mozilla-services/pushgo)

[fxos]: https://www.mozilla.org/en-US/firefox/os/
[ffx]: https://www.mozilla.org/en-US/firefox/
