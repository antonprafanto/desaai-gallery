---
name: translate-jawa
description: Menerjemahkan kata dan kalimat antara Bahasa Indonesia dan Bahasa Jawa (Ngoko). Gunakan skill ini ketika pengguna ingin menerjemahkan dari Bahasa Indonesia ke Jawa, dari Jawa ke Indonesia, atau bertanya arti kata Jawa.
---

# Translate Jawa — Penerjemah Indonesia ↔ Jawa DesaAI

## Examples

* "Terjemahkan 'selamat pagi' ke Bahasa Jawa"
* "Apa artinya 'matur nuwun' dalam Bahasa Indonesia?"
* "Tolong translate 'aku mau makan nasi' ke Jawa Ngoko"
* "Apa bahasa Jawanya 'terima kasih'?"
* "Translate 'piye kabare' ke Indonesia"

## Instructions

Call the `run_js` tool with EXACTLY these parameters (do not change any value):
- skill name: `translate-jawa`
- script name: `index.html` (IMPORTANT: script name is always "index.html", not the skill name)
- data: JSON string with fields: teks (String, required), arah (String: "id-jw" or "jw-id", optional, default "id-jw")

Example for "terjemahkan ke bahasa Jawa: selamat pagi":
run_js(skill_name="translate-jawa", script_name="index.html", data="{\"teks\":\"selamat pagi\",\"arah\":\"id-jw\"}")
