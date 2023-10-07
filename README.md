[한국어 리드미](https://github.com/HOOOO98/Awesome-DND/tree/main/KR#readme)
# ✨Awesome-DND
Practicing grid-based drag and drop functionality.
<br>
<br>
# 👀Preview
![ezgif-5-862bac119c](https://github.com/HOOOO98/Awesome-DND/assets/120024673/40cd7223-eeab-4a4c-9c52-ac3158b6ddf9)
<br>
<br>
<br>
<br>

# 🤔Description
Were you looking for a drag-and-drop of grid layout?<br>
If so, you can try the muri library exactly.
<br>
<br>
<br>
<br>

# 👉Following Step1 : create index.html file
Create idex.html file in root directory.<br>
<br>
and use `!` emment to create initial HTML setting<br>
<br>
![스크린샷 2023-10-07 213608](https://github.com/HOOOO98/Awesome-DND/assets/120024673/f855df38-5478-45ec-a64a-fe25c361e6ed)
<br>
<br>
and press `enter`<br>
<br>
![스크린샷 2023-10-07 213734](https://github.com/HOOOO98/Awesome-DND/assets/120024673/0f4700d1-62fa-4d24-bfaa-c5574a15eca6)
<br>
<br>
<br>
<br>

# 👉Following Step2 : import script cdn on index.html
```
<script src="https://cdn.jsdelivr.net/npm/web-animations-js@2.3.2/web-animations.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/muuri@0.9.5/dist/muuri.min.js"></script>
```
<br>
Paste at the bottom of the body tag.
<br>
<br>

![스크린샷 2023-10-07 214337](https://github.com/HOOOO98/Awesome-DND/assets/120024673/87160ae6-a05a-4a1c-bb36-90f25fd47143)

<br>
<br>
<br>
<br>

# 👉Following Step3 : make items
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

# 👉Following Step4 : set the muuri function Options.
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
If you want more Options? then take a look below link.👇 <br>
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
Paste at the bottom of the body tag.
<br>
<br>

![스크린샷 2023-10-07 215849](https://github.com/HOOOO98/Awesome-DND/assets/120024673/7e0e0871-e598-4e9c-9b56-4442957613da)
<br>
<br>
<br>
<br>


# 👉Following Step5 : paste style.css
Create `style.css` file on root directory.<br>
and copy the code below.
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

Then link your `style.css` file to `index.html` file. 

<br>
<br>

![스크린샷 2023-10-07 220246](https://github.com/HOOOO98/Awesome-DND/assets/120024673/770b4546-5bc9-4aac-b9a9-860d051af073)
<br>
<br>
<br>
<br>

# 🔥Final Step : run your files
Right-click and then click `Open with Live Server` (do it in index.html file) 
<br>
<br>

![스크린샷 2023-10-07 220419](https://github.com/HOOOO98/Awesome-DND/assets/120024673/24bc51e9-23d5-47d5-902c-db2559ab81db)
<br>
<br>
<br>
<br>

## ℹ️If you can't see the live server?
Install it at the marketplace first
<br>
<br>

![스크린샷 2023-10-07 220910](https://github.com/HOOOO98/Awesome-DND/assets/120024673/49dab23e-c9cd-4c87-bbf1-2939dc068610)

<br>
<br>
<br>
<br>

# Reference
- How can I make it? : https://www.youtube.com/watch?v=PDG-GqmUZss&t=43s
- What library did I use? : https://github.com/haltu/muuri
- How can I get moving icons? : https://lordicon.com/
