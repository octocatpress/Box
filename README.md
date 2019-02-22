<!DOCTYPE html>
<html lang="zh-CN"><head>
  <meta http-equiv="content-type" content="text/html; charset=UTF-8">
      <meta charset="utf-8">
  	<meta name="viewport" content="width=device-width, initial-scale=1, user-scalable=no">

  	<title>BigCoke's Lab</title>
    </head>
    <body>
        <style type="text/css">
  .jar_loading {
  	position: relative;
  	z-index: 1;
  }
  .jar_loading_body {
  	color: #ccc;
  	padding: 0;
  	margin: 0;
  	text-align: center;
  }
  .jar_loading_body * {
  	box-sizing: border-box;
  	-moz-box-sizing: border-box;
  	-webkit-box-sizing: border-box;
  }
  .jar_loading_box {
  	position: relative;
  	width: 200px;
  	margin: 100px auto 0;
  	text-align: center;
  	padding-top: 40px;
  }
  .jar_loading_bg {
  	background-image: url('data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFoAAABwCAMAAACpQZdgAAAA1VBMVEX///8AAADJycrk5eXw8PDJycr////Jysvp6enJycrLzMz09PX+/v7Ky8vU1dXJycrJycrNzs7Oz8/Q0NHJycrJycrJycrJysvMzM3JycrR0tLJycrV1dbJycrJycrJycrJycr5+fnJycrb29zJycrJycrS0tPJycrJycrJysvNzc7JycrJycrJycrJycrc3d3e3t/g4eHi4+Pt7e74+PjJycrQ0dHx8fH7+/vJycrJycrW1tfJycrX2NjZ2drJycrJycrJycrJycrJycrJycr8/PzJyco2DXaRAAAARnRSTlNNAEB6Y2A7+nDy8VxP6rMaLdrTzMtqCfbl08GwrocD3ZFVw5YUDrxaNfze2rqpo5GNhX5oViPFYVNT1qh1pJxHoJp8eE8/Zpw4YwAAA7JJREFUaN7t2edy2kAUQOEVdqKGkASS6Jjee3FPT877P1KQcWLHFqZoPfnDeYBvmDu7M+yVUN7uRnd/fXydyFkJZUc76C89MMXrNMg68eg8vamI6jMUY9E2lER0l6iVOLQDky30J2jFoZvQ3kKn0ePNuk5vHilPYByPTrD1hKhOPFopghZBT6GsxKQ/wHkEfQaJE32iT/SJPtEn+kSf6BN9ov8bXUkUo+k5jBOVo+ngZpSF6P/XDYDs6CY4hna+6YRl0yKiazdLmP7NOZT+WQfoZRoLsa1FI9MDqP88hP7iAbgNU7yd2XABvC/70k4dUNua2CetrQJ1Zx86KKvQS5li38xUD9RysJPuDoDClTikqwIw6O6g71XInYlDO8uBev8WHYyA0rU4vOsUMAq20rYHxlwc19wAz95C2xfQvxLHdtWHCzuSDuVMTRxfLRPaEXRzLReSIk7JwtpuvqKD+kaObdeDl/QIMms5rp2B0Qvah/5SxG/ZB/8f2sliXAkZnRtknWd0xYOZkNMMvMoT7UNbyKoN/l+6aWGY0mjTwGr+ocvQEPJqQPmRbunkhMxy6K0NfQ8TqfQE7jf0ACsplU5aDB7oLtwJud1BN6SrsJBML6Aa0rf0hez63K5pG0rS6RLYiujAXDo9h44iyrCUTi+hrIgihpCfQVERedJCfmnyirBoC/kVsBSRJSXklyKrCCgJ+ZXgfel3GsiatigI+RWw3vXwFdGF/HSKDxfdlC6bDxf9BmbS6RncKMJ+jyOSAlsRSp6cdDpHXlnTZdAkyxqUQ7oLKfnz6Ia0kidbkyrXsuSVB9qHz1Lpz+Bv6MDCuJYoXxtYwYZWfsAnifQn+KE80kEO9VyafK6SCzb0us7TG0nKS6nz7C0zhIa8f9dD5Rm90lE1ObdFRV890ZuRWKYE2bSg8+JJWgW3Fv+yuFBVXtCVIaRrceU0DCsvaaXlhXZs2WtFLC2aeXDNOHN2Id+MXLU0PbC048+GBd5ajqKV1hDUyZHyRIVha+taq1IFLs1jhnEJVCtvLeM6OhjT5KGXe2qA3tmxQlzVgbR22JTTQH21c/FZ8XXgUtsfvgR0v7LPutYeA2RmyX1GMcsAjO19l8xOEcC4W+yAF3cGQNE5ZDXujFWAXOksue33npVyAOrYOXShb38fEKa6qam2/EddatOUqxI2+G4f9YWjW73gMcPNFNqpUqpdyLgGj11UuzG+y6z8r7dEdfvVX8X85LOulfCrRe9CJ0y/8IpVP9FSdvcbhjbR7CHfGkMAAAAASUVORK5CYII=');
  	background-position: bottom center;
  	background-repeat: no-repeat;
  	position: absolute;
  	left: 0;
  	right: 0;
  	top: 0;
  	bottom: 0;
  	z-index: 2;
  }
  .jar_loading .bubble_loading {
  	width: 10px;
  	height: 10px;
  	position: absolute;
  	background-color: #35EEFB;
  	opacity: 0.4;
  	left: 92px;
  	z-index: 8;
  	top: 40px;
  	-moz-border-radius: 100%;
  	-webkit-border-radius: 100%;
  	border-radius: 100%;
  	-moz-animation: buble 2s linear 1s infinite;
  	-webkit-animation: buble 2s linear 1s infinite;
  	animation: buble 2s linear 1s infinite;
  }
  .jar_loading .bubble_loading + .bubble_loading {
  	left: 90px;
  	top: 42px;
  	width: 15px;
  	height: 15px;
  	-moz-animation-duration: 3s;
  	-webkit-animation-duration: 3s;
  	animation-duration: 3s;
  }
  .jar_loading .base_loading {
  	margin: auto;
  	width: 90px;
  	height: 72px;
  	-moz-border-radius: 50%;
  	-webkit-border-radius: 50%;
  	border-radius: 50%;
  	overflow: hidden;
  	position: relative;
  	z-index: 5;
  	border: 2px solid rgba(255,255,255,0);
  }
  .jar_loading .base_loading .bubble_loading {
  	left: 15px;
  	top: 40px;
  	-moz-animation: bounce 2.3s linear 0s infinite alternate;
  	-webkit-animation: bounce 2.3s linear 0s infinite alternate;
  	animation: bounce 2.3s linear 0s infinite alternate;
  }
  .jar_loading .base_loading .bubble_loading + .bubble_loading {
  	left: 64px;
  	top: 40px;
  	-moz-animation-duration: 3s;
  	-webkit-animation-duration: 3s;
  	animation-duration: 3s;
  }
  .jar_loading .liquid_loading {
  	height: 30px;
  	background-color: #35EEFB;
  	position: absolute;
  	bottom: 0;
  	left: 0;
  	right: 0;
  }
  .jar_loading .wave_loading {
  	width: 60px;
  	height: 20px;
  	position: absolute;
  	background-color: #35EEFB;
  	left: 0;
  	top: 37px;
  	-moz-animation: wave 1s linear infinite alternate;
  	-webkit-animation: wave 1s linear infinite alternate;
  	animation: wave 1s linear infinite alternate;
  	-moz-border-radius: 50%;
  	-webkit-border-radius: 50%;
  	border-radius: 50%;
  }
  .jar_loading .wave_loading + .wave_loading {
  	left: auto;
  	right: 0;
  }
  .jar_loading_text {
  	margin: 8px 0;
  }
   @-moz-keyframes wave {
   from {
   -moz-transform: translateX(100px);
   transform: translateX(100px);
  }
   to {
   -moz-transform: translateX(-100px);
   transform: translateX(-100px);
  }
  }
  @-webkit-keyframes wave {
   from {
   -webkit-transform: translateX(100px);
   transform: translateX(100px);
  }
   to {
   -webkit-transform: translateX(-100px);
   transform: translateX(-100px);
  }
  }
  @keyframes wave {
   from {
   -moz-transform: translateX(100px);
   -ms-transform: translateX(100px);
   -webkit-transform: translateX(100px);
   transform: translateX(100px);
  }
   to {
   -moz-transform: translateX(-100px);
   -ms-transform: translateX(-100px);
   -webkit-transform: translateX(-100px);
   transform: translateX(-100px);
  }
  }
  @-moz-keyframes bounce {
   0% {
   -moz-transform: translate(5px, 15px);
   transform: translate(5px, 15px);
  }
   50% {
   -moz-transform: translate(0, -15px);
   transform: translate(0, -15px);
  }
   100% {
   -moz-transform: translate(-5px, -31px);
   transform: translate(-5px, -31px);
   opacity: 1;
  }
  }
  @-webkit-keyframes bounce {
   0% {
   -webkit-transform: translate(5px, 15px);
   transform: translate(5px, 15px);
  }
   50% {
   -webkit-transform: translate(0, -15px);
   transform: translate(0, -15px);
  }
   100% {
   -webkit-transform: translate(-5px, -31px);
   transform: translate(-5px, -31px);
   opacity: 1;
  }
  }
  @keyframes bounce {
   0% {
   -moz-transform: translate(5px, 15px);
   -ms-transform: translate(5px, 15px);
   -webkit-transform: translate(5px, 15px);
   transform: translate(5px, 15px);
  }
   50% {
   -moz-transform: translate(0, -15px);
   -ms-transform: translate(0, -15px);
   -webkit-transform: translate(0, -15px);
   transform: translate(0, -15px);
  }
   100% {
   -moz-transform: translate(-5px, -31px);
   -ms-transform: translate(-5px, -31px);
   -webkit-transform: translate(-5px, -31px);
   transform: translate(-5px, -31px);
   opacity: 1;
  }
  }
  @-moz-keyframes buble {
   0% {
   -moz-transform: translate(3px, 10px);
   transform: translate(3px, 10px);
  }
   25% {
   -moz-transform: translate(0, 0px);
   transform: translate(0, 0px);
  }
   50% {
   -moz-transform: translate(-1px, -25px);
   transform: translate(-3px, -25px);
  }
   75% {
   -moz-transform: translate(0, -50px);
   transform: translate(0, -50px);
   opacity: 1;
  }
   100% {
   -moz-transform: translate(3px, -100px);
   transform: translate(3px, -100px);
   opacity: 0;
  }
  }
  @-webkit-keyframes buble {
   0% {
   -webkit-transform: translate(3px, 10px);
   transform: translate(3px, 10px);
  }
   25% {
   -webkit-transform: translate(0, 0px);
   transform: translate(0, 0px);
  }
   50% {
   -webkit-transform: translate(-3px, -25px);
   transform: translate(-3px, -25px);
  }
   75% {
   -webkit-transform: translate(0, -50px);
   transform: translate(0, -50px);
   opacity: 1;
  }
   100% {
   -moz-transform: translate(3px, -100px);
   -ms-transform: translate(3px, -100px);
   -webkit-transform: translate(3px, -100px);
   transform: translate(3px, -100px);
   opacity: 0;
  }
  }
  @keyframes buble {
   0% {
   -moz-transform: translate(3px, 10px);
   -ms-transform: translate(3px, 10px);
   -webkit-transform: translate(3px, 10px);
   transform: translate(3px, 10px);
  }
   25% {
   -moz-transform: translate(0, 0px);
   -ms-transform: translate(0, 0px);
   -webkit-transform: translate(0, 0px);
   transform: translate(0, 0px);
  }
   50% {
   -moz-transform: translate(-1px, -25px);
   -ms-transform: translate(-1px, -25px);
   -webkit-transform: translate(-3px, -25px);
   transform: translate(-3px, -25px);
  }
   75% {
   -moz-transform: translate(0, -50px);
   -ms-transform: translate(0, -50px);
   -webkit-transform: translate(0, -50px);
   transform: translate(0, -50px);
   opacity: 1;
  }
   100% {
   -moz-transform: translate(3px, -100px);
   -ms-transform: translate(3px, -100px);
   -webkit-transform: translate(3px, -100px);
   transform: translate(3px, -100px);
   opacity: 0;
  }
      </style>

  		<div class="jar_loading_body">
      <div class="jar_loading_box">
      	<div class="jar_loading_bg"></div>
          <div class="jar_loading">
            <div class="base_loading">
              <div class="liquid_loading"> </div>
              <div class="wave_loading"></div>
              <div class="wave_loading"></div>
              <div class="bubble_loading"></div>
              <div class="bubble_loading"></div>
            </div>
            <div class="bubble_loading"></div>
            <div class="bubble_loading"></div>
          </div>
      </div>
      <p class="jar_loading_text">更多内容努力炼制中······</p>
     </div>
  </body><style type="text/css"></style></html>
