---
title: SDKBrowser Demo App
page_title: Telerik .NET MAUI Examples
description: "Learn how to download and install the SDKBrowser Demo App and check out the Telerik UI for .NET MAUI controls library."
slug: sdkbrowser-app
tags: .net maui, ui for .net maui, .net maui controls
previous_url: /demos-and-sample-apps/maui-demo-app
position: 2
---

# SDKBrowser Demo Application

**Telerik UI for .NET MAUI SDKBrowser** is a set of examples that explain how to use the features of a control. The SDKBrowser shows the components in their pure form without adding extra styling and polishing. It's the go-to source for "how do I use X in Y control". Most of the code snippets available in the documentation are directly generated from the examples in the SDKBrowser (you can see special comments in the code for this).

![Telerik UI for .NET MAUI SDKBrowserMaui App](../images/demo-maui.gif)

You can access the SDKBrowser application in the following ways:

* If you have already installed Telerik UI for .NET MAUI, navigate to the **/[installation-path]/Telerik UI for .NET MAUI [version]/Examples/Sdk** folder and open the `SdkBrowserMaui.sln` file;
* You can explore the code directly in the [.NET MAUI Samples repository on GitHub](https://github.com/telerik/maui-samples/tree/main/Samples);

## Run SDKBrowser on Windows

1. Inside the command prompt, run the `maui-check` command, which is required for using Telerik UI for .NET MAUI controls, and for building and running `SDKBrowserMaui.sln`.

1. Run the `Telerik_UI_for_Maui_[version]_Preview.msi` file and follow the instructions. The file automatically installs Telerik UI for .NET MAUI on your PC.

    On a 32-bit machine, the wizard will suggest to install the UI for .NET MAUI controls in `C:\Program Files\Progress\`. On a 64-bit machine, the wizard will suggest to install the UI for .NET MAUI controls in `C:\Program Files (x86)\Progress\`.

1. The **SDKBrowser** folder is located inside the installation folder and you can now use the following subdirectories:

    * **Binaries**&mdash;Contains the needed dlls for Android, iOS, and WinUI.
    * **Examples**&mdash;Contains all examples available (`Sdk app` and `CryptoTracker app`) with the Telerik UI for .NET MAUI controls.
    * **LicenseAgreements**&mdash;Provides the product End-User License Agreement (EULA).
    * **Packages**&mdash;Contains the `Telerik_UI_for_Maui_[version]_Preview.nupkg` file.

    ![Telerik UI for .NET MAUI Installation Folder](../images/telerik-ui-for-maui-installation-folder.png)

1. `SDKBrowserMaui.sln` on Windows with Visual Studio.

    4.1 Open the SDKBrowser folder in Visual Studio 2022 Preview.

   ![Telerik UI Maui SDKBrowser Maui App VS Code](../images/sdkmaui-structure.png)

    4.2 Wait for the project to restore.

    4.3 Select the target framework of the project.

   ![Telerik UI SDKBrowser Maui App](../images/maui-win-ui-project-structure.png)

    4.4 Select the emulator or device on which you want to run the application.

1. Run On Windows: 

	5.1 Install the [Single-Project MSIX Packaging Tool for VS 2022 Preview](https://marketplace.visualstudio.com/items?itemName=ProjectReunion.MicrosoftSingleProjectMSIXPackagingToolsDev17) to build and run the application.

   ![Telerik UI SDKBrowser Maui App](../images/maui-win-ui-project-structure.png)
   
    5.2 The SdkBrowserMaui on Windows:
 
    ![Telerik UI for .NET MAUI SDKBrowser Maui Application](../images/demo-winui.png)
	
1. SdkBrowserMaui On Android: 

![Telerik UI for .NET MAUI SDKBrowser Maui Application](../images/demo.png)
	
## Install and Run SDKBrowser on macOS

>important Review the [macOS Install .NET MAUI GitHub Wiki page](https://github.com/dotnet/maui/wiki/macOS-Install) for more information how to get started on macOS. 

1. Inside the terminal, run the `maui-check` command, which is required for using Telerik UI for .NET MAUI controls, and for building and running `SDKBrowserMaui.sln`.

1. Run the `Telerik_UI_for_Maui_[version]_Preview.pkg` file, which automatically installs Telerik UI for .NET MAUI on your Mac.

1. The **SDKBrowserMaui** folder is located inside the installation folder and you can now use the following subdirectories:

    * **Binaries**&mdash;Contains the needed dlls for Android, iOS, and WinUI.
    * **Examples**&mdash;Contains all examples available (**Sdk app** and **CryptoTracker app**) with the Telerik UI for .NET MAUI controls.
    * **LicenseAgreements**&mdash;Provides the product End-User Licensce Agreement (EULA).
    * **Packages**&mdash;Contains the `Telerik_UI_for_Maui_[version]_Preview.nupkg` file.

    ![Telerik UI for .NET MAUI Installation Folder](../images/installation-macos.png)

1. Open Terminal inside the Sdk app folder.

1. Run on macOS using the following command:

 `dotnet build -t:Run -f net6.0-maccatalyst`
 
	* SDKBrowserMaui application on MacOS.
	
	![Telerik UI for .NET MAUI SDKBrowser Maui Application](../images/demo-macos.png)
	
1. Run on iOS using the following command: Append the value to the parameter `-p:_DeviceName=:v2:uuid=:`

 `dotnet build -t:Run -f net6.0-ios -p:_DeviceName=:v2:udid=02C556DA-64B8-440B-8F06-F8C56BB7CC22`
 
 where the `-p:_DeviceName=:v2:uuid==02C556DA-64B8-440B-8F06-F8C56BB7CC22` is the desired device id.

	* SDKBrowserMaui application on iOS.

   ![Telerik UI for .NET MAUI SDKBrowser Maui Application](../images/demo-iphone.png)  