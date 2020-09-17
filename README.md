HelloIommuPkg
==============

HelloIommuPkg is a sample DXE runtime driver demonstrating how to program DMA
remapping, one of the Intel VT-d features, to protect the system from DMA access.

This project is meant to show a simplified yet functioning code example for learning
purposes and not designed for actual use in production systems.

For more information about this project see my blog post: [Introductory Study of IOMMU (VT-d) and Kernel DMA Protection on Intel Processors ](https://standa-note.blogspot.com/2020/05/introductory-study-of-iommu-vt-d-and.html)

Building
---------

1. Set up edk2 build environment
2. Copy `HelloIommuPkg` as `edk2\HelloIommuPkg`
3. On the edk2 build command prompt, run the below command:
    ```
    > edksetup.bat
    > build -t VS2019 -a X64 -b NOOPT -p HelloIommuPkg\HelloIommuPkg.dsc
    or
    > build -t CLANGPDB -a X64 -b NOOPT -p HelloIommuPkg\HelloIommuPkg.dsc
    ```
    Or on WSL or Linux,
    ```
    $ . edksetup.sh
    $ build -t GCC5 -a X64 -b NOOPT -p HelloIommuPkg/HelloIommuPkg.dsc
    ```

Also, pre-compiled binary files are available at the Release page.
