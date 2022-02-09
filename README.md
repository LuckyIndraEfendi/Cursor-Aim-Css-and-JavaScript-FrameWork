
<h1> How To Use?</h1>

Letakkan Div yang mempunyai class cursor di awal saat pembuatan website cth :

```html 

  <body>
    <div class="cursor"></div>
  </body>

```


Buat Link CSS yang menuju ke arah Css kamu `application/config/database.php`.
```html
 <link rel="stylesheet" href="style.css" />
```

Konfigurasi Style CSS Kalian Seperti Di Bawah ini `application/config/database.php`.
```html
body {
  background: black;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.cursor {
  width: 30px;
  height: 30px;
  border-radius: 50%;
  border: 1px solid rgb(255, 255, 255);
  position: absolute;
  background-color: transparent;
  transition-duration: 200ms;
  transition-timing-function: ease-out;
  animation: cursorAnim 0.5s infinite alternate;
}
.cursor:after {
  content: "";
  width: 5px;
  height: 5px;
  position: absolute;
  border: 8px solid gray;
  opacity: 0.5;
  top: 3.5px;
  left: 3.5px;

  border-radius: 50%;
  animation: cursorAnim2 0.5s linear alternate;
}

@keyframes cursorAnim {
  from {
    transform: scale(1.3);
  }
  to {
    transform: scale(0.7);
  }
}
@keyframes cursorAnim2 {
  from {
    transform: scale(0);
  }
  to {
    transform: scale(1);
  }
}
```


Setelah Mengkonfigurasi HTML dan CSS, Langkah Berikutnya Salin Script JavaScript ke dalam JavaScript kamu

```html 
 <script src="script.js"></script>
```

Tempatkan Script Ini ke dalam file JavaScript kalian
```javascript 
const cursor = document.querySelector(".cursor");
document.addEventListener("mousemove", (e) => {
  console.log(e);
  cursor.setAttribute("style", "top : " + (e.pageY - 10) + "px; left: " + (e.pageX - 10) + "px");
});
```



<h1>Setelah Kalian Melakukan Seperti contoh yang diatas, kalian bisa melihat hasilnya seperti ini ⬇</h1>

Lihat Hasil =   (https://luckyindraefendi.github.io/Cursor-Aim-Css-and-JavaScript-FrameWork/)
