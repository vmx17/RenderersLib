# RenderersLib - A Sample Project of XAML control as Windows Runtime Component and its Projection to NuGet package, then consume it in C# desktop application.
last update: 9/11/2022

The title is too long.
## What it is
 A sample of XAML control library in C++/WinRT and Projection project to NuGet Package. It will be comsumed in C# using Windows App SDK.

 So the app will be C# based WinUI3 Desktop application using XAML Windows Runtime Component written in C++/WinRT (but still I don't know it is possible).
 
 Currently building WRC stops in compile error. This repository was made to ask Microsoft Q&A but welcome opinions from everyone.
 
## the first priority Error
 does not match build architecture on Prorection project.

## How to reproduce the current error
 1. Open solution file "_RenderersLib.sln_" in VisualStudio 2022.
 2. Restore NuGet packages.
 3. Build Solution.

## update
 - _Error	C2039	'BoxRenderer': is not a member of 'winrt::Renderers::implementation'_.
		-> fixed: move `#include "BoxRenderer.h"` from "BoxRenderer.cpp" to "pch.h".
		
## Reference
- [**XAML custom (templated) controls with C++/WinRT**](https://docs.microsoft.com/en-us/windows/uwp/cpp-and-winrt-apis/xaml-cust-ctrl)
- [**Build XAML controls with C++/WinRT**](https://docs.microsoft.com/en-us/windows/apps/winui/winui3/xaml-templated-controls-cppwinrt-winui-3)
- [**Generate a C# projection from a C++/WinRT component, distribute as a NuGet for .NET apps**](https://docs.microsoft.com/en-us/windows/apps/develop/platform/csharp-winrt/net-projection-from-cppwinrt-component). 

## Others
- These codes were made of Internet public resources (and Microsoft property, of course). So I don't insist license or else.
- English is not my domestic language. So fix rough sentences (_gently_, please).