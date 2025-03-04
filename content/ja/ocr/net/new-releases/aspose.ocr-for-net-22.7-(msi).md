---
title: "画像ノイズ＆スキュー修正ocr api for c＃、asp.netアプリ"
description: "C# .NET API with image noise reduction filter, auto denoising of OCR detected images, filter to correct the image skew by straightening (deskew) skewed images."
keywords: ""
page_type: single_release_page
folder_link: "/ocr/net/new-releases/aspose.ocr-for-net-22.7-(msi)/"
folder_name: "ネット22.7のasophes.ocr（MSI）"
download_link: "/ocr/net/new-releases/aspose.ocr-for-net-22.7-(msi)/7b7cc9c4a71d3758c3c50c09abfe09c3-33-7687"
download_text: "ダウンロード"
intro_text: "新しいPREPROCESSINGFILTERS：オートデノーミングとオートスキュー"
image_link: "/resources/img/msi-icon.png"
download_count: " 22/7/2022 ダウンロードs: 1  Views: 1 "
file_size: "File Size: 162.33MB"
parent_path: "ocr/net"
section_parent_path: "ocr/net"
tags: ""
release_notes_url: "https://docs.aspose.com/ocr/net/release-notes/latest/"
weight: 284
---

{{< Releases/ReleasesWapper >}}
  {{< Releases/ReleasesHeading H2txt="ネット22.7のasophes.ocr（MSI）" imagelink="/resources/img/msi-icon.png">}}
  {{< Releases/ReleasesButtons >}}
    {{< Releases/ReleasesSingleButtons text="ダウンロード" link="/ocr/net/new-releases/aspose.ocr-for-net-22.7-(msi)/7b7cc9c4a71d3758c3c50c09abfe09c3-33-7687" >}}
    {{< Releases/ReleasesSingleButtons text="サポートフォーラム" link="https://forum.aspose.com/c/ocr" >}}
  {{< Releases/ReleasesButtons >}}
  {{< Releases/ReleasesFileArea >}}
    {{< Releases/ReleasesHeading h4txt="ファイルの詳細">}}
    {{< Releases/ReleasesDetailsUl >}}
      {{< Common/li >}} ダウンロードs: {{< /Common/li >}}
      {{< Common/li class="downloadcount" id="dwn-update-7b7cc9c4a71d3758c3c50c09abfe09c3-33-7687" >}} 1 {{< /Common/li >}}
      {{< Common/li >}} ファイルサイズ: {{< /Common/li >}}
      {{< Common/li id="size-update-7b7cc9c4a71d3758c3c50c09abfe09c3-33-7687" >}} 162.33MB {{< /Common/li >}}

      {{< Common/li >}} 日付が追加されました: {{< /Common/li >}}
      {{< Common/li id="added-update-7b7cc9c4a71d3758c3c50c09abfe09c3-33-7687" >}}22/7/2022 {{< /Common/li >}}
    {{< /Releases/ReleasesDetailsUl >}}

  {{< Releases/ReleasesFileFeatures >}}
      <h4>リリースノート</h4><div><a href='https://docs.aspose.com/ocr/net/release-notes/latest/'>https://docs.aspose.com/ocr/net/release-notes/latest/</a></div>
  {{< /Releases/ReleasesFileFeatures >}}
  {{< Releases/ReleasesFileFeatures >}}
      <h4>説明</h4><div class="HTMLDescription">新しいPREPROCESSINGFILTERS：オートデノーミングとオートスキュー</div>
  {{< /Releases/ReleasesFileFeatures >}}

{{< Releases/ReleasesHeading h4txt="Notable Features">}}
{{< Common/wrapper class="HTMLDescription">}}
{{% Releases/ReleasesFileFeatures %}}

# Image Noise Reduction Filter

A new preprocessing filter has been added to the OCR API that automatically removes various types of image noise; such as, unwanted gradients, glare, scratches, dirty spots, dirt, etc.

The following C# code snippet shows the Auto Denoising method of API in action:

```csharp
using Aspose.OCR;

namespace ProgramOCR
{
    class Program
    {
        static void Main(string[] args)
        {
            // Create instance of OCR API
            AsposeOcr api = new AsposeOcr();
            // Add denoise preprocessing filter
            PreprocessingFilter filters = new PreprocessingFilter {
            	PreprocessingFilter.AutoDenoising()
            };
            // Preprocess an image
            MemoryStream ms = api.PreprocessImage("image.jpg", filters)
            // Save cleaned image into a file
            using(FileStream file = new FileStream("result.png", FileMode.Create, System.IO.FileAccess.Write))
            {
            	ms.WriteTo(file);
            }
        }
    }
}
```

# Image Skew Correction Filter

Introduced the filter that corrects the image skew by straightening (deskew) the skewed images.

The following C# code sample demonstrates how you may increase the image recognition accuracy of photos taken from smartphone or inaccurate scans by using `AutoSkew()` method in API:

```csharp
using Aspose.OCR;

namespace ProgramOCR
{
    class Program
    {
        static void Main(string[] args)
        {
            // Create instance of OCR API
            AsposeOcr api = new AsposeOcr();
            // Add deskew preprocessing filter
            PreprocessingFilter filters = new PreprocessingFilter {
            	PreprocessingFilter.AutoSkew()
            };
            // Preprocess an image
            MemoryStream ms = api.PreprocessImage("image.jpg", filters)
            // Save straightened image into a file
            using(FileStream file = new FileStream("result.png", FileMode.Create, System.IO.FileAccess.Write))
            {
            	ms.WriteTo(file);
            }
        }
    }
}
```

# Better Compatibility with Aspose.OMR

Resolved the incompatibility issue between Aspose.OCR and Aspose.OMR installers.

For a complete list of features, enhancements, and bug fixes in this release please visit, [Aspose.OCR for .NET 22.7 - リリースノート](https://docs.aspose.com/ocr/net/aspose-ocr-for-net-22-7-release-notes/).

{{% /Releases/ReleasesFileFeatures %}}

{{< /Common/wrapper >}}
{{< /Releases/ReleasesFileFeatures >}}

{{< /Releases/ReleasesFileArea >}}
{{< /Releases/ReleasesWapper >}}
