# ✨Awesome-DND
드래그 앤 드랍을 연습해 볼 수 있습니다.
<br>
<br>
# 👀미리보기
![ezgif-5-862bac119c](https://github.com/HOOOO98/Awesome-DND/assets/120024673/40cd7223-eeab-4a4c-9c52-ac3158b6ddf9)
<br>
<br>
<br>
<br>

# 🤔프로젝트 설명
그리드 형식이면서... 드래그 앤 드랍을 할 수 있는 라이브러리를 찾고 계신가요?<br>
그렇다면 정확히 잘 찾아오셨습니다!
<br>
<br>
<br>
<br>

# 👉첫번째 단계 : index.html 파일을 만듭니다.
idex.html를 프로젝트 폴더에 만듭니다.<br>
<br>
`!` emment 를 사용해서 html을 빠르게 채웁니다.<br>
<br>
![스크린샷 2023-10-07 213608](https://github.com/HOOOO98/Awesome-DND/assets/120024673/f855df38-5478-45ec-a64a-fe25c361e6ed)
<br>
<br>
`enter`키를 누릅니다.<br>
<br>
![스크린샷 2023-10-07 213734](https://github.com/HOOOO98/Awesome-DND/assets/120024673/0f4700d1-62fa-4d24-bfaa-c5574a15eca6)
<br>
<br>
<br>
<br>

# 👉두번째 단계 :  script cdn 을 index.html 에 가져옵니다.
```
<script src="https://cdn.jsdelivr.net/npm/web-animations-js@2.3.2/web-animations.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/muuri@0.9.5/dist/muuri.min.js"></script>
```
<br>
바디 태그의 가장 밑에 붙여넣습니다.
<br>
<br>

![스크린샷 2023-10-07 214337](https://github.com/HOOOO98/Awesome-DND/assets/120024673/87160ae6-a05a-4a1c-bb36-90f25fd47143)

<br>
<br>
<br>
<br>

# 👉세번째 단계 : items 만들기
```
<div class="grid">
    <div class="item">
      <div class="item-content">
        {put your item here}
      </div>
    </div>
    <div class="item">
      <div class="item-content">
        something one
      </div>
    </div>
    <div class="item">
      <div class="item-content">
        something two
      </div>
    </div>

    ...

    <div class="item">
      <div class="item-content">
        something end
      </div>
    </div>
<div>
```
![스크린샷 2023-10-07 214850](https://github.com/HOOOO98/Awesome-DND/assets/120024673/1d185072-4272-4576-b1c9-456233792c7a)
<br>
<br>
<br>
<br>

# 👉네번째 단계 :  muuri function의 옵션을 작성해줍니다.
(items,
showDuration,
showEasing,
hideDuration,
hideEasing,
visibleStyles,
hiddenStyles,
...
)<br>
<br>
만약 더 많은 옵션에 대해 알고 싶다면? 아래의 링크에서 읽어보세요.👇 <br>
https://github.com/haltu/muuri#grid-options
<br>
<br>
```
<script>
    const grid = new Muuri('.grid', {
      dragEnabled: true
    });
  </script>
```
<br>
바디태그 속 가장 밑에 붙여넣습니다.
<br>
<br>

![스크린샷 2023-10-07 215849](https://github.com/HOOOO98/Awesome-DND/assets/120024673/7e0e0871-e598-4e9c-9b56-4442957613da)
<br>
<br>
<br>
<br>


# 👉다섯번째 단계 : style.css 파일 복사 붙여넣기
우선 `style.css` file을 프로젝트 폴더에 만듭니다.<br>
그리고 아래의 코드를 붙여넣습니다..
```
body {
  font-family: Arial, Helvetica, sans-serif;
  background-color: #fcfaf9;
}

.grid {
  position: relative;
}

.item {
  display: block;
  position: absolute;
  height: 200px;
  width: 200px;
  line-height: 200px;
  margin: 5px;
  text-align: center;
  z-index: 1;
}

.item.muuri-item-dragging {
  z-index: 3;
}
.item.muuri-item-releasing {
  z-index: 2;
}
.item.muuri-item-hidden {
  z-index: 0;
}

.item-content {
  position: relative;
  width: 100%;
  height: 100%;
  cursor: pointer;
  color: #fff;
  background-color: #59687d;
  font-size: 40px;
  text-align: center;
}

.item.muuri-item-dragging .item-content {
  background: #8993a2;
}
.item.muuri-item-releasing .item-content {
  background: #152c43;
}
```
<br>
<br>

그리고 `style.css` file을 `index.html` 와 연결시켜줍니다. 

<br>
<br>

![스크린샷 2023-10-07 220246](https://github.com/HOOOO98/Awesome-DND/assets/120024673/770b4546-5bc9-4aac-b9a9-860d051af073)
<br>
<br>
<br>
<br>

#기
오른쪽 클릭을 한 뒤, `Open with Live Server`를 클릭해줍니다. ( index.html file 안에서 해야 합니다.) 
<br>
<br>

![스크린샷 2023-10-07 220419](https://github.com/HOOOO98/Awesome-DND/assets/120024673/24bc51e9-23d5-47d5-902c-db2559ab81db)
<br>
<br>
<br>
<br>

## ℹ️live server가 안보이시나요?
먼저 마켓 플레이스에서 프로그램을 다운 받아야 합니다.
<br>
<br>

![스크린샷 2023-10-07 220910](https://github.com/HOOOO98/Awesome-DND/assets/120024673/49dab23e-c9cd-4c87-bbf1-2939dc068610)

<br>
<br>
<br>
<br>

# 참고자료
- 더 자세한 만드는 과정 : https://www.youtube.com/watch?v=PDG-GqmUZss&t=43s
- 사용한 라이브러리 : https://github.com/haltu/muuri
- 움직이는 아이콘 : https://lordicon.com/
