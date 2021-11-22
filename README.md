# required.js
Synchronously load javascript files with this minified 1 liner.

    function required(n){var o=new XMLHttpRequest;o.open("GET",n,!1),o.onreadystatechange=function(){var e=o.response||o.responseText;4===o.readyState&&(200===o.status?(eval.apply(window,[e]),console.log("script loaded: ",n)):console.log("ERROR: script not loaded: ",n))},o.send(null)}
