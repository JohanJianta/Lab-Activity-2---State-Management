# Session 4 : Lab Activity 2 - State Management

Ketika membandingkan kedua aplikasi, terlihat tampilan UI keduanya cukup mirip di mana sama-sama dapat menampilkan perubahan nilai counter ketika tombol Increment atau Decrement (khusus App State) ditekan. Tetapi jika dilihat dari penulisan kodenya, diketahui bahwa status counter dari Ephemeral State berada di dalam widget tempat dia digunakan. Sementara untuk App State, status counter-nya berada di luar widget tempat dia digunakan (punya class sendiri), dan baru dapat digunakan ketika class CounterModel diintegrasikan ke dalam widget tersebut.

Kesimpulan:
a) Ephemeral State menggunakan nilai atau status lokal, dan hanya dapat digunakan di dalam widget tempat dia dideklarasikan
b) App State menggunakan nilai atau status global (terpisah dari seluruh widget), dan dapat digunakan oleh beberapa widget sekaligus

## Kelebihan App State Management

TBD
