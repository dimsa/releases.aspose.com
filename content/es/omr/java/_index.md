---
title: "Aspose.omr | Biblioteca de clase Java para la extracción de marcas digitales" 
linktitle: Aspose.OMR
description: "Biblioteca de clase Java para reconocimiento de marcas ópticas (OMR). Reconocer y extraer marcas de imágenes digitalizadas o escaneadas, fotos, encuestas, exámenes y cuestionarios." 
layout: packages
type: repository
categories:
  - fundamentals
keywords:
- Aspose Total
- Aspose OMR
- Aspose Java API
- omr java library
- omr java class
- JPEG
- PNG
- GIF
- TIFF
- BMP
- CSV
- JSON
- XML
- image recognition
- image perspective
- test
- exam
- questionnaire
- survey
- J2SE
- Windows
- Linux
- Mac
- Azure
- Maven
- optical mark recognition
- extract marks
- marks extraction
family_listing_page_title: "Aspose.omr para Java" 
family_listing_page_description: "Aspose.omr para Java es una API para reconocer las marcas ópticas de las imágenes de hoja digitalizadas OMR. Se puede usar para reconocer las marcas ópticas en una variedad de formatos de imagen como BMP, JPG, TIF, TIFF, GIF. La API permite capturar datos marcados por humanos de formularios de documentos como encuestas, cuestionarios, documentos de examen de opción múltiple y otras pruebas." 
family_listing_page_iconurl: "https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/omr/272x272/aspose_omr-for-java.png"
family_listing_page_selfHosted: "1"
family_listing_page_type: "1"
family_listing_page_venture: "4"
family_listing_page_package: "192"
homepage_package_type: "Maven"
homepage_package_link: "https://releases.aspose.com/java/repo/com/aspose/aspose-omr/"
weight: 02	#rem
forumLink: https://forum.aspose.com/c/omr/38
productLink: https://products.aspose.com/omr/java/
releaseNotesLink: https://docs.aspose.com/omr/java/release-notes/
dataFolder: aspose_omr
packages_refs:
- "19-12"
- "2-3-0"
---

# API Java para realizar OMR
{{< repository/extract-package-explore-link imgsrc=./aspose_omr-for-java-banner.png >}}

[Hogar](https://www.aspose.com/) | [Página del producto](https://products.aspose.com/omr/java) | [Documentos](https://docs.aspose.com/omr/java/) | [Población](https://products.aspose.app/omr/family) | [Referencia de API](https://apireference.aspose.com/omr/java) | [Ejemplos](https://github.com/aspose-omr/Aspose.OMR-for-Java) | [Blog](https://blog.aspose.com/category/omr/) | [Búsqueda](https://search.aspose.com/) | [Soporte gratuito](https://forum.aspose.com/c/omr) | [Licencia temporal](https://purchase.aspose.com/temporary-license)

[Aspose.OMR for Java](https://products.aspose.com/omr/java) es una biblioteca de clase Java que proporciona API para reconocer las marcas ópticas de las imágenes de hoja digitalizadas OMR. Se puede usar para reconocer las marcas ópticas en una variedad de formatos de imagen como BMP, JPG, TIF, TIFF, GIF. La API permite capturar datos marcados por humanos de formularios de documentos como encuestas, cuestionarios, documentos de examen de opción múltiple y otras pruebas. Con esta solución, es posible reconocer imágenes escaneadas e incluso fotos con alta precisión. El reconocimiento se basa en un marcado de plantilla que contiene un mapeo gráfico de los elementos que se reconocen a partir de las imágenes escaneadas.

## Características de la API de OMR
- Reconocimiento de imágenes y fotos escaneadas.
- Capacidad para procesar imágenes rotadas y perspectivas (vistas laterales).
- Reconocer datos de pruebas, exámenes, cuestionarios, encuestas, etc.
- Alta tasa de precisión y capacidad para exportar los resultados en formato de archivo `CSV` y` JSON`.

- [Crear plantillas OMR](https://docs.aspose.com/omr/java/create-omr-template/) del marcado de texto.

## Guardar resultados de OMR como
CSV, JSON

## leer imágenes para OMR
JPEG, PNG, GIF, TIFF, BMP

## Entornos compatibles
- ** Microsoft Windows: ** Windows Desktop & Server (x86, x64)
- ** macOS: ** Mac OS X
- ** Linux: ** Ubuntu, OpenSuse, CentOS y otros
- ** versiones Java: ** `J2SE 7.0 (1.7)`, `J2SE 8.0 (1.8)` o superior

## Empezar

Aspose.OMR Las API Java están alojadas en el [Repositorio de asposio](https://repository.aspose.com/omr/). Puede usar fácilmente Aspose.omr para la API Java directamente en sus proyectos Maven con configuraciones simples. Para las instrucciones detalladas, visite la página de documentación [Installing Aspose.OMR for Java from Maven Repository](https://docs.aspose.com/omr/java/installation/).

## Realizar operación OMR en imágenes usando Java

```java
// For complete examples and data files, please go to https://github.com/aspose-omr/Aspose.OMR-for-Java
String TemplateName = "Sheet.omr";
String[] UserImages = new String[] { "Sheet1.jpg", "Sheet2.jpg" };
String[] UserImagesNoExt = new String[] { "Sheet1", "Sheet2" };

String sourceDirectory = Utils.getSourceDirectory();
String outputDirectory = Utils.combine(Utils.getOutputDirectory(), "Result");
String templatePath = Utils.combine(Utils.getSourceDirectory(), TemplateName);

// initialize engine and get template processor providing path to the .omr file
OmrEngine engine = new OmrEngine();
TemplateProcessor templateProcessor = engine.getTemplateProcessor(templatePath);
System.out.println("Template loaded.");

// images loop
for (int i = 0; i < UserImages.length; i++) {
    // path to the image to be recognized
    String imagePath = Utils.combine(sourceDirectory, UserImages[i]);
    System.out.println("Processing image: " + imagePath);

    // recognize image and receive result
    RecognitionResult result = templateProcessor.recognizeImage(imagePath);

    // export results as csv string
    String csvResult = result.getCsv();

    String json = result.getJson();

    // save csv to the output folder
    PrintWriter wr = new PrintWriter(new FileOutputStream(Utils.combine(outputDirectory, UserImagesNoExt[i] + ".csv")), true);
    wr.println(csvResult);
}
```

[Hogar](https://www.aspose.com/) | [Página del producto](https://products.aspose.com/omr/java) | [Documentos](https://docs.aspose.com/omr/java/) | [Población](https://products.aspose.app/omr/family) | [Referencia de API](https://apireference.aspose.com/omr/java) | [Ejemplos](https://github.com/aspose-omr/Aspose.OMR-for-Java) | [Blog](https://blog.aspose.com/category/omr/) | [Búsqueda](https://search.aspose.com/) | [Soporte gratuito](https://forum.aspose.com/c/omr) | [Licencia temporal](https://purchase.aspose.com/temporary-license)
