---
title: "aspose.omr |用于数字标记提取的Java类库" 
linktitle: Aspose.OMR
description: "Java类库的光标识识别（OMR）。从数字化或扫描的图像，照片，调查，考试和问卷中识别并提取标记。" 
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
family_listing_page_title: "aspose.omr for Java" 
family_listing_page_description: "Java的Aspose.OMR是一种API，可以从OMR数字化板图像中识别光标记。它可用于识别BMP，JPG，TIF，TIFF，GIF等各种图像格式的光标记。 API允许从文档表格，调查，问卷，多项选择检查文件和其他测试中捕获人类标记的数据。" 
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

# 执行OMR的Java API
{{< repository/extract-package-explore-link imgsrc=./aspose_omr-for-java-banner.png >}}

[家](https://www.aspose.com/) | [产品页面](https://products.aspose.com/omr/java) | [文档](https://docs.aspose.com/omr/java/) | [演示](https://products.aspose.app/omr/family) | [API参考](https://apireference.aspose.com/omr/java) | [例子](https://github.com/aspose-omr/Aspose.OMR-for-Java) | [博客](https://blog.aspose.com/category/omr/) | [搜索](https://search.aspose.com/) | [免费支持](https://forum.aspose.com/c/omr) | [临时许可](https://purchase.aspose.com/temporary-license)

[Aspose.OMR for Java](https://products.aspose.com/omr/java)是一个Java类库，它提供了API，可以从OMR数字化的片段图像中识别光标记。它可用于识别BMP，JPG，TIF，TIFF，GIF等各种图像格式的光标记。 API允许从文档表格，调查，问卷，多项选择检查文件和其他测试中捕获人类标记的数据。使用此解决方案，可以以高精度识别扫描的图像甚至照片。识别基于模板标记，该模板标记包含要从扫描图像中识别的元素的图形映射。

## OMR API功能
 - 识别扫描的图像和照片。
 - 能够处理旋转和透视图（侧视图）图像的能力。
 - 识别来自测试，考试，问卷，调查等的数据。
 - 高精度率和以“ CSV”和`json'文件格式导出结果的能力。

-[创建OMR模板](https://docs.aspose.com/omr/java/create-omr-template/)来自文本标记。

## 将OMR结果保存为
CSV，JSON

## 读取OMR的图像
JPEG，PNG，GIF，TIFF，BMP

## 支持环境
 -  ** Microsoft Windows：** Windows Desktop＆Server（X86，X64）
 -  ** macOS：** Mac OS X
 -  ** Linux：** Ubuntu，Opensuse，Centos等
 -  ** java版本：**``j2se 7.0（1.7）`，`j2se 8.0（1.8）`或更高版本

## 开始

Aspose.omr Java API托管在[Aspose存储库](https://repository.aspose.com/omr/)。您可以直接在使用简单配置的Maven项目中轻松地将Aspose.omr用于Java API。有关详细说明，请访问[Installing Aspose.OMR for Java from Maven Repository](https://docs.aspose.com/omr/java/installation/)文档页面。

## 使用Java在图像上执行OMR操作

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

[家](https://www.aspose.com/) | [产品页面](https://products.aspose.com/omr/java) | [文档](https://docs.aspose.com/omr/java/) | [演示](https://products.aspose.app/omr/family) | [API参考](https://apireference.aspose.com/omr/java) | [例子](https://github.com/aspose-omr/Aspose.OMR-for-Java) | [博客](https://blog.aspose.com/category/omr/) | [搜索](https://search.aspose.com/) | [免费支持](https://forum.aspose.com/c/omr) | [临时许可](https://purchase.aspose.com/temporary-license)
