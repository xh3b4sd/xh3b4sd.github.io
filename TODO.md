


https://github.com/google/fonts/issues/473#issuecomment-458549555

```
curl -s -A "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_3) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/71.0.3578.98 Safari/537.36" https://fonts.googleapis.com/css\?family\=Cutive+Mono | openssl dgst -sha512 -binary | openssl base64 -A | xargs -I {} echo 'sha512-'{}
```

```
curl -s -A "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/60.0.3112.113 Safari/537.36" https://fonts.googleapis.com/css\?family\=Cutive+Mono | openssl dgst -sha512 -binary | openssl base64 -A | xargs -I {} echo 'sha512-'{}
```



https://stackoverflow.com/questions/2504071/how-do-i-combine-a-background-image-and-css3-gradient-on-the-same-element
https://stackoverflow.com/a/56423619/3479043

https://codepen.io/tkmoney/pen/jKKWEN
https://codepen.io/StephenScaff/pen/oLBqmw
