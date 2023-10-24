# Session 4 : Lab Activity 2 - State Management

Ketika membandingkan kedua aplikasi, terlihat tampilan UI keduanya cukup mirip di mana sama-sama dapat menampilkan perubahan nilai counter ketika tombol Increment atau Decrement (khusus App State) ditekan. Tetapi jika dilihat dari penulisan kodenya, diketahui bahwa status counter dari Ephemeral State berada di dalam widget tempat dia digunakan. Sementara untuk App State, status counter-nya berada di luar widget tempat dia digunakan (punya class sendiri), dan baru dapat digunakan ketika class CounterModel diintegrasikan ke dalam widget tersebut.

Kesimpulan perbedaan:
a) Ephemeral State menggunakan nilai atau status lokal, serta hanya dapat digunakan dan dimodifikasi di dalam widget tempat dia dideklarasikan
b) App State menggunakan nilai atau status global (terpisah dari seluruh widget), serta dapat digunakan dan dimodifikasi oleh beberapa widget sekaligus secara terpisah

## Kelebihan App State Management

1) Skalabilitas
App State Management memungkinkan pengembang untuk memisakahkan antara logika status aplikasi dengan tampilan UI-nya. Hal ini membuat kode aplikasi jadi semakin rapi dan mudah dikelola, sehingga akan sangat membantu apabila ke depannya aplikasi akan dikembangkan lagi.

2) Konsistensi data secara global
App State Management memungkinkan dibuatnya fitur aplikasi yang lebih luas dan kompleks, misalnya autentikasi pengguna. Dengan menempatkan status autentikasi pengguna sebagai status global, maka ketika pengguna selesai login, seluruh widget yang membutuhkan autentikasi penggunan akan otomatis bisa digunakan (seluruh fitur berbagi status autentikasi). Contoh lainnya adalah keranjang belanja. Dengan membuat keranjang belanja menjadi nilai global, maka tiap barang yang dibeli pengguna akan otomatis ditambahkan ke dalam keranjang (keranjang dapat diakses oleh seluruh barang). Hal ini menjamin konsistensi data yang diterima oleh seluruh bagian aplikasi. 
