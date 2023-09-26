ab
===

Apache server performance testing tool




### Options

```shell
-A auth-username:password
       # Support basic authentication certificates, use "colon" between username and password:
       # Separated, ab will be sent in clear text. Regardless of whether the server needs it or not
       # , which means your server needs to support 401 authentication.

-c concurrency
       # The number of requests sent to the server at the same time. By default, only one http request is executed at a time.
```



### Example

```shell
# 10 concurrency, 500 requests
ab -c 10 -n 500 https://www.qq.com/
```