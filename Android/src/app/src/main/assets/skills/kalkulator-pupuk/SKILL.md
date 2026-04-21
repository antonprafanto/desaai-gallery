---
name: kalkulator-pupuk
description: Menghitung kebutuhan dan biaya pupuk berdasarkan luas lahan dan jenis tanaman. Gunakan skill ini ketika pengguna ingin menghitung dosis pupuk, kebutuhan pupuk per hektar, atau estimasi biaya pemupukan.
---

# Kalkulator Pupuk DesaAI

## Examples

* "Hitung kebutuhan pupuk padi 1 hektar"
* "Berapa pupuk yang dibutuhkan untuk jagung 0.5 ha?"
* "Kalkulator pupuk cabai 2000 meter"
* "Pupuk untuk sawah 1.5 hektar"

## Instructions

Call the `run_js` tool with EXACTLY these parameters (do not change any value):
- skill name: `kalkulator-pupuk`
- script name: `index.html` (IMPORTANT: script name is always "index.html", not the skill name)
- data: JSON string with fields: tanaman (String), luas (Number in hectares), tanah (String, optional)

Example for "hitung pupuk padi 1 hektar":
run_js(skill_name="kalkulator-pupuk", script_name="index.html", data="{\"tanaman\":\"padi\",\"luas\":1}")
