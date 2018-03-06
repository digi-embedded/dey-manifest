Digi Embedded Yocto (DEY) manifest
==================================

This repository contains the manifest files for the Digi Embedded Yocto
distribution for [Digi's Embedded modules](https://www.digi.com/products/embedded-systems).

Installing Digi Embedded Yocto
------------------------------

To download Digi Embedded Yocto, you need the repo tool.

Follow these steps to install Digi Embedded Yocto:

1. Download repo to a directory within your path and add execution permissions.

    ```
    $ sudo curl -o /usr/local/bin/repo http://commondatastorage.googleapis.com/git-repo-downloads/repo
    $ sudo chmod a+x /usr/local/bin/repo
    ```

2. Create an installation folder with user write permissions; for example,
    `/usr/local/dey-2.4` and navigate to that folder.

    ```
    $ sudo install -o <your-user> -g <your-group> -d /usr/local/dey-2.4
    $ cd /usr/local/dey-2.4
    ```

    Note: You can get your primary user and group using the `id` command.

3. Use repo to download Digi Embedded Yocto.

    ```
    $ repo init -u https://github.com/digi-embedded/dey-manifest.git -b rocko
    $ repo sync -j8 --no-repo-verify
    ```

More information about [Digi Embedded Yocto](https://github.com/digi-embedded/meta-digi).

License
-------
Copyright 2018, Digi International Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
