# css3BatteryCharging
css3实现电池充电效果

[Demo -- 演示页面](http://unclehking.github.io/css3BatteryCharging/)

css:
```java  
.battery{margin: 50px auto;width:200px;height: 96px;border: solid #4a4a4a 10px;border-radius: 10px;position: relative;transform:rotate(-90deg);}
.battery.horizon{transform:rotate(0deg);}
.battery svg{position: relative;top: -30%;left: 10%;fill: #4a4a4a;transform:rotate(90deg);width: 80%;}
.battery:after{display: block;content: " ";width: 24px;height: 50%;background-color: #4a4a4a;position: absolute;right: -24px;top: 25%;border-radius: 0 4px 4px 0;}
.battery:before{display: block;content: " ";width: 0%;height: 100%;background-color: #ff0000;position: absolute;animation: charging 3s infinite;}
@keyframes charging{
    0%{background-color: #ff0000;}
    30%{background-color: #ffa200;}
    100%{background-color: #00ff00;width: 100%;}
}
```

html:
```java  
<div class="battery horizon">
  <svg version="1.1" x="0px" y="0px"  viewBox="0 0 100 100" style="enable-background:new 0 0 100 100;" xml:space="preserve">
      <g>
      	<path  d="M37.965,96.277c0,0,31.768-68.942,31.772-68.952l1.763-3.921c-6.834,1.964-22.103,5.703-22.152,5.855c1.597-4.469,8.469-24.537,8.765-24.537c-6.532,0-13.064,0-19.596,0l-1.988,9.467l-8.362,34.313l22.09-6.014L37.965,96.277z"/>
      </g>
  </svg>
</div>
```
