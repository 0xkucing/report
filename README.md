## Unauthenticated Blind SSRF via xmlrpc.php
- target: ppid.baliprov.go.id
- severity: 5.3 (Medium)
- cvss: CVSS:3.0/AV:N/AC:L/PR:N/UI:N/S:U/C:L/I:N/A:N

### Description

SSRF via XMLRPC WordPress Pingback adalah kerentanan pada WordPress yang memungkinkan penyerang membuat permintaan HTTP arbitrer dari situs web WordPress yang rentan. Kerentanan ini dapat dimanfaatkan untuk melakukan berbagai serangan.

### Impact

1. Serangan DDoS: Penyerang dapat mengirim sejumlah besar permintaan ke situs web yang rentan, membebani server dan menyebabkannya tidak tersedia.
2. Pengungkapan informasi: Penyerang dapat mengirim permintaan ke server internal atau pribadi, berpotensi mengungkapkan informasi sensitif.

### Proof of concept

1. Menggunakan tools ```SecurityTrails``` saya mencari subdomain
2. Dengan tools ```httpx``` saya filter mana website yang menggunkan cms ```WordPress```
3. Dan saya coba menargetkan ```ppid.baliprov.go.id```
