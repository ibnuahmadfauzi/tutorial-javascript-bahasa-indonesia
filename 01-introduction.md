# 01 - Introduction

**JavaScript** adalah bahasa pemrograman untuk web, digunakan untuk memanpulasi halaman web bekerja bersama HTML dan CSS.

Pada awalnya bahasa ini hanya digunakan untuk pemrograman web di sisi client. Seiring berkembangnya teknologi dan dengan munculnya **NodeJS**, sekarang JavaScript bisa digunakan untuk berbagai macam kebutuhan, seperti: pengembangan aplikasi mobile, desktop, IoT, server, game, dll.

Kode JavaScript biasanya ditempatkan di dalam tag

```javascript
<script>
    . . .
</script>.
```

Cotohnya:

```javascript
<script>
  document.getElementById("demo").innerHTML = "My First JavaScript";
</script>
```

Pada kode JavaScript lama, elemen `<script>` membutuhkan atribut `type="text/javascript"`. Atribut `type=" "` sekarang tidak wajib digunakan.

Elemen `<script> . . . </script>` bisa di tempatkan di dalam `<head>` atau sebelum penutup `</body>`. Namun sangat di sarankan untuk ditempatkan sebelum penutup `</body>` karena nanti efeknya akan sangat terasa ketika sudah belajar di **Document Object Model (DOM)**.

Contohnya:

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Belajar JavaScript</title>
  </head>
  <body>
    <h1 id="judul"></h1>

    <button onclick="myFunction()">Klik Disini</button>

    <script>
      function myFunction() {
        document.getElementById("judul").innerText = "Belajar JavaScript!";
      }
    </script>
  </body>
</html>
```

Selain itu bisa juga menempatkan kode JavaScript ke file terpisah dengan ekstensi **.js**

Contohnya saya buat file JavaScript dengan nama **script.js** lalu saya masukkan kode JavaScript ke dalam file tersebut:

```javascript
function myFunction() {
  document.getElementById("judul").innerText = "Belajar JavaScript!";
}
```

Dengan begitu isi file **index.html** saya jadi seperti ini:

```html
<!doctype html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Belajar JavaScript</title>
  </head>
  <body>
    <h1 id="judul"></h1>

    <button onclick="myFunction()">Klik Disini</button>

    <script src="script.js"></script>
  </body>
</html>
```

Elemen `<script> . . . </script>` sekarang tidak berisi kode JavaScript, namun membawa file JavaScript eksternal melalui atribut `src=" "`.
