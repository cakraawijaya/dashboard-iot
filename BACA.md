[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?style=flat)](https://github.com/ellerbrock/open-source-badges/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?logo=github&color=%23F7DF1E)](https://opensource.org/licenses/MIT)
![GitHub last commit](https://img.shields.io/github/last-commit/cakraawijaya/Dashboard-IoT-Berbasis-Node-JS?logo=Codeforces&logoColor=white&color=%23F7DF1E)
![Project](https://img.shields.io/badge/Project-Website-light.svg?style=flat&logo=googlechrome&logoColor=white&color=%23F7DF1E)
![Type](https://img.shields.io/badge/Type-Workshop%20Assignment-light.svg?style=flat&logo=gitbook&logoColor=white&color=%23F7DF1E)

# Dashboard IoT Berbasis Node.js
Proyek ini memiliki efisiensi sumber daya dan kinerja yang tinggi, termasuk pemrosesan data secara real-time, serta keamanan siber yang baik.

<br>

## Kebutuhan Proyek
| Bagian | Deskripsi |
| --- | --- |
| Skema | Virtual |
| Fitur | • Publish<br>• Subscribe |
| Papan Pengembangan | DOIT ESP32 DEVKIT V1 |
| Editor Kode | Visual Studio Code |
| Dukungan Aplikasi | • Wokwi<br>• MQTTX<br>• Node.js |
| Broker MQTT | EMQX Broker |
| Protokol komunikasi | • Hypertext Transfer Protocol (HTTP)<br>• Message Queuing Telemetry Transport (MQTT) |
| Arsitektur IoT | 3 Lapisan |
| Kerangka Kerja | • Bootstrap 5<br>• Express.js<br>• Font-Awesome 6 |
| Pustaka | MQTT.js |

<br><br>

## Unduh & Instal
1. Visual Studio Code
   <table><tr><td width="810">

   ```
   https://bit.ly/VScode_Installer
   ```

   </td></tr></table><br>

2. NodeJS
   <table><tr><td width="810">

   ```
   https://nodejs.org/en/download/prebuilt-installer
   ```

   </td></tr></table><br>

3. MQTTX
   <table><tr><td width="810">

   ```
   https://mqttx.app/downloads
   ```

   </td></tr></table>

<br><br>

## Rancangan Proyek
<table>
<tr>
<th width="840">Infrastruktur</th>
</tr>
<tr>
<td><img src="documentation/diagram/Infrastructure.jpg" alt="infrastructure"></td>
</tr>
</table>

<br><br>

## Memulai
1. Buat direktori baru dengan nama ``` dashboard-iot ```.<br><br>
2. Unduh dan ekstrak repositori ini.<br><br>
3. Salin direktori: ``` public ``` dan ``` views ```.<br><br>
4. Salin berkas: ``` server.js ```.<br><br>
5. Tempel dan Timpa ke dalam direktori ``` dashboard-iot ```.<br><br>
6. Buka ``` Terminal ``` di dalam direktori tersebut.<br><br>
7. Buat berkas ``` package.json ``` dengan mengetik perintah:<br>
   <table><tr><td width="810">
      
   ```bash
   npm init -y
   ```
   
   </td></tr></table>
   <br>
8. Instal ``` express ``` untuk membuat server backend:<br>
   <table><tr><td width="810">
      
   ```bash
   npm install express
   ```
   
   </td></tr></table>
   <br>
9. Instal ``` mqtt ``` untuk komunikasi data IoT:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install mqtt
    ```
   
    </td></tr></table>
    <br>
10. Instal ``` mqttjs ``` untuk menghubungkan web dan Node.js ke broker MQTT secara real-time:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install mqttjs
    ```
   
    </td></tr></table>
    <br>
11. Instal ``` ejs ``` untuk membuat halaman web dengan konten dinamis:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install ejs
    ```
   
    </td></tr></table>
    <br>
12. Instal ``` bootstrap ``` untuk mengatur tampilan (layout):<br>
    <table><tr><td width="810">
      
    ```bash
    npm install bootstrap
    ```
   
    </td></tr></table>
    <br>
13. Instal ``` fontawesome ``` untuk ikon:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install @fortawesome/fontawesome-free
    ```
   
    </td></tr></table>
    <br>
14. Buka ``` package.json ```, lalu ubah bagian ``` scripts ``` menjadi seperti ini:<br>
    <table><tr><td width="810">
      
    ```bash
    "scripts": {
      "start": "node server.js",
      "dev": "nodemon server.js"
    },
    ```
   
    </td></tr></table>
    <br>
15. Instal ``` nodemon ``` untuk me-restart server secara otomatis:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install --save-dev nodemon
    ```
   
    </td></tr></table>
    <br>
16. Untuk menjalankan web, ketikan perintah:<br>
    <table><tr><td width="810">
      
    ```bash
    npm run dev
    ```
   
    </td></tr></table>
    <br>
17. Buka peramban anda, lalu ketik -> ``` http://localhost:3000/ ```.<br><br>
18. Isi form Topic dan Data terlebih dahulu, misalnya: `kelasiot/pot` | `4095` -> kemudian klik `Publish`, maka hasilnya akan tertampil.<br><br>
19. Port dan Topic Subscribe ini dapat diubah sesuai keinginan pengguna. Pengaturan ini terdapat dalam file bernama `server.js`.<br><br>
20. Silakan akses fitur-fiturnya dan nikmatilah [Selesai].

<br><br>

## Simulasi Dengan MQTTX
`MQTTX Web` menyediakan 2 protokol komunikasi, yaitu `WebSocket (WS)` dan `WebSocket Secure (WSS)`. Selain itu juga ada `MQTTX Desktop`, yang secara pilihan lebih lengkap.<br><br>
1. Jika anda menggunakan `MQTTX Web`, pastikan untuk memilih protokol `WSS` agar aman.<br><br>
2. Jika anda menggunakan `MQTTX Desktop`, jangan lupa untuk mengunduh aplikasinya. Lalu, jika sudah diunduh, bukalah aplikasi tersebut di laptop atau komputer anda.<br><br>
3. Klik `+ New Connection` -> lalu beri nama koneksi sesuai dengan keinginan anda -> lalu klik `Connect`.<br><br>
4. Buat topic baru dengan nama `kelasiot/pot`.<br><br>
5. Kemudian untuk pengaturan topic bisa anda sesuaikan seperti yang terlihat di bawah ini:<br><br>
   <table><tr><td width="810">
   • Format Payload to Publish by : &nbsp; <strong>`Plaintext`</strong>.<br><br>
   • Qos : &nbsp; <strong>`0`</strong>.<br><br>
   • Beri tanda centang pada <strong>`Retain`</strong>.
   </td></tr></table><br>
6. Publish data.<br><br>
7. Setelah itu, silakan klik `+ New Subscription` -> lalu cantumkan topic yang ingin anda subscribe, contohnya: `kelasiot/#`.<br><br>
8. Tunggu hingga hasil subscribenya tertampil.<br><br>
9. Bersenang-senang dan nikmatilah [Selesai].

<br><br>

## Deploy di Railway
1. Buka platform Railway:&nbsp;&nbsp;<strong><a href="https://railway.com/">Klik Disini</a></strong> &nbsp;, lalu Login dengan Github.<br><br>
2. Izinkan Railway untuk mengakses repositori.<br><br>
3. Upload proyek ke GitHub.<br><br>
4. Masuk ke dashboard Railway:&nbsp;&nbsp;<strong><a href="https://railway.com/dashboard">Klik Disini</a></strong><br><br>
5. Klik ``` Add New Project ```.<br><br>
6. Pilih repositori GitHub mana yang diinginkan.<br><br>
7. Pilih menu ``` Settings ``` -> Ubah ``` Name ``` dan ``` Description ``` sesuai dengan kebutuhan -> Klik tombol ``` Update ```.<br><br>
8. Pilih menu ``` Architecture ``` -> Klik ``` Project ```.<br><br>
9. Klik ``` Variables ``` di bagian Project -> Klik tombol ``` New Variable ```, lalu isi persis seperti ini:<br>
   - Placeholder: ``` VARIABLE_NAME ```
       <table><tr><td width="810">
         
       ```bash
       MQTT_BROKER
       ```
      
       </td></tr></table>
       
   - Placeholder: ``` VALUE or ${{REF}} ```
       <table><tr><td width="810">
         
       ```bash
       mqtt://broker.emqx.io
       ```
      
       </td></tr></table>
       <br>
10. Klik ``` Settings ``` di bagian Project -> Cari ``` Public Networking ``` -> Klik tombol ``` Generate Domain ```.<br><br>
11. Untuk mendapatkan domain yang bersih:&nbsp;&nbsp;Klik ``` Edit ``` -> Klik tombol ``` Update ``` (*Opsional).

<br><br>

## Simulasi Dengan Wokwi
Tautan untuk mensimulasikan : <strong><a href="https://wokwi.com/projects/413253569138415617" target="_blank">Klik Disini</a></strong>

<br><br>

## Sorotan
<table>
<tr>
<th width="420">Tampilan Dashboard</th>
<th width="420">Menjalankan Server</th>
</tr>
<tr>
<td><img src="documentation/experiment/Web Dashboard.jpg" alt="dashboard"></td>
<td><img src="documentation/experiment/Running the Server.jpg" alt="server"></td>
</tr>
</table>
<table>
<tr>
<th width="420">Simulasi MQTTX</th>
<th width="420">Simulasi Wokwi</th>
</tr>
<tr>
<td><img src="documentation/experiment/MQTTX Simulation.jpg" alt="mqttx"></td>
<td><img src="documentation/experiment/Wokwi Simulation.jpg" alt="wokwi"></td>
</tr>
</table>

<br><br>

## Apresiasi
Jika karya ini bermanfaat bagi anda, maka dukunglah karya ini sebagai bentuk apresiasi kepada penulis dengan mengklik tombol `⭐Bintang` di bagian atas repositori.

<br><br>

## Penafian
Aplikasi ini merupakan hasil pengembangan dari Workshop Kelas IoT. Saya tidak memungkiri bahwa saya masih menggunakan layanan pihak ketiga dalam pengerjaan ini, antara lain: library, framework, dan lain sebagainya.

<br><br>

## LISENSI
LISENSI MIT - Hak Cipta © 2024 - Devan C. M. Wijaya, S.Kom

Dengan ini diberikan izin tanpa biaya kepada siapa pun yang mendapatkan salinan perangkat lunak ini dan file dokumentasi terkait perangkat lunak untuk menggunakannya tanpa batasan, termasuk namun tidak terbatas pada hak untuk menggunakan, menyalin, memodifikasi, menggabungkan, mempublikasikan, mendistribusikan, mensublisensikan, dan/atau menjual salinan Perangkat Lunak ini, dan mengizinkan orang yang menerima Perangkat Lunak ini untuk dilengkapi dengan persyaratan berikut:

Pemberitahuan hak cipta di atas dan pemberitahuan izin ini harus menyertai semua salinan atau bagian penting dari Perangkat Lunak.

DALAM HAL APAPUN, PENULIS ATAU PEMEGANG HAK CIPTA DI SINI TETAP MEMILIKI HAK KEPEMILIKAN PENUH. PERANGKAT LUNAK INI DISEDIAKAN SEBAGAIMANA ADANYA, TANPA JAMINAN APAPUN, BAIK TERSURAT MAUPUN TERSIRAT, OLEH KARENA ITU JIKA TERJADI KERUSAKAN, KEHILANGAN, ATAU LAINNYA YANG TIMBUL DARI PENGGUNAAN ATAU URUSAN LAIN DALAM PERANGKAT LUNAK INI, PENULIS ATAU PEMEGANG HAK CIPTA TIDAK BERTANGGUNG JAWAB, KARENA PENGGUNAAN PERANGKAT LUNAK INI TIDAK DIPAKSAKAN SAMA SEKALI, SEHINGGA RISIKO ADALAH MILIK ANDA SENDIRI.
