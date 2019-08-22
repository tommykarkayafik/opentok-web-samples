# OpenTok.js Screen Sharing Video chat

In this sample application you can see how to share screens using OpenTok, and how to use the [`unpublish()`](https://tokbox.com/developer/sdks/js/reference/Session.html#unpublish), [`preventDefault()`](https://tokbox.com/developer/sdks/js/reference/StreamEvent.html#preventDefault) methods to disconnect and reconnect to a session using the same publisher.

It is quite similar to the [Basic Video Chat](../Basic%20Video%20Chat) example and adds the screen sharing capabilities to it.

## Running the App

* Simply open [index.html](index.html) in your browser.
* The "screen sharing" button toggles publishing your screen.
  
  This is done by unpublishing the stream from the active publisher and publishing the inactive one, while still keeping both of the publishers alive.
* If you are both subscribed to a screen sharing stream, and publishing a screen sharing screen of your own, you can click the small `<div>` to switch between the small and the big ones.
## Known Limitations

* In Opera and older versions of Chrome (prior to Chrome 72), to publish a screen-sharing video, the client needs to add an extension that enables publishing screen-sharing streams for your domain. (See [Developing a screen-sharing extension](https://tokbox.com/developer/guides/screen-sharing/js/#chrome-extension).)

* Publishing screen-sharing streams is currently not supported in Safari or Edge.
  