## Week 5 Write-Up
Week four focused on content provided by Aditya Kapoor, a research architect at McAfee Labs. The lecture this week provided a brief overview of Windows operating system internals and the development as well as implementation of rootkits. Content for week 5 introduced how the Windows kernel and user ineract, kernel memory, Windows threads, Windows processes, and Rootkit styles plus various techniques utilized. 

### Kernel v. User
One of the first concepts discussed was the interaction between the operating system kernel and the end user. At the top layer is of the interaction is applications which are compiled to executables or dll's that interact with the Windows operating system API which will then interact with either user-mode drivers or the operating system kernel iteself. knowing this top level is very important as it shows the interaction to utilized the systems kernel for system calls which if accessed from outside can lead to detrimental security issues. Furthermore after receiving the API information or exported driver information (from user-mode) the kernel will then interact with the abstract hardware layer which will use the kernel's information to utilize subroutines built for specific hardware so that when interacting directly with the hardware the hardware itself can perform the necessary computation or system routine designated by the user or application that came in contact through the Windows API or exported drivers. Below is a diagram of the interaction between users/applications and an operating system's kernel.

<img src="KernelvUser.png" alt="" class="inline"/>





