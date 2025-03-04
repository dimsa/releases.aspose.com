---
title: "Converta HTML em imagem | API de código alto para C#, APPS ASP.NET"
description: "C# .NET API for HTML to Image conversion, enhanced processing speed of the CSS & document generation performance, improved parsing & rendering algorithms."
keywords: ""
page_type: single_release_page
folder_link: "/html/net/new-releases/aspose.html-for-.net-22.8/"
folder_name: "Aspose.html para .NET 22.8"
download_link: "/html/net/new-releases/aspose.html-for-.net-22.8/3965995fe83fa8a58ac02e972a24701f-4-7784"
download_text: "Download"
intro_text: "Ele contém aspose.html para .NET 22.8 Release."
image_link: "/resources/img/msi-icon.png"
download_count: " 19/8/2022 Downloads: 1  Views: 1 "
file_size: "File Size: 16.12MB"
parent_path: "html/net"
section_parent_path: "html/net"

tags: ""
release_notes_url: "https://docs.aspose.com/html/net/aspose-html-for-net-22-8-release-notes"
weight: 238
---

{{< Releases/ReleasesWapper >}}
{{< Releases/ReleasesHeading H2txt="Aspose.html para .NET 22.8" imagelink="/resources/img/msi-icon.png">}}
{{< Releases/ReleasesButtons >}}
{{< Releases/ReleasesSingleButtons text="Download" link="/html/net/new-releases/aspose.html-for-.net-22.8/3965995fe83fa8a58ac02e972a24701f-4-7784" >}}
{{< Releases/ReleasesSingleButtons text="Fórum de suporte" link="https://forum.aspose.com/c/html" >}}
{{< Releases/ReleasesButtons >}}
{{< Releases/ReleasesFileArea >}}
{{< Releases/ReleasesHeading h4txt="Detalhes do arquivo">}}
{{< Releases/ReleasesDetailsUl >}}
{{< Common/li >}} Downloads: {{< /Common/li >}}
{{< Common/li class="downloadcount" id="dwn-update-3965995fe83fa8a58ac02e972a24701f-4-7784" >}} 1 {{< /Common/li >}}
{{< Common/li >}} Tamanho do arquivo: {{< /Common/li >}}
{{< Common/li id="size-update-3965995fe83fa8a58ac02e972a24701f-4-7784" >}} 16.12MB {{< /Common/li >}}

      {{< Common/li >}} data adicionada: {{< /Common/li >}}
      {{< Common/li id="added-update-3965995fe83fa8a58ac02e972a24701f-4-7784" >}}19/8/2022 {{< /Common/li >}}
    {{< /Releases/ReleasesDetailsUl >}}

{{< Releases/ReleasesFileFeatures >}}
<h4>Notas de liberação</h4><div><a href='https://docs.aspose.com/html/net/aspose-html-for-net-22-8-release-notes'>https://docs.aspose.com/html/net/aspose-html-for-net-22-8-release-notes</a></div>
{{< /Releases/ReleasesFileFeatures >}}
{{< Releases/ReleasesFileFeatures >}}

{{< Releases/ReleasesHeading h4txt="Notable Features">}}
{{< Common/wrapper class="HTMLDescription">}}
{{% Releases/ReleasesFileFeatures %}}

# Improved Processing Speed of CSS Styles

Improved the CSS styles processing speed. Following is a C# code sample of inline CSS usage via API:

```csharp
using System.IO;
using Aspose.Html;
using Aspose.Html.Rendering.Pdf;
...
    // Create an instance of an HTML document with specified content
    var content = "<p> Inline CSS </p>";
    using (var document = new HTMLDocument(content, "."))
    {
        // Find the paragraph element to set a style attribute
        var paragraph = (HTMLElement)document.GetElementsByTagName("p").First();

        // Set the style attribute
        paragraph.SetAttribute("style", "font-size: 250%; font-family: verdana; color: #cd66aa");
                        
        // Save the HTML document to a file 
        document.Save(Path.Combine(OutputDir, "edit-inline-css.html"));
    
        // Create the instance of the PDF output device and render the document into this device
        using (var device = new PdfDevice(Path.Combine(OutputDir, "edit-inline-css.pdf")))
        {
            // Render HTML to PDF
    		document.RenderTo(device);
        }                     
    }
```

# Improved HTML to Image Conversion

Improved the conversion of HTML to Image formats and resolved the rendering issues. The following simple C# code sample converts HTML to PNG format:

```csharp
using System.IO;
using Aspose.Html.Converters;
using Aspose.Html.Rendering.Image;
using Aspose.Html.Saving;
...
    // Invoke the ConvertHTML method to convert the HTML code to PNG image           
    Converter.ConvertHTML(@"<h1>Convert HTML to PNG!</h1>", ".", new ImageSaveOptions(), Path.Combine(OutputDir, "convert-with-single-line.png"));
```

> For a complete list of features, enhancements, and bug fixes in this release please visit, [Aspose.HTML for .NET 22.8 Notas de liberação](https://docs.aspose.com/html/net/aspose-html-for-net-22-8-release-notes/).

{{% /Releases/ReleasesFileFeatures %}}

{{< /Common/wrapper >}}
{{< /Releases/ReleasesFileFeatures >}}

{{< /Releases/ReleasesFileArea >}}
{{< /Releases/ReleasesWapper >}}
