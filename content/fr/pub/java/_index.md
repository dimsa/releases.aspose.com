---
title: "Aspose.pub | Fichiers de publication électronique bibliothèque de classe Java" 
linktitle: Aspose.PUB
description: "Bibliothèque Java pour analyser, traiter et convertir les formats de documents d'éditeurs en PDF. Implémentez les fonctionnalités dans votre propre produit." 
layout: packages
type: repository
categories:
  - fundamentals
keywords:
- Aspose Total
- Aspose PUB
- Aspose Java API
- pub java library
- pub java class
- PUB
- PDF
- Microsoft Publisher
- PUB conversion
- Convert PUB
- PUB to PDF
- metadata
- Windows
- Linux
- Mac
- J2SE
- Maven
- edit metadata
- modify metadata
family_listing_page_title: "Aspose.pub pour java" 
family_listing_page_description: "La bibliothèque ASPOSE.PUB fournit une API simple et pratique qui peut charger et convertir les fichiers Pub en PDF. Il est implémenté à l'aide de Java et peut être utilisé avec n'importe quelle application basée sur Java, y compris le Web ou l'application de bureau." 
family_listing_page_iconurl: "https://www.aspose.cloud/templates/aspose/App_Themes/V3/images/pub/272x272/aspose_pub-for-java.png"
family_listing_page_selfHosted: "1"
family_listing_page_type: "1"
family_listing_page_venture: "4"
family_listing_page_package: "225"
homepage_package_type: "Maven"
homepage_package_link: "https://releases.aspose.com/java/repo/com/aspose/aspose-pub/"
weight: 02	#rem
forumLink: https://forum.aspose.com/c/pub/40
productLink: https://products.aspose.com/pub/java/
releaseNotesLink: https://docs.aspose.com/pub/java/release-notes/
dataFolder: aspose_pub
packages_refs:
- "22-8"
- "20-8"
---

# Process Fichiers Pub via Java API
{{< repository/extract-package-explore-link imgsrc=./aspose_pub-for-java-banner.png >}}

[Page de produit](https://products.aspose.com/pub/java) | [Docs](https://docs.aspose.com/pub/java/) | [Référence de l'API](https://apireference.aspose.com/pub/java) | [Exemples](https://github.com/aspose-pub/Aspose.PUB-for-Java/tree/master/Exemples) | [Blog](https://blog.aspose.com/category/pub/) | [Chercher](https://search.aspose.com/) | [Support gratuit](https://forum.aspose.com/c/pub) | [Licence temporaire](https://purchase.aspose.com/temporary-license)

[Aspose.PUB for Java](https://products.aspose.com/pub/java) est une API Java qui peut lire, manipuler et convertir les fichiers Microsoft Publisher (.Pub) en PDF. Vous pouvez utiliser l'API dans vos applications Java pour travailler avec des fichiers .pub sans vous soucier du format Filie sous-jacent. L'API peut être utilisée dans Java Desktop ainsi que dans les applications Web à l'aide de JSP. L'API est légère, facile à utiliser et simplifie votre application avec des lignes de code simples dans votre application.

## Pub Java API Fonctions
- Lisez les fichiers Microsoft Publisher (Pub) pour la conversion au format PDF.
- Travailler avec les métadonnées des fichiers de pub.

## lire les fichiers pub
** Microsoft Publisher: ** Pub

## Save Pub comme
** Disposition fixe: ** PDF

## Environnements pris en charge
- ** Microsoft Windows: ** Windows Desktop & Server (x86, x64)
- ** macOS: ** mac os x
- ** Linux: ** Ubuntu, Centos et autres
- ** Versions Java: ** `J2SE 8.0 (1.8)` ou au-dessus

## Commencer

Les API Java ASPOSE.PUB sont hébergées au [Référentiel](https://repository.aspose.com/pub/). Vous pouvez facilement utiliser Aspose.pub pour l'API Java directement dans vos projets Maven avec des configurations simples. Pour les instructions détaillées, veuillez visiter la page de documentation [Installing Aspose.PUB for Java from Référentiel](https://docs.aspose.com/pub/java/installation/).

## Modifier les métadonnées des fichiers Microsoft Publisher à l'aide de Java

```java
// For complete examples and data files, please go to https://github.com/aspose-pub/Aspose.PUB-for-Java
IPubParser parser = PubFactory.createParser(fileName);
Document document = parser.parse();

document.getDocumentSummaryInfo().setCategory("category");
document.getDocumentSummaryInfo().setCompany("company");
document.getDocumentSummaryInfo().setLanguage("language");

document.getSummaryInfo().setComments("comments");
document.getSummaryInfo().setKeywords("keywords");
document.getSummaryInfo().setLastAuthor("last author");
document.getSummaryInfo().setTitle("title");
document.getSummaryInfo().setSubject("subject");
```

[Page de produit](https://products.aspose.com/pub/java) | [Docs](https://docs.aspose.com/pub/java/) | [Référence de l'API](https://apireference.aspose.com/pub/java) | [Exemples](https://github.com/aspose-pub/Aspose.PUB-for-Java/tree/master/Exemples) | [Blog](https://blog.aspose.com/category/pub/) | [Chercher](https://search.aspose.com/) | [Support gratuit](https://forum.aspose.com/c/pub) | [Licence temporaire](https://purchase.aspose.com/temporary-license)
