# Everyone should study Operating Systems
This February I took the plunge and decided to complete my Operating Systems class I signed up for last year. I’m currently in the last few weeks of the class and I'd like to share my 2 cents.


So here’s the deal, **I think you should study Operating Systems**. But Why? You may ask.


### Here’s Why


Wait! Before I explain **Why**, I need to explain **What**.

&nbsp;

## So What is an Operating System, anyway?

An Operating System is just another computer program! (If a large, complex, mature and mission critical one.) There! I said it.

More specifically, it’s a computer program that
-   multiplexes hardware resources and
-   implements useful abstractions.


**Wait, What?**


**Multiplexing** allows multiple people or programs to use the same set of hardware resources—​processors, memory, disks, network connection—​safely and efficiently.


**Abstractions:** processes, threads, address spaces, files, and sockets—​simplify the usage of hardware resources by organizing information or implementing new capabilities.

&nbsp;

### Let's get a little deeper into abstractions.
Abstractions simplify application design by:
-   hiding undesirable properties,
-   adding new capabilities, and
-   organizing information.


Abstractions provide an **interface** (An interface describes what an computer program does, and how it interacts with the rest of the world.) to application programmers that separates **policy**—what the interface commits to accomplishing—​from **mechanism**—how the interface is implemented.


I think an example would make things a little more clear. So let's take an example

### File
We all know what a File is, right?


I bet you're thinking, "What do you mean File? A File is a File!". We don't really think about Files anymore, do we?

Everything in a computer is File (I mean literally). From network sockets to your images, everything! Let's just say it's like an container where bunch of data goes.


Ok. So applying our abstractions definition,

**What undesirable properties do File Systems hide?**

-   Disks are just large arrays of non-volatile memory
    >   Disks have no concept of a file or file systems. They don't understand file names. Only thing they understand (over simplified) is to store/retrieve a bunch of data from a given location.
-   Disks are slow!
    >   Yep. In-fact they are one of biggest bottlenecks (And yes, your latest ssd with blazing fast speeds is still a huge bottleneck for a cpu) of a modern day computer (also Internet in some places). But, we don't care about that, right? We just want the file to be open as soon we click on it.
-   Chunks of storage are actually distributed all over the disk.
    >   When you open any file (no matter it's size), you can see it in it's entirety. But underneath the hood, they are actually spread out all over the disk.
-   Disk storage may fail!
    >   I know, It's the harsh truth. Your disk storage may fail. Disk drives have mechanical parts that can brake. The sectors in the plater of disk drive may die. And Yes your ssd can fail too. So, File Systems have features built into them that are designed to make Disk more Robust.

&nbsp;

**What new Capabilities do Files add?**

-   Growth and shrinking.
    >   We can easly grow or shrink a file. Imagine your reaction when you try to edit a file and your computer says you can't edit anymore. Yeah, You don't want that. File systems allows files to easly grow from say 4KB to 4GB or even Terabytes. Or shrink from Megabytes to kilobytes.
-   Organization into directories.
    >   Guess what! There's no concept of directories on a disk. File System implements this notion of directories. Underneath the hood directories are just files containing entries for other files. But you don't need to know that. That's taken care for you by the file systems.

&nbsp;

**What information do Files help Organize?**

-   Ownership and permissions.
    >   Imagine if you created a file on your multi user computer. You wouldn't want any other user (say your sister or brother) to edit your file, would you? File Systems provide this notion of owenership and permissions.
-   Access time, modification time, type, etc.
    >   File Systems provide other metadata about files such as access time, modification time, etc.


File Systems abstract away the Disks. That's their job. If you'd never heard (or had to take care about) any of the undesireable proprties I mentioned above (and there are lot more), File Systems have done their job well.


&nbsp;


>   The essence of abstractions is preserving information that is relevant in a given context, and forgetting information that is irrelevant in that context.
>
>   – John V. Guttag

&nbsp;

Oh My! that got a little out of hand. But, I think it's really important.

&nbsp;

## Ok. Now that it's out of the way, let's jump back to Why (which btw is really simple).

-   Reality:
    >   This is how Computers really work, and as a Computer Scientist or Engineer you should know how Computers really work.
-   Ubiquity:
    >   Operating Systems are everywhere and you are likely to eventually encounter them or their limitations.
-   Beauty:
    >   Operating Systems are examples of mature solutions to difficult Design and Engineering problems. Studying them will improve your ability to Design and Implement abstractions.
-   Design:
    >   Programming Operating Systems stresses the importance of careful Design and Specification before coding begins. You will learn the value of Design, probably the hard way.
-   Difficulty:
    >   Operating Systems are large existing code bases where new solutions have stringent performance requirements. While many Operating Systems concepts are elegantly simple, implementing them is not! Programming Operating Systems will make you a better programmer and improve all of your subsequent work.
-   Debugging:
    >   Debugging Operating Systems is challenging due to their multi- threaded nature and the lack of typical debugging support provided to applications. Again, Debugging Operating Systems will sharpen your debugging skills.


&nbsp;


>   akash


&nbsp;


-   [source][0]


[0]:https://www.ops-class.org