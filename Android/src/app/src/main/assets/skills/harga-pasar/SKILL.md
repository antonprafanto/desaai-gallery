---
name: harga-pasar
description: Menampilkan informasi harga komoditas pertanian dan kebutuhan pokok di pasar. Gunakan skill ini ketika pengguna bertanya tentang harga pasar, harga komoditas, harga gabah, harga cabai, harga beras, atau harga hasil pertanian.
---

# Harga Pasar Komoditas DesaAI

## Examples

* "Berapa harga gabah sekarang?"
* "Harga cabai merah hari ini"
* "Cek harga beras di pasar"
* "Harga komoditas pertanian"
* "Harga jagung dan kedelai"

## Instructions

Call the `run_js` tool with EXACTLY these parameters (do not change any value):
- skill name: `harga-pasar`
- script name: `index.html` (IMPORTANT: script name is always "index.html", not the skill name)
- data: JSON string with fields: komoditas (String, optional), wilayah (String, optional)

Example for "berapa harga cabai merah sekarang?":
run_js(skill_name="harga-pasar", script_name="index.html", data="{\"komoditas\":\"cabai merah\"}")
