# flutter_plugin_pubdev

## Praktikum
### Langkah 1
Pada langkah pertama ini kita membuat project baru serta melakukan push ke githab untuk pertama kali

### Langkah 2
Pada langkah kedua, dilakukan instalasi plugin auto size text dengan perintah `flutter pub add auto_size_text`
![ss](img/Screenshot%20(94).png)

### Langkah 3
Di langkah ketiga, kita membuat file dart baru pada folder lib yang berisi widget RedTextWidget

### Langkah 4
Selanjutnya adalah memodifikasi returd dari return container pada class RedTextWidget untuk dapat menggunakan plugin auto text size, namun pada code tersebut terdapat error yang disebabkan karena variable text yang ada belum di deklarasikan sebelumnya sehingga menyebabkan error. Untuk memperbaikinya terdapat di langkah 5

### Langkah 5
Untuk memperbaiki error tersebut, dengan menambahkan pembuatan variabel pada constructor.
final String text; -> bertujuan untuk membuat variabel text
const RedTextWidget({Key? key, required this.text}) : super(key: key); -> adalah parameter RedTextWidget

### Langkah 6
Pada langkah terakhir ini adalah melakukan pemanggilan widget pada file main.dart untuk dapat ditampilkan.
Sehingga hasil akhir yang diinginkan adalah seprti berikut ini

![ss](img/Screenshot%20(95).png)

Dapat dilihat dari gamber diatas, bahwa text berwarna merah dengan latar kuning adalah text yang menggunakan widget auto text dengan ukuran width 50 dan maksimal line adalah 2
Sedangkan pada text yang warna hijau tanpa menggunakan widget auto text

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
