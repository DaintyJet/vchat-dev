# 



1. Download Visual Studio
2. Open Visual Studio 
3. Click Create a new Project

    <img src="Images/I3.png">

4. Select Dynamic-Link Library (DLL)

    <img src="Images/I4.png">

5. Select a location to store the project

    <img src="Images/I5.png">

6. There may be a few pre-generated files as shown below, you can remove the `dllmain.cpp`, `pch.cpp`. and `pch.h`

    <img src="Images/I6.png">

7. We can disable the use of precompiled headers in the following manner
   1. Open the Project Properties window: Project -> Properties

        <img src="Images/I7.png">

   2. Navigate to the Precompiled Headers options: C/C++ -> Precompiled Headers 

        <img src="Images/I8.png">

   3. Select "Not Using Precompiled Headers

        <img src="Images/I9.png">



## Refs

https://learn.microsoft.com/en-us/cpp/build/creating-precompiled-header-files?view=msvc-170

https://learn.microsoft.com/en-us/cpp/assembler/inline/inline-assembler?view=msvc-170

https://edgesupport.diasemi.com/hc/en-us/articles/205663464-How-to-set-up-your-Visual-Studio-project-to-build-for-x86-Hardware-platform-KB1025#:~:text=Click%20BUILD%20%3E%20CONFIGURATION%20MANAGER%20select%20the%20platform,create%20x86%20as%20a%20platform%20option%20to%20choose.