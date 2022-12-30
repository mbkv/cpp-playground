# CPP Playground

CPP Playground is the minimal viable project you can make with both cmake and
conan. The C++ community has an awful track record of being extremely obtuse.
The fact you need to read cmake or conan docs at all shows the community has
been going the wrong direction. If all you wanted was to run some C++ code you
thought of at 3am, you'd be SOL. This project serves as a temporary measure
until C++ finally figures out a system where `conan --init; make` is all you
need in setting up a project (or [Jonathan Blow's
Jai](https://github.com/BSVino/JaiPrimer/blob/master/JaiPrimer.md))

Assuming you have both cmake and conan installed, all you need to do is:

```bash
git clone https://github.com/mbkv/cpp-playground && cd cpp-playground

mkdir build
cd build
conan install ..
cmake ..
make
```

And then you can run your executible with:

```bash
$ ./bin/playground
Hello from utils!
Hello from main!
```

