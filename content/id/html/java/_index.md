---
title: "Aspose.html | Perpustakaan Kelas Java untuk memanipulasi file HTML" 
linktitle: Aspose.HTML
description: "Perpustakaan kelas Java untuk menulis, mengedit, parse, membaca, menerjemahkan dan mengonversi format html, xhtml, mhtml, dan epub. Juga mendukung memanipulasi DOM melalui JavaScript." 
layout: packages
type: repository
categories:
  - fundamentals
keywords:
- Aspose Total
- Aspose HTML
- Aspose Java API
- html java library
- html java class
- Maven
- html converter
- svg converter
- mhtml converter
- markdown converter
- template converter
- html to image
- html to pdf
- html to xps
- html to mhtml
- html to markdown
- svg to image
- svg to pdf
- svg to xps
- epub to image
- epub to pdf
- epub to xps
- mhtml to image
- mhtml to pdf
- mhtml to xps
- markdown to html
- html template
- html navigation
- html5
- DOM
- html form editor
- css extension
family_listing_page_title: "Aspose.html untuk Java" 
family_listing_page_description: "Aspose.html untuk Java adalah API manipulasi HTML canggih yang dibangun untuk melakukan berbagai tugas manipulasi HTML secara langsung dalam aplikasi Java." 
family_listing_page_iconurl: "https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/html/272x272/aspose_html-for-java.png"
family_listing_page_selfHosted: "1"
family_listing_page_type: "1"
family_listing_page_venture: "4"
family_listing_page_package: "9"
homepage_package_type: "Maven"
homepage_package_link: "https://releases.aspose.com/java/repo/com/aspose/aspose-html/"
weight: 02	#rem
forumLink: https://forum.aspose.com/c/html/29
productLink: https://products.aspose.com/html/java/
releaseNotesLink: https://docs.aspose.com/html/java/release-notes/
dataFolder: aspose_html
packages_refs:
- "22-9"
- "22-8"
- "22-7"
- "17-10"
- "17-11"
- "17-11-1"
- "17-12"
- "17-8"
- "17-9"
- "18-10"
- "18-10-1"
- "18-10-2"
- "18-11"
- "18-11-1"
- "18-5"
- "18-5-1"
- "18-6"
- "18-8"
- "19-3"
- "19-4"
- "19-5"
- "19-6"
- "19-7"
- "19-8"
- "19-9"
- "20-12"
- "20-6"
- "20-8"
- "20-9-1"
- "21-12"
- "21-3"
- "21-4"
- "21-5"
- "21-6"
---

# HTML File Manipulation Java API
{{< repository/extract-package-explore-link imgsrc=./aspose_html-for-java-banner.png >}}

