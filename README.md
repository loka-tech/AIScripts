# AIScripts
Kumpulan scripts yang salah satu member disini gunakan untuk mempelajari AI + beberapa notebooks tutor.


## Daftar Isi
- [AIScripts](#aiscripts)
  - [Daftar Isi](#daftar-isi)
  - [Keterangan](#keterangan)
  - [Requirements](#requirements)
  - [Cara Menjalankan](#cara-menjalankan)
  - [Referensi](#referensi)

## Keterangan
- `Inference`: berisi notebook yang digunakan untuk inferensi smodel (menjalankan model). Saat ini hanya ada notebook untuk [Text generation web UI](https://github.com/oobabooga/text-generation-webui) dan [koboldcpp](https://github.com/LostRuins/koboldcpp). Untuk backend lain akan ditambahkan jika ada waktu luang.
- `Merging scripts`: berisi berbagai script yang digunakan untuk menggabungkan model dan peft(LoRA).
- `Quant scripts`: berisi scripts yang digunakan untuk mengubah model menjadi lebih kecil (quantization)

## Requirements
- [Google Colab](https://colab.research.google.com/)
runpod/vast.ai juga bisa, tapi colab lebih mudah digunakan 

Untuk inference, bisa menggunakan colab free, tapi untuk quantisasi, merging dan training model, colab pro sangat disarankan. Contoh penggunaan RAM dan VRAM untuk quantisasi:

- ExllamaV2: 20GB RAM, 12GB VRAM untuk 13B model
- GPTQ: 30GB RAM, 16GB VRAM untuk 13B model
- llama.cpp: 12GB RAM, 5GB VRAM untuk 13B model

Sedangkan untuk merging, membutuhkan RAM yang lebih besar lagi, karena membutuhkan RAM untuk load model dan peft. Contoh penggunaan RAM untuk merging:

- DARE Method: 55GB RAM untuk merging 3 model 13B
- Mergekit: Tergantung metode yang digunakan, biasanya setiap 1 model 13B membutuhkan 20GB - 30GB RAM
- BlockMerge Gradient: Kacau yang ini, butuh ram 50GB uuntuk merging 2 model 13B

Setiap model juga membutuhkan penyimpanan yang besar, untuk 1 Model 13B, membutuhkan penyimpanan sekitar 25GB dalam bentuk fp16, kalau yang punya model upload nya dalam bentuk fp32, lebih kacau lagi... Untuk 1 model 70B, membutuhkan penyimpanan sekitar 150GB dalam bentuk fp16.


## Cara Menjalankan

### Text generation web UI
- to be added later

### Merging scripts
- to be added later

### Quant scripts
- to be added later

## Referensi
- [Mergekit](https://github.com/cg123/mergekit)
- [ExLlamaV2](https://github.com/turboderp/exllamav2)
- [Text generation web UI](https://github.com/oobabooga/text-generation-webui)
- [koboldcpp](https://github.com/LostRuins/koboldcpp)
- [AIScripts](https://github.com/TheBlokeAI/AIScripts)
- [zaraki-tools](https://github.com/zarakiquemparte/zaraki-tools)
- [LLM-notebooks](https://github.com/DocShotgun/LLM-notebooks)
- [LLM Course](https://github.com/mlabonne/llm-course)
