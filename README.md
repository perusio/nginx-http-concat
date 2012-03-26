# HTTP Concatenation module for Nginx

## Introduction 

This is a module that is distributed with
[tengine](http://tengine.taobao.org) which is a distribution of
[Nginx](http://nginx.org) that is used by the e-commerce/auction site
[Taobao.com](http://en.wikipedia.org/wiki/Taobao). This distribution
contains some modules that are new on the Nginx scene. The
`ngx_http_concat` module is one of them.

The module is inspired by Apache's
[`modconcat`](http://code.google.com/p/modconcat). It follows the same
pattern for enabling the concatenation. It uses two `?`, like this: 

    http://example.com/??style1.css,style2.css,foo/style3.css
    
If a **third** `?` is present it's treated as **version string**. Like
this:

    http://example.com/??style1.css,style2.css,foo/style3.css?v=102234

## New Repository

The new repo is at
[https://github.com/taobao/nginx-http-concat](https://github.com/taobao/nginx-http-concat).
