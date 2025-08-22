# Windows изнутри

### Введение

Windows Internals, Seventh Edition is intended for advanced computer professionals\
(developers, security researchers, and system administrators) who want to understand how the core components of the Microsoft Windows 10 and Windows Server 2016\
operating systems work internally. With this knowledge, developers can better comprehend the rationale behind design choices when building applications specific to the\
Windows platform. Such knowledge can also help developers debug complex problems.\
System administrators can benefit from this information as well, because understanding how the operating system works “under the hood” facilitates an understanding of\
the performance behavior of the system and makes troubleshooting system problems\
much easier when things go wrong. Security researchers can figure out how software\
applications and the operating system can misbehave and be misused, causing undesirable behavior, while also understanding the mitigations and security features modern\
Windows offers against such scenarios. After reading this book, you should have a better\
understanding of how Windows works and why it behaves as it does.

### Предупреждение

Because this book describes undocumented behavior of the internal architecture and the\
operation of the Windows operating system (such as internal kernel structures and functions), this content is subject to change between releases.\
By “subject to change,” we don’t necessarily mean that details described in this book\
will change between releases, but you can’t count on them not changing. Any software\
that uses these undocumented interfaces, or insider knowledge about the operating\
system, might not work on future releases of Windows. Even worse, software that runs\
in kernel mode (such as device drivers) and uses these undocumented interfaces might\
experience a system crash when running on a newer release of Windows, resulting in\
potential loss of data to users of such software.\
In short, you should never use any internal Windows functionality, registry key,\
behavior, API, or other undocumented detail mentioned in this book during the development of any kind of software designed for end-user systems, or for any other purpose\
other than research and documentation. Always check with the Microsoft Software\
Development Network (MSDN) for official documentation on a particular topic first.

### Требования перед прочтением

The book assumes the reader is comfortable with working on Windows at a power-user\
level, and has a basic understanding of operating system and hardware concepts, such\
as CPU registers, memory, processes, and threads. Basic understanding of functions,\
pointers, and similar C programming language constructs is beneficial in some sections.

### Описание глав

The book is divided into two parts (as was the sixth edition), the first of which you’re\
holding in your hands.\
■ Chapter 1, “Concepts and tools,” provides a general introduction to Windows\
internals concepts and introduces the main tools used throughout the book. It’s\
critical to read this chapter first, as it provides the necessary background needed\
for the rest of the book.\
■ Chapter 2, “System architecture,” shows the architecture and main components\
that comprise Windows and discusses them in some depth. Several of these concepts are dealt with in greater detail in subsequent chapters.\
■ Chapter 3, “Processes and jobs,” details how processes are implemented in\
Windows and the various ways of manipulating them. Jobs are also discussed\
as a means for controlling a set of processes and enabling Windows Container\
support.\
■ Chapter 4, “Threads,” details how threads are managed, scheduled, and otherwise manipulated in Windows.\
■ Chapter 5, “Memory management,” shows how the memory manager uses physical and virtual memory, and the various ways that memory can be manipulated\
and used by processes and drivers alike.\
■ Chapter 6, “I/O system,” shows how the I/O system in Windows works and\
integrates with device drivers to provide the mechanisms for working with I/O\
peripherals.\
■ Chapter 7, “Security,” details the various security mechanisms built into Windows,\
including mitigations that are now part of the system to combat exploits.

