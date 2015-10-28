# Mozilla Push Service

Mozilla Push Service is the server-side project support Push Notifications in
the [Firefox browser][ffx] and [Firefox OS][fxos].

## History

The Push Service was originally developed in Go, utilizing a websocket
connection from [Firefox OS][fxos] to the Push service. It was deployed in 2013
with the [SimplePush DOM API][https://developer.mozilla.org/en-US/docs/Web/API/Simple_Push_API]
that runs under [Firefox OS][fxos]. This API only supported incrementing
version numbers, to wake a device so that it could check with an Application
Server to determine what to display.

In 2015 the Push Service was rewritten in Python, and added preliminary
[WebPush][wp] support for carrying data in push messages. The underlying
protocol used between [Firefox][ffx] and the Push Service is an extended
[SimplePush Protocol][] that will eventually be deprecated in favor of a
complate [WebPush][wb] HTTP 2.0 protocol. 

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
named **autopush**, developed on Github. The Push Service team has several
repositories for development of the Push Server, and supporting tooling.

- [autopush](https://github.com/mozilla-services/autopush) - Actively developed
  Push server
- [pushgo](https://github.com/mozilla-services/pushgo) - Legacy Go-based Push
  server (no longer developed or deployed)
- [push-tester](https://github.com/bbangert/push-tester) - SimplePush load
  tester (no longer developed)

[wp]: https://webpush-wg.github.io/webpush-protocol/
[fxos]: https://www.mozilla.org/en-US/firefox/os/
[ffx]: https://www.mozilla.org/en-US/firefox/
