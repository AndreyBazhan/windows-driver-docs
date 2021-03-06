---
title: General Design and Implementation Strategies
description: General Design and Implementation Strategies
ms.assetid: c631062c-87ec-4bad-9de2-1844d0c81661
keywords:
- display driver model WDK Windows 2000 , strategies
- Windows 2000 display driver model WDK , strategies
- video miniport drivers WDK Windows 2000 , strategies
- display drivers WDK Windows 2000 , strategies
ms.author: windowsdriverdev
ms.date: 04/20/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# General Design and Implementation Strategies


## <span id="ddk_general_design_and_implementation_strategies_gg"></span><span id="DDK_GENERAL_DESIGN_AND_IMPLEMENTATION_STRATEGIES_GG"></span>


To design an effective Windows 2000 and later display driver and video miniport driver, consider the following strategies:

-   Modify an existing Windows Driver Kit (WDK) sample driver that was designed for a similar type of graphics adapter to reduce driver design time.

-   Use C to write as much of the driver as possible to maximize portability, using assembly language only when necessary for time-critical operations that are not well supported by the hardware. Although coding in assembly increases the potential for optimization, time and portability issues outweigh its benefits.

-   Use video miniport drivers for operations that manage resources, perform physical device memory mapping, ensure that register outputs occur in close proximity, or respond to interrupts. Miniport drivers are predominately used for handling variations within a hardware family and for minimizing display driver hardware-type dependencies.

For additional information of interest to display driver writers, see [Graphics DDI Functions for Display Drivers](graphics-ddi-functions-for-display-drivers.md). This topic and the subtopics following it discuss the graphics DDI functions that are required, conditionally required, and optional for a display driver. [Video Miniport Drivers in the Windows 2000 Display Driver Model](video-miniport-drivers-in-the-windows-2000-display-driver-model.md) and its subtopics contain similar information aimed at video miniport driver writers.

You should also consider the following facts:

-   The display driver and video miniport driver operate in the same privileged kernel-mode address space as the rest of the NT executive. A fault in either driver will cause the rest of the system to fault.

-   Display drivers and video miniport drivers can be preempted at any time.

-   The code and data sections of a display driver are both entirely pageable.

-   Exported functions must execute the standard NT-based operating system *prolog* on entry and the *epilog* on exit. For more information, see the Microsoft Windows SDK documentation.

For information that is specific to display drivers, see [Graphics DDI Functions for Display Drivers](graphics-ddi-functions-for-display-drivers.md). That section contains information about required, conditionally required, and optionally required graphics DDI functions.

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20General%20Design%20and%20Implementation%20Strategies%20%20RELEASE:%20%282/10/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




