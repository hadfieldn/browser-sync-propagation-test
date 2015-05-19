## BrowserSync Event-Propagation Demo

Simple test that shows how BrowserSync propagates events
among all windows it is serving.


### Installation

1. `npm install`
2. `bower install`
3. `gulp serve`


### Demonstration

1. Open two or more browsers to the URL given by BrowserSync in the output of the
   `gulp serve` command (above).
2. In the web page that opens, follow the instructions to see that an event sent
   from one window is received by all other windows opened to the same page,
   including those in other browsers.
3. In the terminal window from wich BrowserSync was launched, quit BrowserSync (Ctrl-C) 
   and then enter `http-server -p <port>` to serve the same web page *without* 
   BrowserSync. This time, the signal does not propagate outside the current browser window.
