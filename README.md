# raptorize

Simply drop this anywhere on any site for instant raptor! Loads the Raptorize from [davesierra/raptorize](https://github.com/davesierra/raptorize) which is based on the Raptorize from [ZURB's Playground](http://www.zurb.com/playground/jquery-raptorize).

```js
(function () {
  function loadScript(c,b){var a=document.createElement("script");a.type="text/javascript";a.readyState?a.onreadystatechange=function(){if("loaded"==a.readyState||"complete"==a.readyState)a.onreadystatechange=null,b()}:a.onload=function(){b()};a.src=c;document.getElementsByTagName("head")[0].appendChild(a)};

  loadScript("https://ajax.googleapis.com/ajax/libs/jquery/1.6.1/jquery.min.js", function() {
    loadScript("https://rawgit.com/davesierra/raptorize/master/jquery.raptorize.1.0.js", function() {
      jQuery('html').raptorize({'enterOn': 'timer', 'delayTime': 0});
    });
  });
})();
```

## Cool trick to prank your co-workers
1. Open the BrowserSync client of your co-worker
2. Select "Remote Debug", activate "Remote Debugger (weinre)" and launch it
3. Connect to your co-worker's computer (most likely the one with _localhost_ in it's name)
4. Select the "Console" tab
5. Paste the snippet below
6. RAPTOR-TIME
