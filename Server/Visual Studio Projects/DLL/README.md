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

8. Now we should specify that this project will be compiled to x86, not x86-64 as may be the default
   1. Click on *Properties* in the Solution Explorer, or in the *Project* dropdown as shown previously

        <img src="Images/I10.png">

   2. Select *Platform* and *Win32*

        <img src="Images/I11.png">

9. Now we can configure the *Linker*
   1.  Open the Linker *All Options* table as shown below

        <img src="Images/I12.png">

   2. Set the preferred base address

        <img src="Images/I13.png">

   3. Disable DEP

        <img src="Images/I14.png">

   4. Set Incremental Linking to NO - It does not appear we did this with the GCC version

        <img src="Images/I15.png">

   5. Set SAFE-SEH to No

        <img src="Images/I16.png">

## Refs

https://learn.microsoft.com/en-us/cpp/build/creating-precompiled-header-files?view=msvc-170

https://learn.microsoft.com/en-us/cpp/assembler/inline/inline-assembler?view=msvc-170

https://edgesupport.diasemi.com/hc/en-us/articles/205663464-How-to-set-up-your-Visual-Studio-project-to-build-for-x86-Hardware-platform-KB1025#:~:text=Click%20BUILD%20%3E%20CONFIGURATION%20MANAGER%20select%20the%20platform,create%20x86%20as%20a%20platform%20option%20to%20choose.