# Image File Reader

A image file reader and generator.

---

**Note**: In this repository, "*reader*" is defined as *something that analyzes 
information*; therefore, this repository will not contain anything with the 
ability to display images, but it will be able to generate images.

---

## Supported file formats

* The Netpbm file format family:
    * Portable BitMap `.pbm`
    * Portable GrayMap `.pgm`
    * Portable PxMap `.ppm`

## Help

```
Usage:
    `ifr [command] <comand-input> [option]`

Command:
    help                        Displays the program's help information.
    read <source-file>          Reads an image file.
                                If the *format* option is not specified, it reads the file as the file extension. 

Options:
    -h | --help                 Displays the command's help information.
                                If a command is not given, it will display the results of the `help` command.
    -f | --format               Specifies the file format to be read/generated.
```

## Running

Prerequisites:
    

### Via the binary

1. Look in the `/Output` directory, there should be a generated x64 binary named `ifr.exe`.
2. Execute it using a terminal with the command `./ifr.exe` followed by a command, command input, and then options.
    * Note: Solely executing `./ifr.exe` will automatically use the `help` command.

### Via building

Prerequisites:
    * A C++ compiler that supports the C++20 standard (e.g. Clang and GCC).
    * [GNU Make](https://www.gnu.org/software/make).

Steps:
    1. Execute `make build` or just `make`.
    1. Follow the steps specified in the **Via the binary** subsection within the **Running** section in this document.
