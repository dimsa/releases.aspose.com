---
title: "Konversi XPS ke Image Set Image Size API untuk C#, ASP.NET Apps"
description: "C# .NET API untuk mengonversi XPS ke format gambar dengan opsi untuk mengatur ukuran gambar yang diperlukan. Mendukung konversi XPS ke format gambar raster BMP, JPG, PNG, dan TIFF."
keywords: ""
page_type: single_release_page
folder_link: "/page/net/new-releases/aspose.page-for-.net-22.7/"
folder_name: "Aspose.Halaman untuk .Net 22.7"
download_link: "/page/net/new-releases/aspose.page-for-.net-22.7/a6b95730770cef3fa391241ceb764056-7-7640"
download_text: "Download"
Intro_text: "Ini berisi Aspose.Page untuk .NET 22.7 rilis."
image_link: "/resources/img/msi-icon.png"
download_count: " 14/7/2022 Downloads: 1  Views: 1 "
file_size: "File Size: 31.74MB"
parent_path: "page/net"
section_parent_path: "page/net"
tags: ""
release_notes_url: "https://docs.aspose.com/page/net/aspose-page-for-net-22-7-release-notes/"
weight: 106
---

{{< Releases/ReleasesWapper >}}
{{< Releases/ReleasesHeading H2txt="Aspose.Halaman untuk .Net 22.7" imagelink="/resources/img/msi-icon.png">}}
{{< Releases/ReleasesButtons >}}
{{< Releases/ReleasesSingleButtons text="Download" link="/page/net/new-releases/aspose.page-for-.net-22.7/a6b95730770cef3fa391241ceb764056-7-7640" >}}
{{< Releases/ReleasesSingleButtons text="Support Forum" link="https://forum.aspose.com/c/page" >}}
{{< Releases/ReleasesButtons >}}
{{< Releases/ReleasesFileArea >}}
{{< Releases/ReleasesHeading h4txt="Detail File">}}
{{< Releases/ReleasesDetailsUl >}}
{{< Common/li >}} Downloads: {{< /Common/li >}}
{{< Common/li class="downloadcount" id="dwn-update-a6b95730770cef3fa391241ceb764056-7-7640" >}} 1 {{< /Common/li >}}
{{< Common/li >}} File Size: {{< /Common/li >}}
{{< Common/li id="size-update-a6b95730770cef3fa391241ceb764056-7-7640" >}} 31.74MB {{< /Common/li >}}

      {{< Common/li >}} Date Added: {{< /Common/li >}}
      {{< Common/li id="added-update-a6b95730770cef3fa391241ceb764056-7-7640" >}}14/7/2022 {{< /Common/li >}}
    {{< /Releases/ReleasesDetailsUl >}}

{{< Releases/ReleasesFileFeatures >}}
<h4>Catatan Rilis</h4><div> <a href='https://docs.aspose.com/page/net/aspose-page-for-net-22-7-release-notes/'>https://docs.aspose.com/page/net/aspose-page-for-net-22-7-release-notes/</a></div>
{{< /Releases/ReleasesFileFeatures >}}
{{< Releases/ReleasesFileFeatures >}}

{{< Releases/ReleasesHeading h4txt="Fitur Penting">}}
{{< Common/wrapper class="HTMLDescription">}}
{{% Releases/ReleasesFileFeatures %}}

 

# Konversi XPS ke Format Gambar

Konversi XPS ke format gambar dengan opsi untuk mengatur ukuran gambar yang diperlukan. Mendukung konversi XPS ke format gambar raster BMP, JPG, PNG, dan TIFF. Berikut ini adalah kode C# konverter XPS ke PNG yang menggunakan API pemrosesan XPS:

```csharp
// The path to the documents directory.
string dataDir = RunExamples.GetDataDir_WorkingWithDocumentConversion();
// Input file
string inputFileName = dataDir + "input.xps";
//Outut file 
string outputFileName = dataDir + "XPStoImage_out.png";
// Initialize XPS input stream
using (Stream xpsStream = File.Open(inputFileName, FileMode.Open, FileAccess.Read))
{
    // Load XPS document form the stream
    XpsDocument document = new XpsDocument(xpsStream, new XpsLoadOptions());
    // or load XPS document directly from file. No xpsStream is needed then.
    // XpsDocument document = new XpsDocument(inputFileName, new XpsLoadOptions());

    // Initialize options object with necessary parameters.
    PngSaveOptions options = new PngSaveOptions()
    {
        SmoothingMode = System.Drawing.Drawing2D.SmoothingMode.HighQuality,
        Resolution = 300,
        PageNumbers = new int[] { 1, 2, 6 }
    };

    // Create rendering device for image
    ImageDevice device = new ImageDevice();

    document.Save(device, options);

    // Iterate through document partitions (fixed documents, in XPS terms)
    for (int i = 0; i < device.Result.Length; i++)
        // Iterate through partition pages
        for (int j = 0; j < device.Result[i].Length; j++)
        {
            // Initialize image output stream
            using (Stream imageStream = System.IO.File.Open(Path.GetDirectoryName(outputFileName) +
                Path.GetFileNameWithoutExtension(outputFileName) + "_" + (i + 1) + "_" + (j + 1) +
                Path.GetExtension(outputFileName), System.IO.FileMode.Create, System.IO.FileAccess.Write))
                // Write image
                imageStream.Write(device.Result[i][j], 0, device.Result[i][j].Length);
        }
}
```

> Untuk daftar lengkap fitur, penyempurnaan, dan perbaikan bug dalam rilis ini, kunjungi [Aspose.Page for .NET 22.7 Release Notes](https://docs.aspose.com/page/net/aspose-page-for-net-22-7-release-notes/).

{{% /Releases/ReleasesFileFeatures %}}

{{< /Common/wrapper >}}
{{< /Releases/ReleasesFileFeatures >}}

{{< /Releases/ReleasesFileArea >}}
{{< /Releases/ReleasesWapper >}}

