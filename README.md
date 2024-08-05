


# Awesome Nginx [![Build Status](https://travis-ci.org/agile6v/awesome-nginx.svg?branch=master)](https://travis-ci.org/agile6v/awesome-nginx) [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
A curated list of awesome nginx distributions, third party modules, active developers and so forth.

If you want to contribute, please submit a pull request.

Feel free to add your project :)


# Table of Contents
* [Well-known Distributions](#well-known-distributions)
* [Embeddable Scripting Languages](#embeddable-scripting-languages)
* [Third Party Modules](#third-party-modules)
	* [C Modules](#c-modules)
    * [Rust Modules](#rust-modules)
	* [Lua Modules](#lua-modules)
* [Built-in Modules](#built-in-modules)
* [Njs Projects](#njs-projects)
* [Tools](#tools)
* [Tutorials](#tutorials)
* [Mailing Lists](#mailing-lists)
* [Forum](#forum)
* [Active Developers](#active-developers)

## Well-known Distributions
* [NGINX](https://nginx.org/en/docs/install.html)
* [FreeNGINX](https://freenginx.org/)
* [OpenResty](https://github.com/openresty/ngx_openresty)
* [Tengine](https://github.com/alibaba/tengine)

## Embeddable Scripting Languages
* [lua](https://github.com/openresty/lua-nginx-module)
* [javascript (njs)](https://nginx.org/en/docs/njs/)
* [perl](http://nginx.org/en/docs/http/ngx_http_perl_module.html)
* [mruby](https://github.com/matsumoto-r/ngx_mruby)
* [clojure](https://github.com/nginx-clojure/nginx-clojure)
* [php](https://github.com/rryqszq4/ngx_php)
* [wasm](https://github.com/Kong/ngx_wasm_module)

## Builder
This is bash command line builder that uses this curated list to automate installing and compiling nginx
* [nginx-builder](https://github.com/gp187/nginx-builder)

## Third Party Modules
These modules are not distributed with the Nginx source.


### C Modules
* [lua-nginx-module](https://github.com/openresty/lua-nginx-module) - Embed the Power of Lua into NGINX.
* [nginx-rtmp-module](https://github.com/arut/nginx-rtmp-module) - NGINX-based Media Streaming Server.
* [xss-nginx-module](https://github.com/openresty/xss-nginx-module) - Native support for cross-site scripting (XSS) in an nginx.
* [srcache-nginx-module](https://github.com/openresty/srcache-nginx-module) - Transparent subrequest-based caching layout for arbitrary nginx locations. 
* [replace-filter-nginx-module](https://github.com/openresty/replace-filter-nginx-module) - Streaming regular expression replacement in response bodies. 
* [rds-json-nginx-module](https://github.com/openresty/rds-json-nginx-module) - An nginx output filter that formats Resty DBD Streams generated by ngx_drizzle and others to JSON. 
* [echo-nginx-module](https://github.com/openresty/echo-nginx-module) - An Nginx module for bringing the power of "echo", "sleep", "time" and more to Nginx's config file. 
* [headers-more-nginx-module](https://github.com/openresty/headers-more-nginx-module) - Set, add, and clear arbitrary output headers. 
* [rds-csv-nginx-module](https://github.com/openresty/rds-csv-nginx-module) - Nginx output filter module to convert Resty-DBD-Streams (RDS) to Comma-Separated Values (CSV). 
* [memc-nginx-module](https://github.com/openresty/memc-nginx-module) - An extended version of the standard memcached module that supports set, add, delete, and many more memcached commands.. 
* [encrypted-session-nginx-module](https://github.com/openresty/encrypted-session-nginx-module) - encrypt and decrypt nginx variable values. 
* [redis2-nginx-module](https://github.com/openresty/redis2-nginx-module) - Nginx upstream module for the Redis 2.0 protocol. 
* [drizzle-nginx-module](https://github.com/openresty/drizzle-nginx-module) - an nginx upstream module that talks to mysql and drizzle by libdrizzle. 
* [array-var-nginx-module](https://github.com/openresty/array-var-nginx-module) - Add support for array-typed variables to nginx config files.
* [set-misc-nginx-module](https://github.com/openresty/set-misc-nginx-module) - Various set_xxx directives added to nginx's rewrite module (md5/sha1, sql/json quoting, and many more). 
* [nginx-eval-module](https://github.com/vkholodkov/nginx-eval-module) - A module for evaluating memcached or proxy response into variable.
* [ngx_pagespeed](https://github.com/apache/incubator-pagespeed-ngx) - Automatic PageSpeed optimization module for Nginx. 
* [ngx_devel_kit](https://github.com/simpl/ngx_devel_kit) - Nginx Development Kit - an Nginx module that adds additional generic tools that module developers can use in their own modules.
* [ngx_cache_purge](https://github.com/FRiCKLE/ngx_cache_purge) - nginx module which adds ability to purge content from FastCGI, proxy, SCGI and uWSGI caches. 
* [ngx_postgres](https://github.com/FRiCKLE/ngx_postgres) - upstream module that allows nginx to communicate directly with PostgreSQL database.
* [nginx-backtrace](https://github.com/alibaba/nginx-backtrace) - A Nginx module to dump backtrace when a worker process exits abnormally. 
* [nginx-http-concat](https://github.com/alibaba/nginx-http-concat) - A Nginx module for concatenating files in a given context: CSS and JS files usually.
* [nginx-http-user-agent](https://github.com/alibaba/nginx-http-user-agent) - A nginx module to match browsers and crawlers. 
* [nginx-http-footer-filter](https://github.com/alibaba/nginx-http-footer-filter) - A nginx module that prints some text in the footer of a request.
* [nginx-http-slice](https://github.com/alibaba/nginx-http-slice) - Nginx module for serving a file in slices (reverse byte-range). 
* [nginx-clojure](https://github.com/nginx-clojure/nginx-clojure) - Nginx module for embedding Clojure or Java or Groovy programs, typically those Ring based handlers.
* [nginx-audio-track-for-hls-module](https://github.com/flavioribeiro/nginx-audio-track-for-hls-module) - Nginx module that generates audio track for HTTP Live Streaming (HLS) streams on the fly. 
* [nginx-access-plus](https://github.com/nginx-clojure/nginx-access-plus) - nginx module allows limiting access to certain http request methods and client addresses.
* [ngx_http_subrange_module](https://github.com/Qihoo360/ngx_http_subrange_module) - Split one big HTTP/Range request to multiple subrange requesets. 
* [nginx_tcp_proxy_module](https://github.com/yaoweibin/nginx_tcp_proxy_module) - add the feature of tcp proxy with nginx, with health check and status monitor.
* [nginx_ajp_module](https://github.com/yaoweibin/nginx_ajp_module) - support AJP protocol proxy with Nginx. 
* [ngx_http_substitutions_filter_module](https://github.com/yaoweibin/ngx_http_substitutions_filter_module) - a filter module which can do both regular expression and fixed string substitutions for nginx.
* [nginx-sticky-module](https://github.com/yaoweibin/nginx-sticky-module) - A nginx module to add an upstream server persistance using cookies. 
* [nginx-http-sysguard](https://github.com/alibaba/nginx-http-sysguard) - A Nginx module to protect servers when system load or memory use goes too high.
* [nginx-tfs](https://github.com/alibaba/nginx-tfs) - An Asynchronous Nginx module providing a RESTful API for TFS (Taobao File System). 
* [ngx_aws_auth](https://github.com/anomalizer/ngx_aws_auth) - nginx module to proxy to authenticated AWS services.
* [nginx_mod_akamai_g2o](https://github.com/refractalize/nginx_mod_akamai_g2o) - Nginx Module for Authenticating Akamai G2O requests. 
* [ngx_supervisord](https://github.com/FRiCKLE/ngx_supervisord) - nginx module providing API to communicate with supervisord and manage (start/stop) backends on-demand.
* [ngx_http_google_filter_module](https://github.com/cuber/ngx_http_google_filter_module) - Nginx Module for Google Mirror. 
* [ngx_http_dyups_module](https://github.com/yzprofile/ngx_http_dyups_module) - update upstreams' config by restful interface.
* [ngx_sync_msg_module](https://github.com/yzprofile/ngx_sync_msg_module) - This module provides a mechanism to sync messages between workers for your module. 
* [nginx-upload-module](https://github.com/fdintino/nginx-upload-module) - A module for nginx web server for handling file uploads using multipart/form-data encoding (RFC 1867).
* [nginx-video-thumbextractor-module](https://github.com/wandenberg/nginx-video-thumbextractor-module) - Nginx module to extract thumbs from a video file. 
* [nginx-push-stream-module](https://github.com/wandenberg/nginx-push-stream-module) - A pure stream http push technology for your Nginx setup. Comet made easy and really scalable.
* [nginx-module-vts](https://github.com/vozlt/nginx-module-vts) - Nginx virtual host traffic status module.
* [url-protector-nginx-module](https://github.com/Trax-retail/url-protector-nginx-module) - Nginx module which adds ability to decrypt strings encrypted with xxtea algorithm.
* [nginx-module-url](https://github.com/vozlt/nginx-module-url) - Nginx url encoding converting module.
* [ngx_small_light](https://github.com/cubicdaiya/ngx_small_light) - Dynamic Image Transformation Module For nginx. 
* [nginx-upstream-fair](https://github.com/gnosek/nginx-upstream-fair) - The fair load balancer module for nginx.
* [nginx_modSecurity](https://github.com/SpiderLabs/ModSecurity-nginx) - ModSecurity is an open source, cross platform web application firewall (WAF) engine for Apache, IIS and Nginx that is developed by Trustwave's SpiderLabs. 
* [nginx-fluentd-module](https://github.com/fluent/nginx-fluentd-module) - Nginx module for Fluentd data collector.
* [ngx_zeromq](https://github.com/FRiCKLE/ngx_zeromq) - ZeroMQ transport for nginx. 
* [ngx_cache_viewer](https://github.com/agile6v/ngx_cache_viewer) - nginx module which adds ability to view cache node info from FastCGI, proxy, SCGI and uWSGI caches.
* [nginx_http_push_module](https://github.com/slact/nginx_http_push_module) - Turn NGiNX into an adept HTTP push server. 
* [nginx-selective-cache-purge-module](https://github.com/wandenberg/nginx-selective-cache-purge-module) - A module to purge cache by GLOB patterns.. 
* [naxsi](https://github.com/wargio/naxsi) - NAXSI is an open-source, high performance, low rules maintenance WAF for NGINX. 
* [couchbase-nginx-module](https://github.com/couchbaselabs/couchbase-nginx-module) - The module for nginx webserver to access Couchbase Server. 
* [protobuf-nginx](https://github.com/dbcode/protobuf-nginx) - Google Protocol Buffers code generator for nginx module developers. 
* [testcookie-nginx-module](https://github.com/kyprizel/testcookie-nginx-module) - simple robot mitigation module using cookie based challenge/response technique. 
* [nginx_circle_gif](https://github.com/evanmiller/nginx_circle_gif) - this module generates simple circle images with the colors and size specified in the URL. 
* [ngx_http_estreaming_module](https://github.com/whatvn/ngx_http_estreaming_module) - An adaptive hls streaming module for nginx. 
* [ngx_mruby](https://github.com/matsumoto-r/ngx_mruby) - ngx_mruby - A Fast and Memory-Efficient Web Server Extension Mechanism Using Scripting Language mruby for nginx. 
* [ngx_http_geoip2_module](https://github.com/leev/ngx_http_geoip2_module) - creates variables with values from the maxmind geoip2 databases based on the client IP (supports both IPv4 and IPv6). 
* [tcp-nginx-module](https://github.com/laocai/tcp-nginx-module) - Use nginx as a common TCP server framework. 
* [ngx_openresty](https://github.com/openresty/ngx_openresty) - Turning Nginx into a Full-fledged Web App Server. 
* [iconv-nginx-module](https://github.com/calio/iconv-nginx-module) - a character conversion nginx module using libiconv. 
* [form-input-nginx-module](https://github.com/calio/form-input-nginx-module) - This is a nginx module that reads HTTP POST and PUT request body encoded in "application/x-www-form-urlencoded", and parse the arguments in request body into nginx variables.. 
* [ngx-ip2location](https://github.com/chaizhenhua/ngx-ip2location) - Nginx IP2Location Module. 
* [nginx-hmux-module](https://github.com/wangbin579/nginx-hmux-module) - The module implements resin's hmux protocol in nginx. 
* [nginx_ocsp_proxy-module](https://github.com/kyprizel/nginx_ocsp_proxy-module) - Nginx OCSP processing module designed for response caching. 
* [nginx-hmac-secure-link](https://github.com/nginx-modules/nginx-hmac-secure-link) - Alternative Nginx secure link module with support for MD5, SHA-1, and SHA-2 hashes. 
* [waf-nginx-module](https://github.com/gsdu8g9/waf-nginx-module) - A lightweight web application firewall module for nginx.. 
* [ngx-gm-filter](https://github.com/liseen/ngx-gm-filter) - Another image filter based GraphicsMagick.. 
* [nginx-mod-so](https://github.com/hamano/nginx-mod-so) - nginx_mod_so is dynamic loadable module for Nginx. 
* [nginx-auth-ldap](https://github.com/kvspb/nginx-auth-ldap) - LDAP authentication module for nginx. 
* [nginx-xsltproc-module](https://github.com/yoreek/nginx-xsltproc-module) - XSLT processor bases on Nginx. 
* [nginx-dlg-auth](https://github.com/algermissen/nginx-dlg-auth) - NGINX module for delegating authentication and authorization to an HTTP gateway. 
* [ngx_http_qqwry_module](https://github.com/anjuke/ngx_http_qqwry_module) - A nginx module that creates variables with location info from QQWry. 
* [nginx-markdown-module](https://github.com/gabrielfalcao/nginx-markdown-module) - renderize markdown as HTML directly from your upstream server. 
* [nginx-nonewlines](https://github.com/vedang/nginx-nonewlines) - This is an nginx module to strip the served HTML of all newlines (\n and \r characters). 
* [nginx-udplog-module](https://github.com/vkholodkov/nginx-udplog-module) - Implementation of logging using BSD Syslog Protocol for nginx (RFC 3164). 
* [nginx-fancyindex](https://github.com/aperezdc/ngx-fancyindex) - nginx fancy index module. 
* [nginx_ipset_blacklist](https://github.com/Vasfed/nginx_ipset_blacklist) - nginx module to use linux netfilter ipsets as blacklists. 
* [nginx-mogilefs-module](https://github.com/vkholodkov/nginx-mogilefs-module) - MogileFS client for nginx. 
* [ngx_http_php_session](https://github.com/replay/ngx_http_php_session) - nginx module to parse php sessions. 
* [ngx_trace](https://github.com/zzzcpan/ngx_trace) - runtime call tracer for nginx. 
* [nginx-qrcode](https://github.com/alexchamberlain/nginx-qrcode) - Native QR encoding for Nginx Web Server. 
* [nginx-dav-ext-module](https://github.com/arut/nginx-dav-ext-module) - NGINX WebDAV missing methods support (PROPFIND & OPTIONS). 
* [nginx-gridfs](https://github.com/mdirolf/nginx-gridfs) - Nginx module for serving files from MongoDB's GridFS. 
* [Session-Binding-Proxy](https://github.com/wburgers/Session-Binding-Proxy) - An Nginx module capable of binding the application session to the SSL session by encrypting the application cookie with a secret key and the SSL master key. 
* [ngx_http_gif_magick](https://github.com/mschenck/ngx_http_gif_magick) - nginx http filter module for dynamically resizing gifs with ImageMagick. 
* [nginx-upload-progress-module](https://github.com/masterzen/nginx-upload-progress-module) - Nginx module implementing an upload progress system, that monitors RFC1867 POST uploads as they are transmitted to upstream servers. 
* [ngx_http_avatars_gen_module](https://github.com/dizballanze/ngx_http_avatars_gen_module) - Nginx module for on-the-fly generating of avatars based on user initials.
* [ngx_http_proxy_connect_module](https://github.com/chobits/ngx_http_proxy_connect_module) - A forward proxy module for CONNECT request handling
* [modjpeg-nginx](https://github.com/ioppermann/modjpeg-nginx) - Filter module for adding overlays and logos to JPEGs on-the-fly without degrading the quality of the image.
* [nginx-c-function](https://github.com/Taymindis/nginx-c-function) - It is a NGINX module that allow you to link your .so(c/c++) application in server context and call the function of .so application in location directive.
* [ngx_lfqueue](https://github.com/Taymindis/ngx_lfqueue) - a lock free queue(enq/deq) container running on nginx share memory and it enqueue/dequeue the messages across multiple threads and multiple workers without any locking.
* [ngx_lfstack](https://github.com/Taymindis/ngx_lfstack) - a lock free stack(push/pop) container running on nginx share memory and it push/pop the messages across multiple threads and multiple workers without any locking.
* [ngx-stomp](https://github.com/Taymindis/ngx-stomp) - A STOMP upstream module on nginx, STOMP is the Simple (or Streaming) Text Orientated Messaging Protocol.
* [nginx-elastic-client](https://github.com/Taymindis/nginx-elastic-client) - To structure your elastic client command in your nginx proxy for multiple elasticsearch server.
* [zstd-nginx-module](https://github.com/tokers/zstd-nginx-module) - Nginx modules for the Zstandard compression.
* [nginx_upstream_check_module](https://github.com/yaoweibin/nginx_upstream_check_module) - Health checks upstreams for nginx.
* [ngx_php](https://github.com/rryqszq4/ngx_php) - Embedded php script language for nginx-module.
* [ngx_http_guess_mime_module](https://github.com/ohnx/nginx-guess-mime) - Guess the MIME type of files served using libmagic.
* [ngx_http_stat_check](https://github.com/mk-fg/nginx-stat-check) - Dynamic access blacklisting configuration via filesystem paths.
* [nginx_mime_magic_module](https://github.com/FadedCoder/nginx-mime-magic-module) - Another MIME guesser using libmagic with configurable Magic database path and fallback or compulsory mode.
* [nginx-otel](https://github.com/nginxinc/nginx-otel) - Module providing support for OpenTelemetry distributed tracing.
* [nginx-http-est](https://github.com/61131/nginx-http-est) - Enrollment over Secure Transport (EST) module for Nginx
* [nginx-http-auth-totp](https://github.com/61131/nginx-http-auth-totp) - Time-based one-time password (TOTP) authentication for Nginx

## Rust Modules
* [ngx-rust](https://github.com/nginxinc/ngx-rust) - Rust bindings for Nginx modules.

### Lua Modules
* [lua-resty-redis](https://github.com/openresty/lua-resty-redis) - Lua redis client driver for the ngx_lua based on the cosocket API. 
* [lua-resty-memcached](https://github.com/openresty/lua-resty-memcached) - Lua memcached client driver for the ngx_lua based on the cosocket API. 
* [lua-resty-mysql](https://github.com/openresty/lua-resty-mysql) - Nonblocking Lua MySQL driver library for ngx_lua. 
* [lua-resty-postgres](https://github.com/azurewang/lua-resty-postgres) - Nonblocking Lua PostgreSQL driver library for ngx_lua. 
* [lua-resty-cassandra](https://github.com/jbochi/lua-resty-cassandra) - Pure Lua Cassandra client using CQL binary protocol.
* [lua-resty-fastcgi](https://github.com/benagricola/lua-resty-fastcgi) - Lua FCGI client driver for ngx_lua based on the cosocket API. 
* [lua-resty-ssdb](https://github.com/LazyZhu/lua-resty-ssdb) - Lua ssdb client driver for the ngx_lua based on the cosocket API, SSDB is a leveldb server. 
* [lua-resty-fastdfs](https://github.com/azurewang) - Nonblocking Lua FastDFS driver library for ngx_lua.
* [lua-resty-mongol](https://github.com/Olivine-Labs/resty-mongol) - Lua MongoDB driver. 
* [lua-resty-oceanbase](https://github.com/hugozhu/lua-resty-oceanbase) - Lua OceanBase client driver for ngx_lua based on the cosocket API.
* [lua-resty-lrucache](https://github.com/openresty/lua-resty-lrucache) - Lua-land LRU Cache based on LuaJIT FFI. 
* [lua-resty-core](https://github.com/openresty/lua-resty-core) - New FFI-based API for lua-nginx-module. 
* [lua-resty-upload](https://github.com/openresty/lua-resty-upload) - Streaming reader and parser for http file uploading based on ngx_lua cosocket.
* [lua-resty-websocket](https://github.com/openresty/lua-resty-websocket) - WebSocket support for the ngx_lua module (and OpenResty). 
* [lua-resty-dns](https://github.com/openresty/lua-resty-dns) - DNS resolver for the nginx lua module.
* [lua-resty-string](https://github.com/openresty/lua-resty-string) - String utilities and common hash functions for ngx_lua and LuaJIT.
* [lua-redis-parser](https://github.com/openresty/lua-redis-parser) - Lua module for parsing raw redis responses. 
* [lua-rds-parser](https://github.com/openresty/lua-rds-parser) - Resty DBD Stream (RDS) parser for Lua written in C.
* [lua-resty-http](https://github.com/pintsized/lua-resty-http) - Lua HTTP client cosocket driver for OpenResty / ngx_lua. 
* [lua-resty-template](https://github.com/bungle/lua-resty-template) - Templating Engine (HTML) for Lua and OpenResty
* [lua-resty-cookie](https://github.com/cloudflare/lua-resty-cookie) - Lua library for HTTP cookie manipulations for OpenResty/ngx_lua. 
* [lua-resty-kafka](https://github.com/doujiang24/lua-resty-kafka) - Lua kafka client driver for the ngx_lua based on the cosocket API.
* [lua-resty-rabbitmqstomp](https://github.com/wingify/lua-resty-rabbitmqstomp) - Opinionated Lua RabbitMQ client library for the ngx_lua apps based on the cosocket API. 
* [lua-resty-logger-socket](https://github.com/cloudflare/lua-resty-logger-socket) - Raw-socket-based Logger Library for Nginx.
* [lua-resty-beanstalkd](https://github.com/smallfish/lua-resty-beanstalkd) - non-blocking beanstalkd client lib for ngx_lua. 
* [lua-resty-libcjson](https://github.com/bungle/lua-resty-libcjson) - LuaJIT FFI-based cJSON library for OpenResty. 
* [lua-resty-session](https://github.com/bungle/lua-resty-session) - Session library for OpenResty implementing Secure Cookie Protocol.
* [lua-resty-validation](https://github.com/bungle/lua-resty-validation) - Validation Library (Input Validation and Filtering) for Lua and OpenResty. 
* [lua-resty-random](https://github.com/bungle/lua-resty-random) - LuaJIT FFI-based Random Library for OpenResty.
* [lua-resty-scrypt](https://github.com/bungle/lua-resty-scrypt) - LuaJIT FFI-based scrypt library for OpenResty. 
* [lua-resty-uuid](https://github.com/bungle/lua-resty-uuid) - LuaJIT FFI bindings for libuuid, a DCE compatible Universally Unique Identifier library.
* [lua-resty-hoedown](https://github.com/bungle/lua-resty-hoedown) - LuaJIT FFI bindings to Hoedown, a standards compliant, fast, secure markdown processing library in C.
* [lua-resty-snappy](https://github.com/bungle/lua-resty-snappy) - LuaJIT FFI bindings for Snappy, a fast compressor/decompressor. 
* [lua-resty-nettle](https://github.com/bungle/lua-resty-nettle) - LuaJIT FFI bindings for Nettle (a low-level cryptographic library).
* [lua-resty-rack](https://github.com/pintsized/lua-resty-rack) - A simple and extensible HTTP server framework for OpenResty.
* [lua-resty-upstream](https://github.com/hamishforbes/lua-resty-upstream) - Upstream connection load balancing and failover module for Openresty.
* [lua-resty-dns-cache](https://github.com/hamishforbes/lua-resty-dns-cache) - Cache wrapper for lua-resty-dns. 
* [lua-resty-consul](https://github.com/hamishforbes/lua-resty-consul) - Library to interface with the consul HTTP API from ngx_lua.
* [lua-resty-gearman](https://github.com/zhhchen/lua-resty-gearman) - Lua gearman client driver for the ngx_lua based on the cosocket API.
* [lua-resty-jwt](https://github.com/SkyLothar/lua-resty-jwt) - JWT For The Great Openresty. 
* [lua-resty-shell](https://github.com/juce/lua-resty-shell) - tiny subprocess/shell library to use with OpenResty application server.
* [lua-resty-rsa](https://github.com/doujiang24/lua-resty-rsa) - RSA encrypt/decrypt & sign/verify for LuaJIT.
* [lua-resty-smtp](https://github.com/duhoobo/lua-resty-smtp) - I must be crazy trying to send mail with Nginx.. 
* [lua-resty-riak](https://github.com/bakins/lua-resty-riak) - Lua riak protocol buffer client driver for the ngx_lua based on the cosocket API.
* [lua-resty-iputils](https://github.com/bakins/lua-resty-riak) - Utility functions for working with IP addresses in Openresty. 
* [lua-resty-qless](https://github.com/pintsized/lua-resty-qless) - Lua binding to Qless (Queue / Pipeline management) for OpenResty.
* [lua-resty-hmac](https://github.com/jkeys089/lua-resty-hmac) - HMAC functions for ngx_lua and LuaJIT.
* [lua-resty-kyototycoon](https://github.com/cloudflare/lua-resty-kyototycoon) - Lua client driver for KyotoTycoon using its native wire protocol (OpenResty/ngx_lua).
* [lua-resty-libxl](https://github.com/bungle/lua-resty-libxl) - LuaJIT FFI-based LibXL (Excel) library for OpenResty.
* [lua-resty-gettext](https://github.com/bungle/lua-resty-gettext) - LuaJIT FFI-based gettext library for OpenResty.
* [lua-resty-github](https://github.com/jamesmarlowe/lua-resty-github) - Lua library for using the github api in the ngx_lua nginx module.
* [lua-resty-murmurhash2](https://github.com/bungle/lua-resty-murmurhash2) - LuaJIT MurmurHash 2 bindings to Nginx / OpenResty murmurhash2 implementation.
* [lua-resty-hipchat](https://github.com/jamesmarlowe/lua-resty-hipchat) - Lua library for using the hipchat api.
* [lua-resty-readurl](https://github.com/jamesmarlowe/lua-resty-readurl) - Lua library for capturing urls, decoding, and logging results.
* [lua-resty-kyototycoon](https://github.com/sjnam/lua-resty-kyototycoon) - kyototycoon's binary protocol.
* [lua-resty-mobile](https://github.com/isage/lua-resty-mobile) - Mobile detection for nginx/openresty.
* [lua-resty-fileinfo](https://github.com/bungle/lua-resty-fileinfo) - LuaJIT FFI bindings to libmagic, magic number recognition library - tries to determine file types.
* [lua-resty-sass](https://github.com/bungle/lua-resty-sass) - LuaJIT FFI bindings for libsass - A C/C++ implementation of a Sass compiler.
* [lua-resty-taglib](https://github.com/bungle/lua-resty-taglib) - LuaJIT FFI bindings for TagLib - An Audio Meta-Data Library.
* [lua-resty-woothee](https://github.com/woothee/lua-resty-woothee) - Woothee Lua-Openresty implementation.
* [lua-resty-json](https://github.com/cloudflare/lua-resty-json) - json lib for lua and C.
* [ngx_lua_waf](https://github.com/loveshell/ngx_lua_waf) - lua waf based on ngx_lua.
* [lua-resty-limit-req](https://github.com/timebug/lua-resty-limit-req) - Limit the request processing rate between multiple NGINX instances. 
* [LuaWeb](https://github.com/torhve/LuaWeb) - A very simple blog engine using openresty, nginx, lua, markdown, git and redis.
* [lua-nginx-osm](https://github.com/miurahr/lua-nginx-osm) - OpenStreetMap extension for Nginx Lua module. 
* [nginx-tcp-lua-module](https://github.com/bigplum/nginx-tcp-lua-module) - A TCP server with lua supporting based on nginx.
* [nginx-google-oauth](https://github.com/agoragames/nginx-google-oauth) - Lua module to add Google OAuth to nginx. 
* [lua-upstream-nginx-module](https://github.com/openresty/lua-upstream-nginx-module) - Nginx C module to expose Lua API to ngx_lua for Nginx upstreams.
* [lua-resty-upstream-healthcheck](https://github.com/openresty/lua-resty-upstream-healthcheck) - Health Checker for Nginx Upstream Servers in Pure Lua. 
* [lua-resty-lock](https://github.com/openresty/lua-resty-lock) - Simple nonblocking lock API for ngx_lua based on shared memory dictionaries. 


## Built-in Modules
For more details, see [nginx.org](http://nginx.org/en/docs/).

## Njs Projects
* [njs-types](https://npm.io/package/njs-types) - Provides type script type definitions for njs.
* [njs-examples](https://github.com/nginx/njs-examples) - Examples of njs usage.
* [nginx-njs-usecases](https://github.com/f5devcentral/nginx-njs-usecases) - A collection of njs use cases.
* [njs-acme](https://github.com/nginx/njs-acme) - ACME protocol implementation in njs allowing Let's Encrypt certificates to be issued directly from nginx.
* [nginx-s3-gateway](https://github.com/nginxinc/nginx-s3-gateway) - S3 gateway for Nginx allowing to proxy requests directly to S3 private buckets.
* [njs-memory-profiler](https://github.com/4141done/njs-memory-profiler) - Tool to understand per-request memory usage of njs scripts.
* [nginx-dns](https://github.com/TuxInvader/nginx-dns) - Example njs configuration for using Nginx with DNS services.
* [njs-prometheus-module](https://github.com/nginxinc/njs-prometheus-module) - Converts NGINX metrics exposed by the API module to a Prometheus format.
* [nginx-xml-json](https://github.com/lcrilly/nginx-xml-json) - Proof-of-concept solution for presenting XML services as a JSON API.
* [mqtt5](https://github.com/gallarda/mqtt5) - MQTT 5.0 protocol parser implemented in njs.
* [babel-preset-njs](https://github.com/jirutka/babel-preset-njs) - A Babel preset for njs - NGINX JavaScript.
* [njs-typescript-starter](https://github.com/jirutka/njs-typescript-starter) - A starting template for developing njs (NGINX JavaScript) scripts for NGINX server in TypeScript.

## Tools
* [nginx-devel-utils](https://github.com/openresty/nginx-devel-utils) - Utilities for nginx module development. 
* [gixy](https://github.com/yandex/gixy) - Nginx configuration static analyzer
* [no-pool-nginx](https://github.com/openresty/no-pool-nginx) - replace nginx's pool mechanism with plain malloc & free to help tools like valgrind. 
* [nginx-dtrace](https://github.com/openresty/nginx-dtrace) - An nginx fork that adds dtrace USDT probes. 
* [test-nginx](https://github.com/openresty/test-nginx) - Data-driven test scaffold for Nginx C module and OpenResty Lua library development. 
* [nginx-systemtap-toolkit](https://github.com/openresty/nginx-systemtap-toolkit) - Real-time analyzing and diagnosing tools for Nginx based on SystemTap. 
* [nginx-gdb-utils](https://github.com/openresty/nginx-gdb-utils) - GDB Utilities for Nginx, ngx_lua, LuaJIT, and etc. 
* [apache2nginx](https://github.com/nhnc-nginx/apache2nginx) - A command line tool, which can be used to generate nginx config file according to given config files of Apache. 
* [nginx-build](https://github.com/cubicdaiya/nginx-build) - seamless nginx builder. 
* [puppet-nginx](https://github.com/jfryman/puppet-nginx) - Puppet Module to manage NGINX on various UNIXes. 
* [server-configs-nginx](https://github.com/h5bp/server-configs-nginx) - Nginx HTTP server boilerplate configs. 
* [nginx-boilerplate](https://github.com/Umkus/nginx-boilerplate) - Awesome Nginx configuration template. 
* [ngxtop](https://github.com/lebinh/ngxtop) - Real-time metrics for nginx server. 
* [GoAccess](https://goaccess.io/) - real-time web log analyzer and interactive viewer that runs in a terminal in \*nix systems or through your browser. 
* [nginx-conf](https://github.com/lebinh/nginx-conf) - A collection of useful Nginx configuration snippets. 
* [libngxcore](https://github.com/cubicdaiya/libngxcore) - libngxcore is the library built from nginx core APIs.. 
* [nginx-cache-purge](https://github.com/perusio/nginx-cache-purge) - A bash script for deleting items from Nginx cache. 
* [ngx-admintools](https://github.com/rmacd/ngx-admintools) - Debian Administration Tools for nginx web server. 
* [nginx-config-formatter](https://github.com/slomkowski/nginx-config-formatter) - Nginx config file formatter/beautifier written in Python.
* [veryNginx](https://github.com/alexazhou/VeryNginx) - A very powerful and friendly nginx base on lua-nginx-module( openresty  ) which provide WAF, Control Panel, and Dashboards.
* [akamai-nginx](https://github.com/wyvern8/akamai-nginx) - Autoconfigure nginx based on Akamai property api rules using generated lua.
* [nginxconfig.io](https://nginxconfig.io) - [GitHub](https://github.com/valentinxxx/nginxconfig.io) - Online nginx configuration generator for general purposes.
* [nginx-opentracing](https://github.com/opentracing-contrib/nginx-opentracing) - NGINX plugin for OpenTracing.
* [nixy](https://github.com/martensson/nixy) - Nginx auto configuration and service discovery for Mesos/Marathon
* [build-nginx](https://github.com/jaygooby/build-nginx) - An nginx build tool to really simplify downloading and building specific versions of nginx with different core and 3rd-party modules.
* [nginx-autoinstall](https://github.com/angristan/nginx-autoinstall) - Compile Nginx from source with custom modules on Debian and Ubuntu
* [nginx-proxy-manager](https://github.com/jc21/nginx-proxy-manager) - Webinterface to manage nginx reverse-proxys with Letsencrypt support.
* [bunkerized-nginx](https://github.com/bunkerity/bunkerized-nginx) - nginx Docker image secure by default.
* [nginx-proxy](https://github.com/nginx-proxy/nginx-proxy) - Automated nginx proxy for Docker containers using docker-gen.
* [nginx-lua](https://github.com/fabiocicerchia/nginx-lua) - Nginx 1.19+ with LUA support based on Alpine Linux, Amazon Linux, CentOS, Debian, Fedora and Ubuntu.
* [nginx-testing](https://github.com/jirutka/nginx-testing) - Support for integration/acceptance testing of nginx configuration in TypeScript/JavaScript.
* [nginx-binaries](https://github.com/jirutka/nginx-binaries) - Nginx and njs binaries for Linux (x86_64, aarch64, ppc64le), macOS and Windows; Linux binaries are static so works on every Linux.

## Tutorials
* [Nginx admin guide](https://www.nginx.com/resources/admin-guide/) - Nginx and nginx plus admin guide. 
* [Nginx documentation](http://nginx.org/en/docs/) - Nginx documentation introduction. 
* [Nginx blog](https://www.nginx.com/blog/) - News, views, and how-tos from nginx. 
* [Nginx beginner’s Guide](http://nginx.org/en/docs/beginners_guide.html) - This guide gives a basic introduction to nginx and describes some simple tasks that can be done with it.
* [Nginx tutorials](https://github.com/openresty/nginx-tutorials) - Nginx tutorials by [Agentzh](https://github.com/agentzh). 
* [Nginx docs cn](https://github.com/taobao/nginx-docs-cn) - The chinese translation of nginx documentation. 
* [Nginx book](https://github.com/taobao/nginx-book) - Nginx from primer to expert (In Chinese).
* [Nginx module development](http://www.evanmiller.org/nginx-modules-guide.html) - Emiller's guide to nginx module development. 
* [OpenResty best practice](https://www.gitbook.com/book/moonbingbing/openresty-best-practices/details) - OpenResty best practice(In Chinese). 
* [Nginx-cheatsheet](https://github.com/SimulatedGREG/nginx-cheatsheet) - A quick reference to common server configurations from serving static files to using in congruency with Node.js applications.
* [Monitoring Nginx on Kubernetes](https://sysdig.com/blog/monitor-nginx-kubernetes/) - Deployment options, use cases, metrics and alerts for containerized Nginx instances on Kubernetes.

## Mailing Lists


* [Nginx Mailman](http://mailman.nginx.org/mailman/listinfo)




## Forum

* [Nginx Forum](http://forum.nginx.org/)
* [Nginx Community Slack](https://community.nginx.org/joinslack)
* [OpenResty Forum](http://groups.google.com/group/openresty-en)

## Active Developers
* [Maxim Dounin](https://twitter.com/mdounin)
* [Roman Arutyunyan](https://github.com/arut)
* Sergey Kandaurov
