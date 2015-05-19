## BrowserSync Event-Propagation Demo

Simple test that shows how browser-sync propagates events
among all windows it is serving.


### Installation

1. `npm install`
2. `bower install`
3. `gulp serve`


### Demonstration

1. Open two or more browsers to the browser-sync URL given in the output of the
   `serve` gulp task.
2. Follow the instructions in the web page that opens to see that an event sent
   from one window is received by all other windows opened to the same page,
   including those in other browsers.
3. Terminate BrowserSync (Ctrl-C) and then enter `http-server -p <port>` to serve
   the same web page without browser-sync. This time, the signal does not
   propagate outside the current browser window.
