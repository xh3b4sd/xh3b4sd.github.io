


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





## css

html {
  height: 100%;
}

.box {
  text-align: centre;
  margin: 100px auto;
  width: 500px;
  height: 100px;
  transform: translate(-50%, -50%);
  overflow: hidden;
  transition: .5s;
}

.box span {
  position: absolute;
  display: block;
}

.box span:nth-child(1) {
  top: 0;
  left: -100%;
  width: 100%;
  height: 1px;
  background: linear-gradient(90deg, transparent, #000);
  animation: btn-anim1 10s linear infinite;
}

@keyframes btn-anim1 {
  0% {
    left: -100%;
  }
  50%,100% {
    left: 100%;
  }
}

.box span:nth-child(2) {
  top: -100%;
  right: 0;
  width: 1px;
  height: 100%;
  background: linear-gradient(180deg, transparent, #000);
  animation: btn-anim2 10s linear infinite;
  animation-delay: 2.5s
}

@keyframes btn-anim2 {
  0% {
    top: -100%;
  }
  50%,100% {
    top: 100%;
  }
}

.box span:nth-child(3) {
  bottom: 0;
  right: -100%;
  width: 100%;
  height: 1px;
  background: linear-gradient(270deg, transparent, #000);
  animation: btn-anim3 10s linear infinite;
  animation-delay: 5s
}

@keyframes btn-anim3 {
  0% {
    right: -100%;
  }
  50%,100% {
    right: 100%;
  }
}

.box span:nth-child(4) {
  bottom: -100%;
  left: 0;
  width: 1px;
  height: 100%;
  background: linear-gradient(360deg, transparent, #000);
  animation: btn-anim4 10s linear infinite;
  animation-delay: 7.5s
}

@keyframes btn-anim4 {
  0% {
    bottom: -100%;
  }
  50%,100% {
    bottom: 100%;
  }
}


## html

<div class="box">
  <span></span>
  <span></span>
  <span></span>
  <span></span>
</div>
