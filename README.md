# CLUDOS_APPDEV
클루도스 어플리케이션 개발문서

# 소개
클루도스 앱 위치는 ./views/apps 에 존재합니다.  
app_(이름).ejs 로 구성됩니다.  

# 구성 
<%= uid%> : 사용자 명  
<%= sid%> : 식별 넘버  

```js
<div id="popup_window_(앱 번호)" width="190" class="card card11" style="position:absolute; z-index: 8970; left:0px; top:50px; cursor:pointer; cursor:hand; " onmousedown="startDrag(event, this)" border="0">
  <div class="card-content bg-light">
    <div class="card-header">
      <b class="card-title">(앱 제목)</b>
      <button type="button" class="close" onclick="Window_c_click((앱 번호));"><div class="circle1"></div></button>
      <button type="button" class="close" onclick="fullScreen((앱 번호))"><div class="circle2"></div></button>
      <button type="button" class="close" onclick="nomove((앱 번호))"><div class="circle3"></div></button>
    </div>
    <div class="card-body">
      <p><%= uid%> 님 환영합니다.</p>

    </div>
  </div>
</div>
```

# 예시
```js
<div id="popup_window_2" width="190" class="card card11" style="position:absolute; z-index: 8970; left:0px; top:50px; cursor:pointer; cursor:hand; " onmousedown="startDrag(event, this)" border="0">
  <div class="card-content bg-light">
    <div class="card-header">
      <b class="card-title">CLUDOS 설정</b>
      <button type="button" class="close" onclick="Window_c_click(2);"><div class="circle1"></div></button>
      <button type="button" class="close" onclick="fullScreen(2)"><div class="circle2"></div></button>
      <button type="button" class="close" onclick="nomove(2)"><div class="circle3"></div></button>


    </div>
    <div class="card-body">
      <p><%= uid%> 님 환영합니다.</p>
    </div>
  </div>
</div>



<script src="./js/dark-mode-switch.min.js"></script>
```

# 임시 앱 배포
./views/index.ejs 에 window_first 함수에서  
```js
    var array = [2,3,4,5,6,7,9,10,12]+count;
```
배열에 앱 번호를 입력합니다  

# 앱 번호
노션 참고  

