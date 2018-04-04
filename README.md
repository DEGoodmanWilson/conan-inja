[ ![Download](https://api.bintray.com/packages/degoodmanwilson/opensource/inja%3ADEGoodmanWilson/images/download.svg) ](https://bintray.com/degoodmanwilson/opensource/inja%3ADEGoodmanWilson/_latestVersion)

[Conan.io](https://conan.io) package for [inja](https://github.com/pantor/inja) project

The packages generated with this **conanfile** can be found in [Bintray](https://bintray.com/degoodmanwilson/opensource/inja%3ADEGoodmanWilson/_latestVersion).

## For Users: Use this package

### Basic setup

    $ conan remote add vthiery https://api.bintray.com/conan/vthiery/conan-packages
    $ conan remote add DEGoodmanWilson https://api.bintray.com/conan/degoodmanwilson/opensource
    $ conan install inja/1.0.0@DEGoodmanWilson/stable

### Project setup

If you handle multiple dependencies in your project is better to add a *conanfile.txt*

    [requires]
    inja/[~=1.0]@DEGoodmanWilson/stable

    [generators]
    txt

Complete the installation of requirements for your project running:

    $ mkdir build && cd build && conan install ..

Note: It is recommended that you run conan install from a build directory and not the root of the project directory.  This is because conan generates *conanbuildinfo* files specific to a single build configuration which by default comes from an autodetected default profile located in ~/.conan/profiles/default .  If you pass different build configuration options to conan install, it will generate different *conanbuildinfo* files.  Thus, they should not be added to the root of the project, nor committed to git.

## For Packagers: Publish this Package

The example below shows the commands used to publish to `degoodmanwilson` conan repository. To publish to your own conan respository (for example, after forking this git repository), you will need to change the commands below accordingly.

## Issues

If you are interested to open a new issue, please visit https://github.com/degoodmanwilson/conan-inja/issues.

## Build and package

The following command both runs all the steps of the conan file, and publishes the package to the local system cache.  This includes downloading dependencies from "build_requires" and "requires" , and then running the build() method.

    $ conan create DEGoodmanWilson/stable

## Add Remote

    $ conan remote add DEGoodmanWilson "https://api.bintray.com/conan/degoodmanwilson/opensource"

## Upload

    $ conan upload inja/1.0@DEGoodmanWilson/stable --all -r DEGoodmanWilson

## License
[LICENSE_TYPE](LICENSE.md)
