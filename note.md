  <!-- waves effect -->
  <svg class="editorial" style="z-index: 20000;"
      xmlns="http://www.w3.org/2000/svg"
      xmlns:xlink="http://www.w3.org/1999/xlink"
      viewBox="0 24 150 28 "
      preserveAspectRatio="none">
    <defs>
      <path id="gentle-wave"
      d="M-160 44c30 0 
      58-18 88-18s
      58 18 88 18 
      58-18 88-18 
      58 18 88 18
      v44h-352z" />
    </defs>
    <g class="parallax1">
      <use xlink:href="#gentle-wave" x="50" y="3" fill="rgba(32,32,54,.4)"/>
    </g>
    <g class="parallax2">
      <use xlink:href="#gentle-wave" x="50" y="0" fill="rgba(21,19,38,0.7)"/>
    </g>
    <g class="parallax3">
      <use xlink:href="#gentle-wave" x="50" y="9" fill="rgba(32,32,54,.8)"/>
    </g>
    <g class="parallax4" style="z-index:999999;">
      <use xlink:href="#gentle-wave" x="50" y="6" fill="#171621"/>  
    </g>
  </svg>
  
  -------------------------
  
  /* ----- Water Effect ----- */
.editorial {
    display: block;
    width: 100%;
    height: 60px;
    max-height: 60px;
    margin: 0;
    z-index:5;
    left:0px;
    float:left;
    }  
    .parallax1 > use {
        animation: move-forever1 10s linear infinite;
    }
    .parallax1:nth-child(1) {
        animation-delay: -2s;
    }
  
    .parallax2 > use {
        animation: move-forever2 8s linear infinite;
    }
    .parallax2:nth-child(1) {
        animation-delay: -2s;
    }
  
    .parallax3 > use {
        animation: move-forever3 6s linear infinite;
    }
    .parallax3:nth-child(1) {
        animation-delay: -2s;
    }  
    .parallax4 > use {
        animation: move-forever4 4s linear infinite;
    }
    .parallax4:nth-child(1) {
          animation-delay: -2s;
        }  
    @keyframes move-forever1 {
        0% {
            transform: translate(85px, 0%);
        }
        100% {
            transform: translate(-90px, 0%);
        }
        }
        @keyframes move-forever2 {
        0% {
            transform: translate(-90px, 0%);
        }
        100% {
            transform: translate(85px, 0%);
        }
        }
        @keyframes move-forever3 {
        0% {
            transform: translate(85px, 0%);
        }
        100% {
            transform: translate(-90px, 0%);
        }
        }
        @keyframes move-forever4 {
        0% {
            transform: translate(-90px, 0%);
        }
        100% {
            transform: translate(85px, 0%);
        }
    }


----------------------------------


/* ----- clouds animation ----- */

/* <div class="x1">
<div class="cloud"></div>
</div>
 */
@-webkit-keyframes animateCloud {
    0% {
        margin-left: -1000px;
    }
    100% {
        margin-left: 100%;
    }
}
@-moz-keyframes animateCloud {
    0% {
        margin-left: -1000px;
    }
    100% {
        margin-left: 100%;
    }
}
@keyframes animateCloud {
    0% {
        margin-left: -1000px;
    }
    100% {
        margin-left: 100%;
    }
}
.x1 {
	-webkit-animation: animateCloud 35s linear infinite;
	-moz-animation: animateCloud 35s linear infinite;
	animation: animateCloud 35s linear infinite;
	
	-webkit-transform: scale(0.65);
	-moz-transform: scale(0.65);
	transform: scale(0.65);
}
.x2 {
	-webkit-animation: animateCloud 20s linear infinite;
	-moz-animation: animateCloud 20s linear infinite;
	animation: animateCloud 20s linear infinite;
	
	-webkit-transform: scale(0.3);
	-moz-transform: scale(0.3);
	transform: scale(0.3);
}
.x3 {
	-webkit-animation: animateCloud 30s linear infinite;
	-moz-animation: animateCloud 30s linear infinite;
	animation: animateCloud 30s linear infinite;
	
	-webkit-transform: scale(0.5);
	-moz-transform: scale(0.5);
	transform: scale(0.5);
}
.x4 {
	-webkit-animation: animateCloud 18s linear infinite;
	-moz-animation: animateCloud 18s linear infinite;
	animation: animateCloud 18s linear infinite;
	
	-webkit-transform: scale(0.4);
	-moz-transform: scale(0.4);
	transform: scale(0.4);
}
.x5 {
	-webkit-animation: animateCloud 25s linear infinite;
	-moz-animation: animateCloud 25s linear infinite;
	animation: animateCloud 25s linear infinite;
	
	-webkit-transform: scale(0.55);
	-moz-transform: scale(0.55);
	transform: scale(0.55);
}
.cloud {
	background: #fff;
	background: -moz-linear-gradient(top,  #fff 5%, #f1f1f1 100%);
	background: -webkit-gradient(linear, left top, left bottom, color-stop(5%,#fff), color-stop(100%,#f1f1f1));
	background: -webkit-linear-gradient(top,  #fff 5%,#f1f1f1 100%);
	background: -o-linear-gradient(top,  #fff 5%,#f1f1f1 100%);
	background: -ms-linear-gradient(top,  #fff 5%,#f1f1f1 100%);
	background: linear-gradient(top,  #fff 5%,#f1f1f1 100%);
	filter: progid:DXImageTransform.Microsoft.gradient( startColorstr='#fff', endColorstr='#f1f1f1',GradientType=0 );	
	-webkit-border-radius: 100px;
	-moz-border-radius: 100px;
	border-radius: 100px;	
	-webkit-box-shadow: 0 8px 5px rgba(0, 0, 0, 0.1);
	-moz-box-shadow: 0 8px 5px rgba(0, 0, 0, 0.1);
	box-shadow: 0 8px 5px rgba(0, 0, 0, 0.1);
	height: 120px;
	position: relative;
	width: 350px;
}
.cloud:after, .cloud:before {
    background: #fff;
	content: '';
	position: absolute;
	z-indeX: -1;
}
.cloud:after {
	-webkit-border-radius: 100px;
	-moz-border-radius: 100px;
	border-radius: 100px;
	height: 100px;
	left: 50px;
	top: -50px;
	width: 100px;
}
.cloud:before {
	-webkit-border-radius: 200px;
	-moz-border-radius: 200px;
	border-radius: 200px;
	width: 180px;
	height: 180px;
	right: 50px;
	top: -90px;
}
