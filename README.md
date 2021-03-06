# iOS Hacking Resources

## Basics

Official references:

* [ARM64 instruction set reference](https://www.element14.com/community/servlet/JiveServlet/previewBody/41836-102-1-229511/ARM.Reference_Manual.pdf) (short)
* [ARMv8 Architecture Reference Manual](https://static.docs.arm.com/ddi0487/b/DDI0487B_a_armv8_arm.pdf) (long)

My own doing:

* [arm64 assembly crash course](https://github.com/Siguza/ios-resources/blob/master/bits/arm64.md)
<!-- TODO: something about memory regions and access permissions -->
<!-- TODO: something about C++ vtables -->
<!-- TODO: something about symbol stubs -->

## Internals

**Mach-O**

* [Jonathan Levin - DYLD DetaYLeD](http://www.newosxbook.com/articles/DYLD.html) <!-- Aug 2013 -->
* [Jonathan Levin - Code Signing](http://www.newosxbook.com/articles/CodeSigning.pdf) <!-- April 2015 -->

**Sandbox**

* Jonathan Levin - The Apple Sandbox ([Video](https://youtu.be/mG715HcDgO8) and [Slides](http://newosxbook.com/files/HITSB.pdf)) <!-- Sep 2016 -->

**IPC**

* Apple - Mach ([Overview](https://developer.apple.com/library/content/documentation/Darwin/Conceptual/KernelProgramming/Mach/Mach.html) and API documentation (inside the [XNU source](https://opensource.apple.com/tarballs/xnu/) in `osfmk/man/index.html`))
* [nemo - Mach and MIG](https://www.exploit-db.com/papers/13176/) (examples are outdated and for PPC/Intel, but descriptions are still accurate) <!-- 2006 -->
* Ian Beer - Apple IPC ([Video](https://vimeo.com/127859750) and [Slides](https://thecyberwire.com/events/docs/IanBeer_JSS_Slides.pdf)) <!-- May 2015 -->

**Kernel**

* Apple - [Kernel Programming Guide](https://developer.apple.com/library/content/documentation/Darwin/Conceptual/KernelProgramming)
* Apple - [IOKit Fundamentals](https://developer.apple.com/library/content/documentation/DeviceDrivers/Conceptual/IOKitFundamentals)
* Apple - [About the Virtual Memory System](https://developer.apple.com/library/content/documentation/Performance/Conceptual/ManagingMemory/Articles/AboutMemory.html)
* qwertyoruiopz - Attacking XNU (Part [One](http://blog.qwertyoruiop.com/?p=38) and [Two](http://blog.qwertyoruiop.com/?p=48)) <!-- July 2015 -->
* [Stefan Esser - Kernel Heap](http://gsec.hitb.org/materials/sg2016/D2%20-%20Stefan%20Esser%20-%20iOS%2010%20Kernel%20Heap%20Revisited.pdf) (I hope I don't get sued) <!-- Aug 2016 -->

**KPP**

* [xerub - Tick Tock](https://xerub.github.io/ios/kpp/2017/04/13/tick-tock.html)

**Hardware**

* Ramtin Amin - [Lightning Connector](http://ramtin-amin.fr/#tristar)
* Ramtin Amin - [NVMe NAND Storage](http://ramtin-amin.fr/#nvmepcie)
* Ramtin Amin - [iPhone PCIe (dumping the 6s BootROM)](http://ramtin-amin.fr/#nvmedma)

## Write-Ups

* [geohot - evasi0n7](http://geohot.com/e7writeup.html)
* Jonathan Levin - TaiG 8.0 - 8.1.2 (Part [One](http://www.newosxbook.com/articles/TaiG.html) and [Two](http://www.newosxbook.com/articles/TaiG2.html))
* Jonathan Levin - TaiG 8.1.3 - 8.4 (Part [One](http://www.newosxbook.com/articles/28DaysLater.html) and [Two](http://www.newosxbook.com/articles/HIDeAndSeek.html))
* [Jonathan Levin - Who needs task_for_pid anyway?](http://newosxbook.com/articles/PST2.html)
* [qwertyoruiopz - About the “tpwn” Local Privilege Escalation](http://blog.qwertyoruiop.com/?p=69)
* [Ian Beer - task_t considered harmful](https://googleprojectzero.blogspot.ch/2016/10/taskt-considered-harmful.html)
* [jndok - Exploiting Pegasus on OS X](https://jndok.github.io/2016/10/04/pegasus-writeup/)
* [Siguza - Exploiting Pegasus on iOS](https://siguza.github.io/cl0ver/)
* [Ian Beer - mach_portal](https://bugs.chromium.org/p/project-zero/issues/detail?id=965#c2)
* [Ian Beer - Exception-oriented exploitation on iOS](https://googleprojectzero.blogspot.ch/2017/04/exception-oriented-exploitation-on-ios.html)
* [Jonathan Levin - Phœnix](http://newosxbook.com/files/PhJB.pdf)
* Gal Beniamini - Over The Air (Parts [One](https://googleprojectzero.blogspot.ch/2017/09/over-air-vol-2-pt-1-exploiting-wi-fi.html), [Two](https://googleprojectzero.blogspot.ch/2017/10/over-air-vol-2-pt-2-exploiting-wi-fi.html) and [Three](https://googleprojectzero.blogspot.ch/2017/10/over-air-vol-2-pt-3-exploiting-wi-fi.html))

## Other Lists

* qwertyoruiopz - iOS Reverse Engineering ([Wiki](https://github.com/kpwn/iOSRE/tree/master/wiki) and [Papers](https://github.com/kpwn/iOSRE/blob/master/resources/papers/PAPERS.md))
* [Ian Beer - All the bugs he has killed](https://bugs.chromium.org/p/project-zero/issues/list?can=1&q=owner:ianbeer&sort=-id)
