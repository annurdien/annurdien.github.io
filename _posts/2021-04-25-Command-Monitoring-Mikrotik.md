## Perintah-Perintah, Parameter, dan Fungsinya
Ketikkan perintah berikut pada kolom _chatting_ Anda dengan _bot_ Telegram Anda. Setiap _parameter_ yang dimasukkan, dipisahkan dengan menggunakan spasi, misalnya ``/interface show``.

| Perintah | Parameter | Fungsi | Contoh |
|-----------|--------------|-------|-----|
| ``/help`` | | Menampilkan daftar fungsi yang dapat dieksekusi | |
| ``/start`` | | Menampilkan daftar fungsi yang dapat dieksekusi | |
| ``/cpu`` | | Menampilkan Router ID, Load CPU, Uptime, dan total RAM yang terpakai | |
| ``/dhcp`` | ``lease`` | menampilkan seluruh detail pada DHCP Lease| ``/dhcp lease`` |
| ``/interface`` | ``show`` | Menampilkan status terhubungnya antar port Ethernet di MikroTik | ``/interface show`` |
| ``/interface`` | ``show all`` | Menampilkan status terhubungnya seluruh interface di MikroTik | ``/interface show all`` |
| ``/hotspot`` | ``help`` | Menampilkan detail bantuan untuk perintah `/hotspot` | ``/hotspot help`` |
| ``/hotspot`` | ``session count`` | Menampilkan jumlah user yang sedang aktif | ``/hotspot session count`` |
| ``/hotspot`` | ``session showall`` | Menampilkan seluruh detail user yang sedang aktif mulai dari Username sampai Uptime (kecuali password) | ``/hotspot session showall`` |
| ``/hotspot`` | ``session deauth-by-user <username>`` | Mencabut _session_ perangkat berdasarkan Username | ``/hotspot session deauth-by-user telecomadmin`` |
| ``/hotspot`` | ``session deauth-by-ip <ip>`` | Mencabut _session_ perangkat berdasarkan Alamat IP | ``/hotspot session deauth-by-ip 192.168.1.2`` |
| ``/hotspot`` | ``session deauth-by-mac <mac address>`` | Mencabut _session_ perangkat berdasarkan Alamat MAC | ``/hotspot session deauth-by-mac AB:CD:EF:01:23:45`` |
| ``/hotspot`` | ``add <username> <password>`` | Menambahkan user hotspot baru | ``/hotspot add telecomadmin admintelecom`` |
| ``/hotspot`` | ``delete <username>`` | Menghapus user hotspot secara permanen | ``/hotspot delete telecomadmin`` |
| ``/hotspot`` | ``disable <username>`` | Mematikan atau menonaktifkan user hotspot | ``/hotspot disable telecomadmin`` |
| ``/hotspot`` | ``enable <username>`` | Mengaktifkan user hotspot yang dinonaktifkan | ``/hotspot enable telecomadmin`` |
| ``/hotspot`` | ``change-password <username> <password baru>`` | Mengubah password user hotspot | ``/hotspot change-password telecomadmin p4ssw0rdny4`` |
| ``/ping`` | | Melakukan ping ke DNS Google | ``/ping`` |
| ``/monitoring`` | ``interface <interface>`` | Melakukan monitoring terhadap interface | ``/monitoring interface wlan1`` |
| ``/monitoring`` | ``cpu`` | Melakukan monitoring terhadap penggunaan Cpu pada router | ``/monitoring cpu`` |
| ``/monitoring`` | ``ram`` | Melakukan monitoring terhadap penggunaan ram/memory pada router | ``/monitoring ram`` |
| ``/monitoring`` | ``memory`` | Melakukan monitoring terhadap penggunaan ram/memory pada router | ``/monitoring memory`` |
| ``/ping`` | ``to <ip address>`` | Melakukan ping ke alamat IP tertentu | ``/ping to 127.0.0.1`` |
| ``/public`` | | Menampilkan Dynamic DNS dan Public IP pada MikroTik Anda | ``/public`` |
| ``/enablehotspot`` | | Mengaktifkan seluruh fungsi hotspot | ``/enablehotspot`` |
| ``/disablehotspot`` | | Menonaktifkan seluruh fungsi hotspot | ``/disablehotspot`` |
| ``/forceupdateddns`` | | Memperbarui Dynamic DNS secara paksa | ``/forceupdateddns`` |
| ``/reboot`` | | Menghidupkan ulang MikroTik (jeda 30 detik sebelum menghidupkan ulang) | ``/reboot`` |

> **Catatan**: untuk dapat menjalankan perintah ``/disablehotspot``,  ``/enablehotspot``, dan ``/interface show``, silakan Anda konfigurasikan sendiri hotspot mana yang akan di "otomatis" kan di script ``tg_cmd_disablehotspot``, ``tg_cmd_enablehotspot``, dan ethernet mana saja yang akan ditampilkan di ``tg_cmd_interface``.

