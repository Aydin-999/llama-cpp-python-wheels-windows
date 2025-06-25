# Windows için Llama-cpp-python ve Sentencepiece Derlenmiş Paketleri (.whl)

Bu depo, en güncel Python sürümleri için `llama-cpp-python` ve `sentencepiece` paketlerini derleme zahmetinden kurtulmak isteyenler için hazırlanmıştır.

Buradaki paketler aşağıdaki ortam için özel olarak derlenmiş ve test edilmiştir.

## Gereksinimler

Bu `.whl` dosyalarını kullanabilmek için sisteminizin aşağıdaki gereksinimleri karşılaması gerekir:

- **İşletim Sistemi:** Windows 10 / 11 (64-bit)
- **Python Sürümü:** Python 3.13.x (64-bit)
- **Ekran Kartı:** CUDA destekli bir NVIDIA ekran kartı
- **NVIDIA Sürücüsü:** CUDA 12.8 veya daha üstünü destekleyen güncel bir sürüm.

## Kurulum

Komut istemini (CMD) veya PowerShell'i açıp aşağıdaki komutları kullanarak kurulumu yapabilirsiniz.

> **Not:** Aşağıdaki linkler, bu depodaki "Releases" bölümünden alınmıştır. Kurmak istediğiniz paketin linkini kopyalayıp direkt `pip install` ile kurabilirsiniz.

### llama-cpp-python (CUDA 12.8 Destekli)

pip install [...llama-cpp-python...whl dosyasının-linkini-buraya-yapıştırın...]

### sentencepiece

pip install [...sentencepiece...whl dosyasının-linkini-buraya-yapıştırın...]

## Nasıl Derlendi?

Bu paketler aşağıdaki araçlar kullanılarak derlenmiştir:
- Visual Studio 2022 Community
- CMake
- CUDA Toolkit 12.8
- `CMAKE_ARGS="-DGGML_CUDA=ON -DCMAKE_CUDA_ARCHITECTURES=86"`