[Halaman produk](https://products.aspose.com/html/java) | [Dokumen](https://docs.aspose.com/html/java/) | [Demo](https://products.aspose.app/html/family) | [Referensi API](https://apireference.aspose.com/html/java) | [Contoh](https://github.com/aspose-html/Aspose.Html-for-Java) | [Blog](https://blog.aspose.com/category/html/) | [Mencari](https://search.aspose.com/) | [Dukungan gratis](https://forum.aspose.com/c/html) | [Lisensi sementara](https://purchase.aspose.com/temporary-license)

[Java HTML API](https://products.aspose.com/html/java) membantu pengembang untuk menulis, membaca, memodifikasi, menavigasi, dan mengonversi (x) dokumen HTML dari dalam aplikasi Java.

Aspose.html untuk Java API berfungsi sebagai browser tanpa kepala yang memungkinkan Anda untuk [Buat atau buka dokumen HTML yang ada](https://docs.aspose.com/html/java/creating-a-document/) dari berbagai sumber untuk melakukan operasi manipulasi seperti menghapus dan mengganti node HTML, menyimpan dokumen HTML, mengekstrak CSS dari HTML, mengkonfigurasi dokumen sandbox dan banyak lagi. Anda dapat menavigasi dokumen HTML dengan menggunakan berbagai metode, seperti, elemen traversal, dokumen traversal, kueri xpath, dan kueri pemilih CSS serta memanipulasi dom html melalui javascript, mengonversi file html ke gambar atau format tata letak tetap, dan mengonversi xhtml dan epub file ke format file lain.

## fitur pemrosesan html
- Ditulis sepenuhnya di Java dan bekerja dengan JRE.
-Mendukung dukungan OS `32-bit` &` 64-bit`.
- Buat atau buka dokumen HTML yang ada dari berbagai sumber.
- Kemampuan untuk memanipulasi (membuat, mengedit, menghapus, mengganti) node html melalui API.
- Ekstrak gaya CSS untuk simpul HTML tertentu.
- Mengkonfigurasi kotak pasir dokumen yang memengaruhi pemrosesan dokumen HTML.
- Mendukung navigasi melalui dokumen HTML dalam berbagai cara (elemen traversal, traversal dokumen, kueri XPath, kueri pemilih CSS).
- memanipulasi html dom melalui javascript.
- Konversi dokumen web ke berbagai format file yang didukung.
- Ekstrak teks dari halaman.
- Cari teks dari halaman.
- Tambahkan teks dalam file html.
- Create, edit, remove and replace HTML nodes
- Extracting CSS styles for particular HTML node
- Convert HTML documents into various supported image formats: JPEG, PNG, BMP, TIFF
- Convert HTML documents to PDF format
- Konversi dokumen HTML ke format XPS.

## Baca & Tulis Format Web
** web: ** html, xhtml^, mHtml ^^ \
** Lainnya: ** SVG*, MD **

## simpan html sebagai
** Tata letak tetap: ** pdf, xps \
** Gambar: ** tiff, jpeg, png, bmp

## Baca format
** Gambar: ** epub

## Lingkungan yang Didukung
- ** Microsoft Windows: ** Windows Desktop & Server (x86, x64)
- ** MacOS: ** Mac OS X
- ** Linux: ** Ubuntu, OpenSuse, Centos, dan lainnya
- ** Versi Java: ** `j2se 6.0 (1.6)`, `j2se 7.0 (1.7)`, `j2se 8.0 (1.8)`

## Memulai

Aspose.html Java API di -host di [Repositori Aspose](https://repository.aspose.com/html/). Anda dapat dengan mudah menggunakan Aspose.html untuk Java API langsung di proyek Maven Anda dengan konfigurasi sederhana. Untuk instruksi terperinci, silakan kunjungi halaman dokumentasi [Installing Aspose.HTML for Java from Repositori Aspose](https://docs.aspose.com/html/java/installation/).

## Muat html dari lokasi jarak jauh

```java
HTMLDocument document = HTMLDocument(new Url("template.html"));
// read children nodes and get length information
if (document.getBody().getChildNodes().getLength() == 0)
    System.out.println("No ChildNodes found...");
// print Document URI to console. As per information above, it has to be https://www.w3.org/TR/html5/
System.out.println("Print Document URI = " + document.getDocumentURI());
// print domain name for remote HTML
System.out.println("Domain Name = " + document.getDomain());
```

## How to use the Contoh?

Clone or Download the ZIP and extract the contents to your local hard drive. This project uses Maven/Gradle build system and can be opened in any modern IDE like IntelliJ IDEA, Eclipse or NetBeans. For more details, visit our [Documentation website](https://docs.aspose.com/display/htmljava/How+to+Run+the+Contoh).

## Step one

For maven
```
mvn compile test
```
For gradle
```
gradle build
```


## Execute all tests
Maven
```
mvn -Dtest="com.aspose.html.examples.**" test
```

Gradle
```
./gradlew test --tests "com.aspose.html.examples.*"
```

## Execute single test
Maven
```
mvn -Dtest=Contoh_Java_AdvancedUsage_DOMMutationObserver_ObserveHowNodesAreAdded test
```
Gradle
```
./gradlew test --tests "com.aspose.html.examples.Contoh_Java_AdvancedUsage_DOMMutationObserver_ObserveHowNodesAreAdded"
```
## Execute asynchronously test in Thread
Maven
```
mvn org.codehaus.mojo:exec-maven-plugin:3.0.0:java -Dexec.mainClass="com.aspose.html.examples.SimpleWait" -Dexec.classpathScope="test" -Dexec.cleanupDaemonThreads=false
```
Gradle
```
./gradlew SimpleWait
```

[Halaman produk](https://products.aspose.com/html/java) | [Dokumen](https://docs.aspose.com/html/java/) | [Demo](https://products.aspose.app/html/family) | [Referensi API](https://apireference.aspose.com/html/java) | [Contoh](https://github.com/aspose-html/Aspose.Html-for-Java) | [Blog](https://blog.aspose.com/category/html/) | [Mencari](https://search.aspose.com/) | [Dukungan gratis](https://forum.aspose.com/c/html) | [Lisensi sementara](https://purchase.aspose.com/temporary-license)
