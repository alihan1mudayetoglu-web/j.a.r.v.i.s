🤖 J.A.R.V.I.S Windows

Windows için geliştirilmiş, Gemini AI destekli sesli asistan.

J.A.R.V.I.S; sesli komutlarla uygulama açma, hava durumu görüntüleme, sistem bilgilerini kontrol etme, YouTube/Spotify kullanma ve daha birçok işlemi gerçekleştirebilir.

⸻

📋 Gereksinimler

* Windows 10 / 11
* Python 3.12
* Visual Studio Code
* Gemini API Key
* Mikrofon
* İnternet bağlantısı

Not: Python 3.13 veya 3.14 bilgisayarınızda kuruluysa kaldırmanız gerekmez. Python 3.12 ile birlikte kullanılabilir.

⸻

🚀 Kurulum

1. Python 3.12 Kur

Python 3.12.8’i aşağıdaki adresten indirin:

Python 3.12.8 İndir

Sayfanın en altında:

Windows installer (64-bit)

bağlantısına tıklayın.

Kurulum sırasında:

1. Add python.exe to PATH seçeneğini işaretleyin.
2. Install Now butonuna tıklayın.

Kurulum tamamlandıktan sonra Terminal / CMD açıp kontrol edin:

py -3.12 --version

Şuna benzer bir çıktı almanız gerekir:

Python 3.12.x

⸻

2. Visual Studio Code Kur

Visual Studio Code uygulamasını indirin ve kurun.

VS Code’u açtıktan sonra:

1. Sol taraftaki Extensions bölümüne girin.
2. Ctrl + Shift + X kısayolunu da kullanabilirsiniz.
3. Arama bölümüne Python yazın.
4. Microsoft tarafından yayınlanan Python eklentisini kurun.

⸻

3. Projeyi VS Code’da Aç

VS Code içerisinde:

File → Open Folder

seçeneğine tıklayın.

Ardından:

jarvis-windows

klasörünü seçin.

⸻

📦 4. Gerekli Paketleri Kur

VS Code içerisinde terminali açın:

Ctrl + J

Ardından aşağıdaki komutu çalıştırın:

python -m pip install google-genai psutil Pillow requests pyperclip mss SpeechRecognition

Eğer bu komut çalışmazsa:

py -3.12 -m pip install google-genai psutil Pillow requests pyperclip mss SpeechRecognition PyAudio

Kurulum birkaç dakika sürebilir. İşlem tamamlanana kadar terminali kapatmayın.

PyAudio

Önce:

python -m pip install pipwin

Ardından:

python -m pipwin install pyaudio

Eğer pipwin ile kurulum hata verirse doğrudan şunu deneyin:

py -3.12 -m pip install PyAudio

⸻

🔑 5. Gemini API Key Al

J.A.R.V.I.S’in Gemini AI özelliklerini kullanabilmesi için bir Gemini API anahtarına ihtiyacınız vardır.

Google AI Studio adresine gidin.

Ardından:

Get API Key
      ↓
Create API Key

seçeneklerini kullanarak API anahtarınızı oluşturun.

⚠️ API anahtarınızı GitHub’a yüklemeyin!

API anahtarınızı main.py, README veya başka bir herkese açık dosyanın içine doğrudan yazmayın.

⸻

▶️ 6. J.A.R.V.I.S’i Çalıştır

VS Code terminalinde proje klasörünün içerisinde:

py -3.12 main.py

komutunu çalıştırın.

Alternatif olarak VS Code içerisinden:

F5

tuşuna basabilirsiniz.

J.A.R.V.I.S penceresi açıldığında kurulum tamamlanmıştır.

Ardından uygulamanın istediği bölüme Gemini API Key bilginizi girin.

⸻

🛠️ Sık Karşılaşılan Hatalar

pip is not recognized

pip yerine:

python -m pip

kullanın.

Örneğin:

python -m pip install requests

⸻

No module named 'pyaudio'

Python sürümünüzü kontrol edin:

py -3.12 --version

J.A.R.V.I.S’i Python 3.12 ile çalıştırın:

py -3.12 main.py

Gerekirse:

py -3.12 -m pip install PyAudio

⸻

No module named 'xxx'

Eksik olan paketi Python 3.12 için kurun:

py -3.12 -m pip install xxx

Örneğin:

py -3.12 -m pip install requests

⸻

PyAudio kurulumu başarısız oluyor

Öncelikle Python sürümünüzü kontrol edin:

py -3.12 --version

Ardından:

py -3.12 -m pip install PyAudio

komutunu deneyin.

⸻

✨ Özellikler

Özellik	Durum
🎙️ Sesli konuşma	✅
🤖 Gemini AI	✅
🚀 Uygulama açma	✅
🌤️ Hava durumu	✅
💻 Sistem bilgileri	✅
🧠 CPU / RAM / Disk / Pil bilgisi	✅
🌐 Browser kontrolü	✅
▶️ YouTube arama ve oynatma	✅
🎵 Spotify	✅
💬 WhatsApp Desktop + Web	✅
🖥️ Ekran analizi	✅
👏 Çift alkış ile uyanma	✅
📅 Google Calendar	⚠️ Tarayıcı üzerinden açılır
⏰ Hatırlatıcılar	⚠️ Microsoft To-Do açılır
🍎 Apple Music	⚠️ YouTube’a yönlendirir

⸻

📁 Proje Yapısı

Örnek proje yapısı:

jarvis-windows/
│
├── main.py
├── README.md
├── requirements.txt
└── ...

⸻

🔐 Güvenlik

Gemini API Key’inizi kesinlikle GitHub repository’sine yüklemeyin.

API anahtarını kod içerisinde sabit olarak tutmak yerine ortam değişkeni veya .env dosyası kullanmanız önerilir.

Örneğin:

.env

dosyasını .gitignore içerisine ekleyin:

.env
__pycache__/
*.pyc

Eğer API anahtarınızı yanlışlıkla GitHub’a yüklediyseniz, anahtarı yalnızca dosyadan silmek yeterli değildir. Google AI Studio üzerinden anahtarı iptal edip yeni bir anahtar oluşturun.

⸻

📄 Lisans

Bu projenin lisans bilgileri için repository içerisindeki LICENSE dosyasına bakın.

⸻

⭐ Destek

Projeyi faydalı bulduysanız GitHub üzerinde ⭐ Star vermeyi unutmayın!

Katkıda bulunmak, hata bildirmek veya yeni özellik önermek için Issues ve Pull Requests bölümünü kullanabilirsiniz.
