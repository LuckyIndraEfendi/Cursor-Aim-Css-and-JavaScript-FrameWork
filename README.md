
<h1> How To Use?</h1>

Buat Link CSS yang menuju ke arah Css kamu `application/config/database.php`.
```html
 <link rel="stylesheet" href="style.css" />
```

Letakkan Div yang mempunyai class cursor di awal saat pembuatan website cth : `application/config/database.php`.

```html 

  <body>
    <div class="cursor"></div>
  </body>

```

Setelah Mengkonfigurasi HTML dan CSS, Langkah Berikutnya Salin Script JavaScript ke dalam JavaScript kamu

```html 
 <script src="script.js"></script>
```

Tempatkan Script JavaScript ke dalam file JavaScript kalian
```javascript 
const cursor = document.querySelector(".cursor");
document.addEventListener("mousemove", (e) => {
  console.log(e);
  cursor.setAttribute("style", "top : " + (e.pageY - 10) + "px; left: " + (e.pageX - 10) + "px");
});
```
