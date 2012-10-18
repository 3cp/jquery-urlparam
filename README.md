# jquery-urlparam

A tiny jQuery plugin for reading current url parameters.

##Usage

For instance, for url
    http://your.site.com?n1=v1&n2=v2a&n2=v2b&n3

    $.urlparam(); // => {n1: 'v1', n2: ['v2a', 'v2b'], n3: ''}
    $.urlparam('n1'); // => 'v1'
    $.urlparam('n2'); // => ['v2a', 'v2b']
    $.urlparam('n3'); // => ''
    $.urlparam('n4'); // => undefined

For url without query part, it always returns undefined.


