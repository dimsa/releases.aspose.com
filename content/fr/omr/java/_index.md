---
title: "Aspose.omr | Bibliothèque de classe Java pour l'extraction des marques numériques" 
linktitle: Aspose.OMR
description: "Bibliothèque de classe Java pour la reconnaissance des marques optiques (OMR). Reconnaître et extraire les marques des images numérisées ou numérisées, des photos, des enquêtes, des examens et des questionnaires." 
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
family_listing_page_title: "Aspose.omr pour java" 
family_listing_page_description: "Aspose.omr pour Java est une API pour reconnaître les marques optiques des images de feuille numérisées OMR. Il peut être utilisé pour reconnaître les marques optiques dans une variété de formats d'image comme BMP, JPG, TIF, TIFF, GIF. L'API permet de capturer des données marquées par l'homme à partir de formulaires de documents tels que des enquêtes, des questionnaires, des documents d'examen à choix multiples et d'autres tests." 
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

# API Java pour effectuer OMR
{{< repository/extract-package-explore-link imgsrc=./aspose_omr-for-java-banner.png >}}

[Maison](https://www.aspose.com/) | [Page de produit](https://products.aspose.com/omr/java) | [Docs](https://docs.aspose.com/omr/java/) | [Démos](https://products.aspose.app/omr/family) | [Référence de l'API](https://apireference.aspose.com/omr/java) | [Exemples](https://github.com/aspose-omr/Aspose.OMR-for-Java) | [Blog](https://blog.aspose.com/category/omr/) | [Chercher](https://search.aspose.com/) | [Support gratuit](https://forum.aspose.com/c/omr) | [Licence temporaire](https://purchase.aspose.com/temporary-license)

[Aspose.OMR for Java](https://products.aspose.com/omr/java) est une bibliothèque de classe Java qui fournit une API pour reconnaître les marques optiques des images de feuille numérisées OMR. Il peut être utilisé pour reconnaître les marques optiques dans une variété de formats d'image comme BMP, JPG, TIF, TIFF, GIF. L'API permet de capturer des données marquées par l'homme à partir de formulaires de documents tels que des enquêtes, des questionnaires, des documents d'examen à choix multiples et d'autres tests. Avec cette solution, il est possible de reconnaître les images numérisées et même les photos avec une grande précision. La reconnaissance est basée sur un balisage de modèle qui contient une cartographie graphique des éléments à reconnaître à partir des images numérisées.

## fonctionnalités de l'API OMR
- Reconnaissance des images et des photos numérisées.
- Capacité à traiter les images tournées et en perspective (vue latérale).
- Reconnaître les données des tests, des examens, des questionnaires, des enquêtes, etc.
- Taux de précision élevée et capacité à exporter les résultats au format de fichier `CSV` et` JSON`.

- [Créer des modèles OMR](https://docs.aspose.com/omr/java/create-omr-template/) à partir du balisage du texte.

## Enregistrer les résultats OMR comme
CSV, JSON

## lire des images pour OMR
JPEG, PNG, GIF, TIFF, BMP

## Environnements pris en charge
- ** Microsoft Windows: ** Windows Desktop & Server (x86, x64)
- ** macOS: ** mac os x
- ** Linux: ** Ubuntu, OpenSuse, Centos et autres
- ** Versions Java: ** `J2SE 7.0 (1.7)`, `J2SE 8.0 (1.8) ou supérieur

## Commencer

Les API Java Aspose.omr sont hébergées au [Référentiel](https://repository.aspose.com/omr/). Vous pouvez facilement utiliser Aspose.omr pour l'API Java directement dans vos projets Maven avec des configurations simples. Pour les instructions détaillées, veuillez visiter la page de documentation [Installing Aspose.OMR for Java from Maven Repository](https://docs.aspose.com/omr/java/installation/).

## Effectuez l'opération OMR sur les images en utilisant Java

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

[Maison](https://www.aspose.com/) | [Page de produit](https://products.aspose.com/omr/java) | [Docs](https://docs.aspose.com/omr/java/) | [Démos](https://products.aspose.app/omr/family) | [Référence de l'API](https://apireference.aspose.com/omr/java) | [Exemples](https://github.com/aspose-omr/Aspose.OMR-for-Java) | [Blog](https://blog.aspose.com/category/omr/) | [Chercher](https://search.aspose.com/) | [Support gratuit](https://forum.aspose.com/c/omr) | [Licence temporaire](https://purchase.aspose.com/temporary-license)
