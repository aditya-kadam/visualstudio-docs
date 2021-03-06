---
title: "Creating Site Definitions for SharePoint | Microsoft Docs"
ms.custom: ""
ms.date: "02/02/2017"
ms.technology: 
  - "office-development"
ms.topic: "conceptual"
dev_langs: 
  - "VB"
  - "CSharp"
  - "VB"
  - "CSharp"
helpviewer_keywords: 
  - "SharePoint development in Visual Studio, site definitions"
  - "site definitions [SharePoint development in Visual Studio]"
author: TerryGLee
ms.author: tglee
manager: douge
ms.workload: 
  - "office"
---
# Creating Site Definitions for SharePoint
  The SharePoint Site Definition project in [!INCLUDE[vsprvs](../sharepoint/includes/vsprvs-md.md)] lets you create a *site definition*, which serves as a foundation for a new SharePoint site. These definitions not only determine the appearance and behavior of the SharePoint site, but also its default content and functionality. In the definition you can put preconfigured lists, content types, event receivers, images, and other items. SharePoint includes some site definitions such as BLOG, for example. When you create a site based on the BLOG site definition, the site contains the lists, Web parts, and other items that a blogging site requires.  
  
 For more information about site definitions, see [Site Templates and Definitions](http://go.microsoft.com/fwlink/?LinkId=179134).  
  
## Site Definition Projects  
 Site definition projects in [!INCLUDE[vsprvs](../sharepoint/includes/vsprvs-md.md)] provide only the basic files that a SharePoint site needs; they do not provide any default functionality. You must add files and content to provide the functionality that you want. You can build the site manually, by creating and adding the files that you need.  
  
## Feature Stapling  
 One benefit of creating site definitions in [!INCLUDE[vsprvs](../sharepoint/includes/vsprvs-md.md)] is that they automatically use *Feature Stapling*. Feature Stapling attaches a feature to a site definition instead of embedding its functionality in the site definition itself. Doing this lets you add the feature to any site created by using the site definition without modifying the original site definition. For more information, see [Feature Stapling](http://go.microsoft.com/fwlink/?LinkID=119283).  
  
## Site Definition Project Components  
 When you create a site definition solution, the following default files are added to its **SiteDefinition** node.  
  
|File Name|Description|  
|---------------|-----------------|  
|default.aspx|The default ASPX home page for the new SharePoint site.|  
|onet.xml|Specifies the configuration of the new site, the components of the site definition template, and default behavior. These settings can include attributes such as the content types that are enabled, the default list views, document template files, and Web parts included with the site. By default, the `Modules` section lists the files to be added to the SharePoint site and how they are configured.|  
|webtemp_*SiteDefinitionName*.xml|Specifies the site definition configurations that appears in the **Template Selection** section of the **New SharePoint Site** page.|  
  
 By default, all site definitions are stored in the *drive:*\Program Files\Common Files\Microsoft Shared\Web Server Extensions\14\TEMPLATE\SiteTemplates folder. Each site definition has its own subfolder.  
  
## Related Topics  
  
|Title|Description|  
|-----------|-----------------|  
|[Walkthrough: Create a Basic Site Definition Project](../sharepoint/walkthrough-create-a-basic-site-definition-project.md)|Leads you step-by-step through the creation of a basic site definition project in [!INCLUDE[vsprvs](../sharepoint/includes/vsprvs-md.md)].|  
|[How to: Create a Custom Site Definition and Configuration](http://go.microsoft.com/fwlink/?LinkId=183309)|Describes how to create a custom site definition in SharePoint by copying an existing site definition and then modifying the copy.|  
|[WebTemp.xml](http://go.microsoft.com/fwlink/?LinkId=183310)|Describes the original file that specifies the site definitions available in the **Template Selection** section of the **New SharePoint Site** page.|  
|[Localizing SharePoint Solutions](../sharepoint/localizing-sharepoint-solutions.md)|Describes how to prepare your SharePoint solutions for global use.|  
|[Creating Web Parts for SharePoint](../sharepoint/creating-web-parts-for-sharepoint.md)|Describes how you can create parts of a SharePoint page that users can modify.|  
|[Creating Reusable Controls for Web Parts or Application Pages](../sharepoint/creating-reusable-controls-for-web-parts-or-application-pages.md)|Describes how you can create reusable controls that run in application pages and Web Parts.|  
|[Visual Web Developer](http://go.microsoft.com/fwlink/?LinkId=178725)|Describes how to use the designer that appears when you open a Web page in your project.|  
|[ASP.NET Web Pages Overview](http://go.microsoft.com/fwlink/?LinkId=178726)|Provides general information about the structure of [!INCLUDE[vstecasp](../sharepoint/includes/vstecasp-md.md)] Web pages, how pages are processed by [!INCLUDE[vstecasp](../sharepoint/includes/vstecasp-md.md)], and how [!INCLUDE[vstecasp](../sharepoint/includes/vstecasp-md.md)] pages display markup that complies with XHTML standards.|  
|[ASP.NET Web Page Syntax](http://go.microsoft.com/fwlink/?LinkId=178727)|Describes the markup elements that make up an ASP.NET page.|  
|[Programming ASP.NET Web Pages](http://go.microsoft.com/fwlink/?LinkId=178728)|Provides information about how to create event handlers in [!INCLUDE[vstecasp](../sharepoint/includes/vstecasp-md.md)] pages and how to work with client script.|  
|[Programming in Windows SharePoint Services](http://go.microsoft.com/fwlink/?LinkId=178729)|Describes how to use the managed object model that is provided in [!INCLUDE[sharepointShort](../sharepoint/includes/sharepointshort-md.md)].|  
  
## See Also  
 [Developing SharePoint Solutions](../sharepoint/developing-sharepoint-solutions.md)  
  
  