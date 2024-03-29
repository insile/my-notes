##### I/O
- I/O 是 Input/Output（输入/输出）的缩写，是计算机领域中用来描述数据在计算机系统内部和外部之间传输的过程的术语。
- 在计算机中，输入（Input）指的是将外部数据引入计算机系统中，供计算机处理。例如，键盘输入、鼠标输入、网络数据接收等都属于输入操作。
- 输出（Output）指的是将计算机系统中的数据传送到外部，供用户或其他系统使用。例如，屏幕显示、打印输出、网络数据发送等都属于输出操作。
- I/O 操作是计算机系统中的基本操作之一，用于在计算机与外部设备或其他系统之间传输数据。在计算机编程中，I/O 操作通常包括从文件中读取数据、写入数据到文件、从网络接收数据、发送数据到网络等。不同类型的设备和资源可能会有不同的 I/O 操作方式和机制。
- 在编程中，I/O 操作通常需要考虑效率、可靠性和错误处理等因素。为了提高性能，常常会使用缓冲、异步等技术。同时，对于可能出现的错误，需要进行适当的异常处理。
- 总之，I/O 是计算机系统中数据传输的重要环节，涵盖了数据输入和输出的各种操作。
##### I/O 关键概念
- **流（Stream）**：流是一种抽象的数据传输方式，用于在程序和外部设备之间传输数据。流可以是输入流（用于读取数据）或输出流（用于写入数据）。流可以是字节流（用于处理二进制数据）或字符流（用于处理文本数据）。
- **文件对象（file object）**：对外提供面向文件 API 以使用下层资源的对象（带有 read() 或 write() 这样的方法）。根据其创建方式的不同，文件对象可以处理对真实磁盘文件，对其他类型存储，或是对通讯设备的访问（例如标准输入/输出、内存缓冲区、套接字、管道等等）。文件对象也被称为 文件类对象 或 流。
- **缓冲（Buffering）**：缓冲是一种机制，用于在内存中暂存数据，减少对底层资源（如文件、网络）的频繁读写操作，从而提高性能。
- **文本 I/O**（Text Input/Output）是一种用于处理文本数据的输入输出操作。文本 I/O 在处理文本文件、字符串和文本流时非常有用，它允许你读取和写入以字符为单位的文本数据。
- **二进制 I/O**（Binary Input/Output）是一种用于处理二进制数据的输入输出操作。与文本 I/O 不同，二进制 I/O 处理的是以字节为单位的数据，适用于处理图像、音频、视频等非文本的文件和数据。
- **原始 I/O**（Raw Input/Output）是一种用于处理原始字节数据的输入输出操作。它提供了对数据的最低级别的访问，适用于需要直接读写二进制数据的情况，如设备驱动、底层通信等。
- **同步（Synchronous）和异步（Asynchronous）**：同步 I/O 是一种阻塞式的操作，程序会等待 I/O 操作完成后再继续执行；异步 I/O 是一种非阻塞式的操作，程序可以继续执行其他任务，当 I/O 操作完成时会通知程序。
- **阻塞（Blocking）和非阻塞（Non-blocking）**：阻塞式 I/O 是指程序在执行 I/O 操作时会被阻塞，直到操作完成；非阻塞式 I/O 是指程序在执行 I/O 操作时不会被阻塞，而是立即返回
- **网络 I/O**：网络 I/O 是在计算机网络中传输数据的操作，包括数据的接收和发送。网络 I/O 涉及套接字（socket）编程，用于实现不同主机之间的通信。
- **流式 I/O（Streaming I/O）**：流式 I/O 是指通过流一次性处理大量数据，而不是一次性将所有数据加载到内存中。这在处理大型数据集或网络传输时特别有用。


