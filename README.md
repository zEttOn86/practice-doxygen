### Practice doxygen
This project refer to [qedsoftware/doxygen-demo](https://github.com/qedsoftware/doxygen-demo).
For more details, refer to [qedsoftware/doxygen-demo](https://github.com/qedsoftware/doxygen-demo).


### Build and Use
To Build this project, try as follows:
```
mkdir build && cd build
cmake ..
cmake --build .
```
  
Afterwards, your tree structure should look like this:
```
.
├── CMakeLists.txt
├── README.md
├── build
│   ├── CMakeCache.txt
│
└── src
    ├── CMakeLists.txt
    ├── circle.cpp

```

And you can execute the program as follows:
```
./src/shape_demo
```

### Build doxygen doc

```
sudo apt install doxygen
sudo apt install texlive-latex-base texlive-fonts-recommended texlive-fonts-extra texlive-latex-extra
```



### Reference
- [CMake : out-of-sourceビルドで幸せになる](https://qiita.com/osamu0329/items/7de2b190df3cfb4ad0ca)
- [qedsoftware/doxygen-demo](https://github.com/qedsoftware/doxygen-demo)
- [Quick setup to use Doxygen with CMake](https://vicrucann.github.io/tutorials/quick-cmake-doxygen/)
- [Document your CMake code within doxygen](http://jesnault.fr/website/document-your-cmake-code-within-doxygen/)