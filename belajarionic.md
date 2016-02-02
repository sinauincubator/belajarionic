## BELAJAR IONIC MOBILE HYBRID FRAMEWORK ##

Ionic merupakan framework untuk membuat aplikasi mobile berbasis HTML5.

### PERSIAPAN ###

#### Android SDK ####

1. Download & install android SDK & android studio
2. Pasang android SDK ke path environment variable
3. Jalankan perintah `android` dan install API, emulator, dll sesuai kebutuhan
4. Jalankan perintah `android avd` untuk membuat emulator baru
5. Download dan install gradle build system
6. Pasang gradle ke path environment variable
7. Konfigurasi gradle supaya dapat berjalan secara [daemon mode](https://docs.gradle.org/2.9/userguide/gradle_daemon.html), yaitu dengan menambahkan baris `org.gradle.daemon=true` pada file gradle.properties (buat file tersebut jika belum ada).

#### Ionic Framework ####

1. Install NodeJS, wajib pakai v.4.x untuk v.5.x saat ini belum disupport
2. Install cordova & ionic dari npm `npm install -g cordova ionic`

#### Editor ####

Untuk editor JS ini ada banyak sekali pilihannya: visual studio (windows only), sublime, atom, brackets, dll. Silahkan pakai yang membuat kita nyaman.

Atom bisa diunduh dilink berikut: https://atom.io/.
Brackets bisa dicicipi dengan mengunduh dilink berikut: http://brackets.io/.

Sayangnya untuk pengguna linux versi terbaru, ada bugs yang memungkinkan brackets tidak dapat diinstall. Ini dikarenakan dependency dari aplikasi tersebut masih menggunakan library versi lawas yaitu libgcrypt11, sedangkan pada linux versi baru sudah menggunakan libgcrypt20. Sampai saat ini (2-Feb-2016) bugs tersebut masih dalam kondisi open atau [belum terselesaikan oleh developer brackets](https://github.com/adobe/brackets/issues/10255).

Ada yang mencoba mencari alternatif workaround yang lain dan berhasil menjalankan brackets dengan selamat. Untuk yang penasaran dan ingin mencoba, bisa mengunjungi [link berikut](http://www.webupd8.org/2015/04/fix-missing-libgcrypt11-causing-spotify.html).

### NGODING TIME ###

1. Jalankan perintah `ionic start belajarionic tabs` untuk membuat project berdasarkan template ionic yang telah ada dan kita beri nama project ini belajarionic
2. Pindahkan direktori console ke dalam project `cd belajarionic` dan jalankan perintah `ionic platform add android` untuk memberi tahu ionic bahwa kita ingin meng-enable platform android
3. Jalankan perintah `ionic build android` untuk nge-build project
4. Jalankan perintah `ionic emulate android` untuk menjalankan project, akan muncul tampilan emulator android dan tunggu sampai proses menjalankan emulator selesai - biasanya ketika menjalankan emulator untuk pertama kali membutuhkan waktu yang cukup lama

Referensi:
[Ionic getting started](http://ionicframework.com/docs/guide/installation.html)
[Starting app](http://ionicframework.com/docs/guide/starting.html)
[Testing app](http://ionicframework.com/docs/guide/testing.html)
[Building out app](http://ionicframework.com/docs/guide/building.html)
[Publishing app](http://ionicframework.com/docs/guide/publishing.html)
[Template project ionic](https://www.npmjs.com/package/ionic)

Catatan:
Instalasi ini dilakukan secara online dan membutuhkan bandwidth yang sangat besar.
Jangan sekali-sekali mencoba ionic ios kalau tidak menggunakan MacOS, karena akan menjadi amal perbuatan yang sia-sia.