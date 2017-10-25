---
author: stevewhims
Description: This section shows you how to author, package, and consume your app's string, image, and file resources.
title: App resources and the Resource Management System
label: Intro
template: detail.hbs
ms.author: stwhi
ms.date: 10/20/2017
ms.topic: article
ms.prod: windows
ms.technology: uwp
keywords: windows 10, uwp, resource, image, asset, MRT, qualifier
---

# App resources and the Resource Management System
<link rel="stylesheet" href="https://az835927.vo.msecnd.net/sites/uwp/Resources/css/custom.css">

This section shows you how to author, package, and consume your app's string, image, and file resources. For example, you might package a file along with your casual game containing a definition of the game's levels, and load the file at run-time. We also show you how maintaining your resources independently of the app's logic makes it easy to localize and customize your app for different locales, device displays, accessibility settings, and other user and machine contexts. Resources such as strings and images typically need to exist in multiple language, scale, and contrast variants. For resources such as that, you have the support of the [Resource Management System](resource-management-system.md).

| Article | Description |
|---------|-------------|
| [Resource Management System](resource-management-system.md) | At build time, the Resource Management System creates an index of all the different variants of the resources that are packaged up with your app. At run-time, the system detects the user and machine settings that are in effect and loads the resources that are the best match for those settings. |
| [How the Resource Management System matches and chooses resources](how-rms-matches-and-chooses-resources.md) | When a resource is requested, there may be several candidates that match the current resource context to some degree. The Resource Management System will analyze all of the candidates and determine the best candidate to return. This topic describes that process in detail and gives examples. |
| [Tailor your resources for language, scale, high contrast, and other qualifiers](tailor-resources-lang-scale-contrast.md) | This topic explains the general concept of resource qualifiers, how to use them, and the purpose of each of the qualifier names. |
| [Localize strings in your UI and app package manifest](localize-strings-ui-manifest.md) | If you want your app to support different display languages, and you have string literals in your code or XAML markup or app package manifest, then move those strings into a Resources File (.resw). You can then make a translated copy of that Resources File for each language that your app supports. |
| [Load images and assets tailored for scale, theme, high contrast, and others](images-tailored-for-scale-theme-contrast.md) | Your app can load image resource files containing images tailored for display scale factor, theme, high contrast, and other runtime contexts. |
| [Tile and toast notification support for language, scale, and high contrast](tile-toast-language-scale-contrast.md) | Your tiles and toasts can load strings and images tailored for display language, display scale factor, high contrast, and other runtime contexts. |
| [URI schemes](uri-schemes.md) | There are several URI (Uniform Resource Identifier) schemes that you can use to refer to files that come from your app's package, your app's data folders, or the cloud. You can also use a URI scheme to refer to strings loaded from your app's Resources Files (.resw). |
| [Compile resources manually with MakePri.exe](compile-resources-manually-with-makepri.md) | MakePri.exe is a command line tool that you can use to create and dump PRI files. It is integrated as part of MSBuild within Microsoft Visual Studio, but it could be useful to you for creating packages manually or with a custom build system. |
| [MakePri.exe command-line options](makepri-exe-command-options.md) | MakePri.exe has the set of commands `createconfig`, `dump`, `new`, `resourcepack`, and `versioned`. This topic details the command-line options for their use. |
| [MakePri.exe configuration file](makepri-exe-configuration.md) | This topic describes the schema of the MakePri.exe XML configuration file. |
| [MakePri.exe format-specific indexers](makepri-exe-format-specific-indexers.md) | This topic describes the format-specific indexers used by the MakePri.exe tool to generate its index of resources. |
| [Use the Windows 10 Resource Management System in a legacy app or game](using-mrt-for-converted-desktop-apps-and-games.md) | By packaging your .NET or Win32 app or game as an AppX package, you can leverage the Resource Management System to load app resources tailored to the run-time context. This in-depth topic describes the techniques. |

Also see the documentation originally created for Windows 8.x, which still applies to Universal Windows Platform (UWP) apps and Windows 10.

-   [App resources and localization](https://msdn.microsoft.com/library/windows/apps/xaml/hh710212.aspx)