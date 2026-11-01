# DataPhoenix

**Data recovery tool for Windows.** Recover deleted files from USB flash drives, hard disks, SSDs, external drives and SD cards.

Turkish version is below, Türkçe açıklama aşağıdadır.

## Download

Go to the **Releases** section on the right side of this page and download the latest file under **Assets**. If it is a zip file, extract it first, then run the installer and click Next. A shortcut is added to your desktop.

**System requirements:** Windows 10 or Windows 11, 64-bit. Administrator rights are required to read drives directly.

## Features

- Full screen interface
- 11 languages: English (default), Turkish, German, French, Spanish, Italian, Portuguese, Russian, Arabic, Chinese and Japanese. You can switch language at the top right.
- Three scan modes: Quick, Full and Deep
- Works on USB flash drives, hard disks, SSDs, external drives and SD cards
- Live progress bar and a list of recovered files while scanning
- Choose which file types to recover
- Stop the scan at any time and keep what was already found
- A log file is saved next to your recovered files to help with troubleshooting

## Scan modes

| Mode | What it does | When to use it |
| --- | --- | --- |
| **Quick scan** | Reads the drive layout and checks only free space, where deleted files are kept. Works with NTFS, FAT32 and exFAT. If the layout cannot be read, it scans the whole drive instead. | Files you deleted recently. Fastest. |
| **Full scan** | Reads the whole drive sector by sector. | Older files, or when Quick scan finds too little. |
| **Deep scan** | The most detailed. Full scan plus a search inside already found data for overlapping files, and extra file types. | When nothing else worked. Slowest. |

## Recoverable file types

| Category | Types |
| --- | --- |
| Photos | JPEG, PNG, GIF, HEIC |
| Video and audio | MP4, MOV, 3GP, AVI, WAV, M4A |
| Documents | PDF, Word (docx), Excel (xlsx), PowerPoint (pptx) |
| Archives | ZIP, 7Z |
| Extra types in Deep scan | WEBP, BMP, SQLite databases |

## How to use

1. Right click and run DataPhoenix as administrator. It asks for permission automatically.
2. Select the drive you want to scan.
3. Select an output folder on a **different drive** than the one being scanned. The program does not allow the same drive, so deleted data is not overwritten.
4. Choose a scan mode.
5. Tick the file types you want. Tip: untick PNG and GIF if you only want photos, because website logos and icons are mostly PNG and GIF.
6. Press start. Recovered files appear in the list and are saved in your output folder, sorted into one folder per file type.

## Good to know

- **Stop using the drive immediately.** Any new file you save can overwrite the deleted data.
- **Original file names and folders are not restored.** Files are saved as `recovered_00001.jpg` and so on. This is how file signature recovery works.
- **You may find pictures you do not remember.** A drive keeps remnants of old data such as web browser cache, app files and thumbnails. The program only copies what is physically on the drive.
- **SSDs are harder.** Modern SSDs often erase deleted data for good through a system feature called TRIM, so recovery chances are lower than on USB flash drives and SD cards.
- **Large or fragmented files** can come out incomplete or damaged.
- Drives that were **formatted or lost their partition** are not supported yet.
- On slow flash drives a full scan can take a long time. The progress line shows how much of the drive has been scanned.

## Troubleshooting

**Windows says unknown publisher.** The installer is not code signed, because signing certificates are paid. Click **More info**, then **Run anyway**.

**My antivirus complains.** Programs that read drives directly are sometimes flagged by antivirus software. If you downloaded the file from this page, you can allow it.

**The scan looks stuck.** Check the scanned size next to the percentage. If it still grows, the scan is working, just slowly. If it does not move, press Stop and send me the file `DataPhoenix_log.txt` from your output folder.

**Nothing was found.** Try Full scan, then Deep scan. If the files were deleted a long time ago or the drive has been written to a lot, they may be gone.

## Status and feedback

DataPhoenix is an early version and has not been tested on every kind of drive. Please try it on non-critical data first. If you find a problem, open the **Issues** tab and describe what happened, which drive type you used and which scan mode. Attaching the `DataPhoenix_log.txt` file helps a lot.

## Disclaimer

Use at your own risk. Data recovery can never be guaranteed. Only recover data you have the right to access.

---

# DataPhoenix (Türkçe)

**Windows için veri kurtarma programı.** USB bellek, HDD, SSD, harici disk ve SD kartlardaki silinmiş dosyaları kurtarır.

## İndirme

Bu sayfanın sağ tarafındaki **Releases** bölümüne girin ve **Assets** altındaki en son dosyayı indirin. Zip dosyasıysa önce klasöre çıkarın, sonra kurulum dosyasını çalıştırıp İleri diyerek kurun. Masaüstüne kısayol eklenir.

**Sistem gereksinimi:** Windows 10 veya Windows 11, 64 bit. Sürücüleri doğrudan okuyabilmesi için yönetici izni gerekir.

## Özellikler

- Tam ekran arayüz
- 11 dil: İngilizce (varsayılan), Türkçe, Almanca, Fransızca, İspanyolca, İtalyanca, Portekizce, Rusça, Arapça, Çince ve Japonca. Dili sağ üstten değiştirebilirsiniz.
- Üç tarama modu: Hızlı, Tam ve Derin
- USB bellek, HDD, SSD, harici disk ve SD kart desteği
- Tarama sırasında canlı ilerleme çubuğu ve kurtarılan dosyaların listesi
- Kurtarılacak dosya türlerini seçebilme
- Taramayı istediğiniz an durdurup o ana kadar bulunanları saklayabilme
- Kurtarılan dosyaların yanına, sorun giderme için kayıt dosyası yazılır

