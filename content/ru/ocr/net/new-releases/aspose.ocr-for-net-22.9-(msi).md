---
title: "Распознавание текста квитанции через API OCR для приложений C#, ASP.NET"
description: "C# .NET API to extract printed receipts text, recognition accuracy of small fonts, recognize Cyrillic characters, Detect all images in folder & convert to PDF."
keywords: ""
page_type: single_release_page
folder_link: "/ocr/net/new-releases/aspose.ocr-for-net-22.9-(msi)/"
folder_name: "Aspose.ocr для net 22,9 (MSI)"
download_link: "/ocr/net/new-releases/aspose.ocr-for-net-22.9-(msi)/4e2c810dcf93208a23b812945f0de7bb-33-7949"
download_text: "Скачать"
intro_text: "Smallfonts, 90Degree, UncisingCeipt"
image_link: "/resources/img/msi-icon.png"
download_count: " 28/9/2022 Скачатьs: 1  Views: 1 "
file_size: "File Size: 162.34MB"
parent_path: "ocr/net"
section_parent_path: "ocr/net"
tags: ""
release_notes_url: "https://docs.aspose.com/ocr/net/release-notes/latest/"
weight: 289
---

{{< Releases/ReleasesWapper >}}
  {{< Releases/ReleasesHeading H2txt="Aspose.ocr для net 22,9 (MSI)" imagelink="/resources/img/msi-icon.png">}}
  {{< Releases/ReleasesButtons >}}
    {{< Releases/ReleasesSingleButtons text="Скачать" link="/ocr/net/new-releases/aspose.ocr-for-net-22.9-(msi)/4e2c810dcf93208a23b812945f0de7bb-33-7949" >}}
    {{< Releases/ReleasesSingleButtons text="Форум поддержки" link="https://forum.aspose.com/c/ocr" >}}
  {{< Releases/ReleasesButtons >}}
  {{< Releases/ReleasesFileArea >}}
    {{< Releases/ReleasesHeading h4txt="Детали файла">}}
    {{< Releases/ReleasesDetailsUl >}}
      {{< Common/li >}} Скачатьs: {{< /Common/li >}}
      {{< Common/li class="downloadcount" id="dwn-update-4e2c810dcf93208a23b812945f0de7bb-33-7949" >}} 1 {{< /Common/li >}}
      {{< Common/li >}} Размер файла: {{< /Common/li >}}
      {{< Common/li id="size-update-4e2c810dcf93208a23b812945f0de7bb-33-7949" >}} 162.34MB {{< /Common/li >}}

      {{< Common/li >}} Дата добавления: {{< /Common/li >}}
      {{< Common/li id="added-update-4e2c810dcf93208a23b812945f0de7bb-33-7949" >}}28/9/2022 {{< /Common/li >}}
    {{< /Releases/ReleasesDetailsUl >}}

  {{< Releases/ReleasesFileFeatures >}}
      <h4>Выпуск заметок</h4><div><a href='https://docs.aspose.com/ocr/net/release-notes/latest/'>https://docs.aspose.com/ocr/net/release-notes/latest/</a></div>
  {{< /Releases/ReleasesFileFeatures >}}
  {{< Releases/ReleasesFileFeatures >}}
      <h4>Описание</h4><div class="HTMLDescription">Smallfonts, 90Degree, UncisingCeipt</div>
  {{< /Releases/ReleasesFileFeatures >}}

{{< Releases/ReleasesHeading h4txt="Notable Features">}}
{{< Common/wrapper class="HTMLDescription">}}
{{% Releases/ReleasesFileFeatures %}}

# Receipt Text Recognition via OCR

Introduced a specialized method `RecognizeReceipt` that is used to extract text specifically from printed receipts.

```csharp
Aspose.OCR.AsposeOcr recognitionEngine = new Aspose.OCR.AsposeOcr();
Aspose.OCR.ReceiptRecognitionSettings recognitionSettings = new Aspose.OCR.ReceiptRecognitionSettings();
recognitionSettings.Language = Aspose.OCR.Language.Ukr;
Aspose.OCR.RecognitionResult result = recognitionEngine.RecognizeReceipt("receipt.png", recognitionSettings);
Console.WriteLine(result.RecognitionText);
```

# Small Fonts Recognition

Introduced a new image detection setting, `UpscaleSmallFont`, that enhances the recognition accuracy of small fonts and lines.

```csharp
Aspose.OCR.AsposeOcr recognitionEngine = new Aspose.OCR.AsposeOcr();
Aspose.OCR.RecognitionSettings recognitionSettings = new Aspose.OCR.RecognitionSettings();
recognitionSettings.UpscaleSmallFont = true;
Aspose.OCR.RecognitionResult result = recognitionEngine.RecognizeImage("source.png", recognitionSettings);
Console.WriteLine(result.RecognitionText);
```

# Cyrillic Characters Recognition

Improved the image recognition via OCR by adding the ability to recognize all Cyrillic characters.

```csharp
Aspose.OCR.AsposeOcr recognitionEngine = new Aspose.OCR.AsposeOcr();
Aspose.OCR.RecognitionSettings recognitionSettings = new Aspose.OCR.RecognitionSettings();
recognitionSettings.Language = Aspose.OCR.Language.Cyrillic;
Aspose.OCR.RecognitionResult result = recognitionEngine.RecognizeImage("source.png", recognitionSettings);
Console.WriteLine(result.RecognitionText);
```

# Batch Image Recognition & Conversion

Added the ability to recognize all images from a specific folder via OCR API and save then all as PDF pages.

```csharp
Aspose.OCR.AsposeOcr recognitionEngine = new Aspose.OCR.AsposeOcr();
Aspose.OCR.RecognitionSettings recognitionSettings = new Aspose.OCR.RecognitionSettings();
// Recognize all images from the folder
List<Aspose.OCR.RecognitionResult> results = recognitionEngine.RecognizeMultipleImages("C:/images/", recognitionSettings);
// Save all pages as PDF
Aspose.OCR.AsposeOcr.SaveMultipageDocument("result.pdf", Aspose.OCR.SaveFormat.Pdf, results);
```

For a complete list of features, enhancements, and bug fixes in this release please visit, [Aspose.OCR for .NET 22.9 - Выпуск заметок](https://docs.aspose.com/ocr/net/aspose-ocr-for-net-22-9-release-notes/).

{{% /Releases/ReleasesFileFeatures %}}

{{< /Common/wrapper >}}
{{< /Releases/ReleasesFileFeatures >}}

{{< /Releases/ReleasesFileArea >}}
{{< /Releases/ReleasesWapper >}}
