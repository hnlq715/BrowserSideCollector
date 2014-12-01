BrowserSideCollector
====================

A project which collects data from web browser using Nginx and javascript.

Table of Contents
-----------------
- [Nginx](#nginx)
- [Javascript](#javascript)
- [Backend](#backend)

Nginx
-----
####sub_filter

This module could replace *</head>* into *</head><script>...</script>*.

####gunzip_filter

This module could unzip the gzipped contents and then do the sub_filter.

####gzip_filter

This module could gzip the unzipped contents back and then send to client.

Javascript
----------
####compatibility

The javascript code injected should take the compatibility into first place.

####async

The javascript code injected should not affect the main process of the web page.

####data

The javascript code injected should be able to collect enough data for analysis.

Backend
-------
####api

The api should support POST with json data, and GET with timestamp and domain...etc.