## Tarama modları

| Mod | Ne yapar | Ne zaman kullanılır |
| --- | --- | --- |
| **Hızlı tarama** | Sürücünün yapısını okuyup sadece silinmiş dosyaların durduğu boş alanı tarar. NTFS, FAT32 ve exFAT ile çalışır. Yapı okunamazsa tüm sürücüyü tarar. | Yakın zamanda sildiğiniz dosyalar. En hızlısı. |
| **Tam tarama** | Tüm sürücüyü sektör sektör okur. | Daha eski dosyalar ya da hızlı tarama az dosya bulduğunda. |
| **Derin tarama** | En ayrıntılısı. Tam tarama, bulunan verilerin içinde üst üste binen dosyaların aranması ve ek dosya türleri. | Hiçbir şey işe yaramadığında. En yavaşı. |

## Kurtarılabilen dosya türleri

| Kategori | Türler |
| --- | --- |
| Fotoğraf | JPEG, PNG, GIF, HEIC |
| Video ve ses | MP4, MOV, 3GP, AVI, WAV, M4A |
| Belgeler | PDF, Word (docx), Excel (xlsx), PowerPoint (pptx) |
| Arşivler | ZIP, 7Z |
| Derin taramada ek türler | WEBP, BMP, SQLite veritabanları |

## Nasıl kullanılır

1. DataPhoenix'i yönetici olarak çalıştırın. İzni kendisi ister.
2. Taramak istediğiniz sürücüyü seçin.
3. Çıktı klasörünü taranan sürücüden **farklı bir sürücüde** seçin. Program aynı sürücüye izin vermez, böylece silinmiş veriler üzerine yazılmaz.
4. Bir tarama modu seçin.
5. İstediğiniz dosya türlerini işaretleyin. İpucu: Sadece fotoğraf istiyorsanız PNG ve GIF işaretini kaldırın, çünkü internet sitelerinin logo ve ikonları çoğunlukla bu türlerdir.
6. Başlata basın. Kurtarılan dosyalar listede görünür ve çıktı klasörünüze, her tür için ayrı klasör olacak şekilde kaydedilir.

## Bilmeniz gerekenler

- **Sürücüyü hemen kullanmayı bırakın.** Kaydettiğiniz her yeni dosya silinmiş verinin üzerine yazılabilir.
- **Orijinal dosya adları ve klasörler geri gelmez.** Dosyalar `recovered_00001.jpg` gibi adlarla kaydedilir. Dosya imzasıyla kurtarma bu şekilde çalışır.
- **Hatırlamadığınız resimler çıkabilir.** Sürücüde internet tarayıcısı önbelleği, uygulama dosyaları ve küçük resimler gibi eski verilerin kalıntıları durur. Program yalnızca sürücüde fiziksel olarak bulunanı kopyalar.
- **SSD'ler daha zordur.** Modern SSD'ler TRIM denen bir sistem özelliğiyle silinen verileri çoğu zaman kalıcı olarak temizler, bu yüzden kurtarma şansı USB bellek ve SD kartlardan düşüktür.
- **Çok büyük ya da parçalanmış dosyalar** eksik veya bozuk çıkabilir.
- **Biçimlendirilmiş veya bölümü silinmiş** sürücüler henüz desteklenmiyor.
- Yavaş flaş belleklerde tam tarama uzun sürebilir. Yüzdenin yanında taranan boyut yazar, ilerlemeyi oradan görebilirsiniz.

## Sorun giderme

**Windows "Bilinmeyen yayıncı" diyor.** Kurulum dosyası dijital olarak imzalı değil, çünkü imza sertifikaları ücretlidir. **Ek bilgi**, ardından **Yine de çalıştır** deyin.

**Antivirüsüm uyarı veriyor.** Sürücüleri doğrudan okuyan programlar bazen antivirüslerde şüpheli görünür. Dosyayı bu sayfadan indirdiyseniz izin verebilirsiniz.

**Tarama takılmış gibi görünüyor.** Yüzdenin yanındaki taranan boyuta bakın. Sayı hâlâ artıyorsa tarama çalışıyordur, sadece yavaştır. İlerlemiyorsa Durdur'a basın ve çıktı klasörünüzdeki `DataPhoenix_log.txt` dosyasını bana gönderin.

**Hiçbir şey bulunamadı.** Önce Tam taramayı, sonra Derin taramayı deneyin. Dosyalar çok eski zamanda silindiyse ya da sürücüye çok yazıldıysa kaybolmuş olabilir.

## Durum ve geri bildirim

DataPhoenix erken bir sürümdür ve her tür sürücüde denenmemiştir. Önce önemli olmayan verilerle deneyin. Bir sorun bulursanız **Issues** sekmesinden ne olduğunu, hangi sürücü türünü ve hangi tarama modunu kullandığınızı yazın. `DataPhoenix_log.txt` dosyasını eklemeniz çok yardımcı olur.

## Sorumluluk reddi

Kullanım sorumluluğu size aittir. Veri kurtarma hiçbir zaman garanti edilemez. Yalnızca erişim hakkınız olan verileri kurtarın.
