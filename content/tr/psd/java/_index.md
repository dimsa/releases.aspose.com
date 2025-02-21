---
title: "Aspose.psd | PSD ve PSB formatlarını oluşturmak için Java Sınıf Kütüphanesi" 
linktitle: Aspose.PSD
description: "Java Sınıf Kütüphanesi, uygulamalarınızın Photoshop PSD ve PSB formatlarını oluşturmasını, değiştirmesini ve dönüştürmesini sağlamak için. Görüntü sıkıştırma, terleme, oluşturma ve ölçeklendirme vb." 
layout: packages
type: repository
categories:
  - fundamentals
keywords:
- Aspose Total
- Aspose PSD
- Aspose Java API
- psd java library
- psd java class
- PSD
- PSB
- TIFF
- JPEG
- PNG
- GIF
- BMP
- JPEG2000
- PDF
- AI
- convert format
- image loading
- photoshop
- raw data processing
- image compression
- psd compression
- image rotation
- flip image
- image scale
- cache system
- exif data
- dithering
- crop
- vector to raster
- cubic b�zier
- matrix transformation
- Maven
- Windows
- Linux
- Mac
- JDK
- adjustment layer
- median filter
- wiener filter
- graphics
- linked layer
- text layer
family_listing_page_title: "Java için aspose.psd" 
family_listing_page_description: "Java için aspose.psd, kullanımı kolay bir Adobe Photoshop Formatları Manipülasyon API'sıdır. Şu anda PSD ve PSB formatlarını kolayca yükleyebilir ve okuyabilir. Geliştiriciler, katman özelliklerini güncelleme, filigran ekleme, sıkıştırma, rotasyon, ölçeklendirme veya Adobe Photoshop'un kurulumu olmadan bir dosya biçimini diğerine oluşturma gibi işlemleri gerçekleştirebilir. TIFF, JPEG, PNG, GIF, BMP ve daha fazlası gibi görüntü formatları kolayca dışa aktarılabilir." 
family_listing_page_iconurl: "https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/psd/272x272/aspose_psd-for-java.png"
family_listing_page_selfHosted: "1"
family_listing_page_type: "1"
family_listing_page_venture: "4"
family_listing_page_package: "160"
homepage_package_type: "Maven"
homepage_package_link: "https://releases.aspose.com/java/repo/com/aspose/aspose-psd/"
weight: 02	#rem
forumLink: https://forum.aspose.com/c/psd/34
productLink: https://products.aspose.com/psd/java/
releaseNotesLink: https://docs.aspose.com/psd/java/release-notes/
dataFolder: aspose_psd
packages_refs:
- "19-12"
- "19-4"
- "20-2"
- "20-3"
- "20-4"
- "20-5"
- "20-6"
- "20-7"
- "20-8"
- "20-9"
- "21-5"
- "21-6"
- "21-7"
---

# Photoshop dosyaları için Java Kütüphanesi
{{< repository/extract-package-explore-link imgsrc=./aspose_psd-for-java-banner.png >}}

[Ürün sayfası](https://products.aspose.com/psd/java) | [Belgeler](https://docs.aspose.com/psd/java/) | [Demolar](https://products.aspose.app/psd/family) | [API referansı](https://apireference.aspose.com/psd/java) | [Örnekler](https://github.com/aspose-psd/Aspose.PSD-for-Java) | [Blog](https://blog.aspose.com/category/psd/) | [Arama](https://search.aspose.com/) | [Ücretsiz Destek](https://forum.aspose.com/c/psd) | [Geçici lisans](https://purchase.aspose.com/temporary-license)

[Aspose.PSD for Java](https://products.aspose.com/psd/java), kullanımı kolay bir Adobe Photoshop Dosyası Formatı Manipülasyon API'sıdır. PSD, PSB ve AI dosyalarını kolayca yükleyebilir ve okuyabilir, Java geliştiricilerinin katman özelliklerini güncelleme, filigran ekleme, sıkıştırma, rotasyon, ölçeklendirme veya Adobe Photoshop'u yüklemeye gerek kalmadan bir dosya formatını başka bir dosya biçimini oluşturmasını mümkün kılabilir.

## Photoshop Dosya İşleme
- PSD ve PSB dosyalarını yükleyin, oluşturun ve manipüle edin.
- PSD'yi RLE ile sıkıştırın.
- Görüntüleri döndürün, çevirin, ölçeklendirin veya kırpın.
- EXIF ​​verilerini okuyun ve yazın.
- Vektörü raster'e dönüştürün.
- Parlaklık, kontrast ve gamma ayarlayın.
- Temel şekilleri çizin ve doldurun.
- Klip dikdörtgen bölgeler.
- Dithering uygulayın.

## Photoshop ve Illustrator dosyalarını yükleyin
** Adobe **: PSD, PSB, AI

## Photoshop ve Illustrator dosyalarını şu şekilde kaydedin
** Raster **: Tiff, JPEG, PNG, GIF, BMP, JPEG2000 \
** Sabit Düzen **: PDF

## Desteklenen Ortamlar
- ** Microsoft Windows: ** Windows Desktop & Server (x86, x64)
- ** MacOS: ** Mac OS X
- ** linux: ** ubuntu, opense, centos ve diğerleri
- ** Java Sürümleri: ** `J2SE 6.0 (1.6)` veya üstü

## Başlamak

Aspose.psd Java API'leri [Aspose deposu](https://repository.aspose.com/psd/)'da barındırılır. Basit konfigürasyonlarla doğrudan Maven projelerinizde Java API'sı için aspose.psd'yi kolayca kullanabilirsiniz. Ayrıntılı talimatlar için lütfen [Installing Aspose.PSD for Java from Maven Repository](https://docs.aspose.com/psd/java/installation/) belgesi PSD'yi ziyaret edin.

## Sıfırdan bir PSD oluşturun

```java
PsdImage bmpImage = new PsdImage(300, 300);

// fill image data.
Graphics graphics = new Graphics(bmpImage);
graphics.clear(Color.getWhite());
Pen pen = new Pen(Color.getBrown());
graphics.drawRectangle(pen, bmpImage.getBounds());

// create an instance of PsdOptions, Set it's various properties Save image to disk in PSD format
PsdOptions psdOptions = new PsdOptions();
psdOptions.setColorMode(ColorModes.Rgb);
psdOptions.setCompressionMethod(CompressionMethod.Raw);
psdOptions.setVersion(4);
bmpImage.save("output.psd", psdOptions);
```

[Ürün sayfası](https://products.aspose.com/psd/java) | [Belgeler](https://docs.aspose.com/psd/java/) | [Demolar](https://products.aspose.app/psd/family) | [API referansı](https://apireference.aspose.com/psd/java) | [Örnekler](https://github.com/aspose-psd/Aspose.PSD-for-Java) | [Blog](https://blog.aspose.com/category/psd/) | [Arama](https://search.aspose.com/) | [Ücretsiz Destek](https://forum.aspose.com/c/psd) | [Geçici lisans](https://purchase.aspose.com/temporary-license)
