---
title: "Refactor para API de soporte de PS, EPS y XPS para aplicaciones C#, ASP.NET"
description: "C# .NET API has been refactored to  include the support for the PS (PostScript), EPS (Encapsulated PostScript), and XPS (XML Paper Specification) formats."
keywords: "    . "
page_type: single_release_page
folder_link: " tex/net/new-releases/aspose.tex-for-.net-22.4/"
folder_name: "Aspose.tex para .NET 22.4"
download_link: " /tex/net/new-releases/aspose.tex-for-.net-22.4/854e74b1103042fa952c697f3ae51497"
download_text: " Descargar"
intro_text: "Contiene aspose.tex para .NET 22.4 lanzamiento."
image_link: "/resources/img/msi-icon.png"
download_count: "   Added: 5 days ago [4/6/2022]  Descargars: 1  Views: 4"
file_size: "  File Size: 67.9 MB "
parent_path: "tex/net"
section_parent_path: "tex/net"
release_notes_url: "https://docs.aspose.com/tex/net/aspose-tex-for-net-22-4-release-notes"
weight: 19
---

{{< Releases/ReleasesWapper >}}
{{< Releases/ReleasesHeading H2txt="Aspose.tex para .NET 22.4" imagelink="/resources/img/msi-icon.png">}}
{{< Releases/ReleasesButtons >}}
{{< Releases/ReleasesSingleButtons text=" Descargar" link="/tex/net/new-releases/aspose.tex-for-.net-22.4/854e74b1103042fa952c697f3ae51497%20%20" >}}
{{< Releases/ReleasesSingleButtons text=" Support Forum " link="https://forum.aspose.com/c/tex" >}}
{{< Releases/ReleasesButtons >}}
{{< Releases/ReleasesFileArea >}}
{{< Releases/ReleasesHeading h4txt="detalles del archivo">}}
{{< Releases/ReleasesDetailsUl >}}
{{< Common/li  >}} Descargars: {{< /Common/li >}}
{{< Common/li class="downloadcount" id="dwn-update-854e74b1103042fa952c697f3ae51497" >}} 1 {{< /Common/li >}}
{{< Common/li  >}} Tamaño del archivo: {{< /Common/li >}}
{{< Common/li id="size-update-854e74b1103042fa952c697f3ae51497" >}} 67.9 MB {{< /Common/li >}}
{{< Common/li  class="hide" >}} Posted By: {{< /Common/li >}}
{{< Common/li class="hide" id="author-update-854e74b1103042fa952c697f3ae51497" >}} kolod {{< /Common/li >}}
{{< Common/li class="hide"  >}} Views: {{< /Common/li >}}
{{< Common/li class="hide" id="view-update-854e74b1103042fa952c697f3ae51497" >}} 5 {{< /Common/li >}}
{{< Common/li  >}} Fecha Agregada: {{< /Common/li >}}
{{< Common/li id="added-update-854e74b1103042fa952c697f3ae51497" >}} : 5 days ago [4/6/2022] {{< /Common/li >}}

    {{< /Releases/ReleasesDetailsUl >}}

{{< Releases/ReleasesFileFeatures >}}

<h4>Notas de lanzamiento</h4><div><a href="https://docs.aspose.com/tex/net/aspose-tex-for-net-22-4-release-notes/">https://docs.aspose.com/tex/net/aspose-tex-for-net-22-4-release-notes/</a></div>
{{< /Releases/ReleasesFileFeatures >}}
{{< Releases/ReleasesFileFeatures >}}

{{< Releases/ReleasesHeading h4txt="Notable Features">}}
{{< Common/wrapper class="HTMLDescription">}}
{{% Releases/ReleasesFileFeatures %}}

# Refactor the PS/EPS & XPS Support

Refactored the API to include the support for the PS (PostScript), EPS (Encapsulated PostScript), and XPS (XML Paper Specification) formats. The following C# code snippet works as LTX to XPS converter, i.e. convert LaTeX to XPS using API:

```csharp
// Create conversion options instance.
...
// Initialize the options for saving in XPS format.
options.SaveOptions = new XpsSaveOptions(); // Default value. Arbitrary assignment.
// Run LaTeX to XPS conversion.
new TeXJob(Path.Combine(RunExamples.InputDirectory, "sample.ltx"), new XpsDevice(), options).Run();
```

# Added the `MathRenderer` Type

This release offers the addition of a `MathRenderer` type, that implements the rendering of Math Formula.

> For a complete list of features, enhancements, and bug fixes in this release please visit, [Aspose.TeX for .NET 22.4 Notas de lanzamiento](https://docs.aspose.com/tex/net/aspose-tex-for-net-22-4-release-notes/).

{{% /Releases/ReleasesFileFeatures %}}

{{< /Common/wrapper >}}
{{< /Releases/ReleasesFileFeatures >}}

{{< /Releases/ReleasesFileArea >}}
{{< /Releases/ReleasesWapper >}}
