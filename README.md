# Twitch Chat for NES (Requires TAS Replay Device)

NES game that is also a Twitch chat client

**_Twitch Chat for NES was created by Vi Grey (https://vigrey.com) <vi@vigrey.com> and is licensed under the BSD 2-Clause License._**

### Description:
**This NES ROM has yet to be tested with a TAS replay device.  This notice will be removed once it has been successfully tested with a TAS replay device**

This is an NROM NES ROM that is also a Twitch chat client that connects to Twitch using a TAS replay device like the TAStm32.

### Platforms:
- GNU/Linux

### Build Dependencies:
- asm6 _(You'll probably have to build asm6 from source.  Make sure the asm6 binary is named **asm** and that the binary is executable and accessible in your PATH. The source code can be found at **http://3dscapture.com/NES/asm6.zip**)_
- zip

### Build NES ROM:
From a terminal, go to the the main directory of this project (the directory this README.md file exists in), you can then build the NES ROM with the following command.

    $ make

The resulting NES ROM will be located at **bin/twitch-nes.nes**

### Cleaning Build Environment:
If you used `make` to build the payload binary, you can run the following command to clean up the build environment.

    $ make clean

### NES-ZIP Polyglot File
After building the NES ROM, you may notice that it is also a functioning ZIP file.  Unzipping the NES ROM will extract the source code for the NES ROM.  This allows the NES ROM to be a Quine of sorts, where everything required to create the NES ROM from scratch is self contained in the NES ROM. You can unzip the NES ROM with the following command.

    $ unzip twitch-nes.nes

Unzipping the NES ROM will result in a directory called **discord-nes**, which will include all of the source code for the NES ROM.

### License:
    Copyright (C) 2020, Vi Grey
    All rights reserved.

    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions
    are met:

        1. Redistributions of source code must retain the above copyright
           notice, this list of conditions and the following disclaimer.
        2. Redistributions in binary form must reproduce the above copyright
           notice, this list of conditions and the following disclaimer in the
           documentation and/or other materials provided with the distribution.

    THIS SOFTWARE IS PROVIDED BY AUTHOR AND CONTRIBUTORS \`\`AS IS'' AND
    ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
    IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
    ARE DISCLAIMED. IN NO EVENT SHALL AUTHOR OR CONTRIBUTORS BE LIABLE
    FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
    DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
    OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
    HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
    LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
    OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
    SUCH DAMAGE.

