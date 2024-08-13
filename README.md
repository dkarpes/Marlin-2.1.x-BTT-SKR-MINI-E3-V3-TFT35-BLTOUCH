Download earlier versions of Marlin on the [Releases page](https://github.com/MarlinFirmware/Marlin/releases).
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <p align="center"><img src="buildroot/share/pixmaps/logo/marlin-outrun-nf-500.png" height="250" alt="MarlinFirmware's logo" /></p>

<h1 align="center">Marlin 3D Printer Firmware</h1>

<p align="center">
    <a href="/LICENSE"><img alt="GPL-V3.0 License" src="https://img.shields.io/github/license/marlinfirmware/marlin.svg"></a>
    <a href="https://github.com/MarlinFirmware/Marlin/graphs/contributors"><img alt="Contributors" src="https://img.shields.io/github/contributors/marlinfirmware/marlin.svg"></a>
    <a href="https://github.com/MarlinFirmware/Marlin/releases"><img alt="Last Release Date" src="https://img.shields.io/github/release-date/MarlinFirmware/Marlin"></a>
    <a href="https://github.com/MarlinFirmware/Marlin/actions/workflows/ci-build-tests.yml"><img alt="CI Status" src="https://github.com/MarlinFirmware/Marlin/actions/workflows/ci-build-tests.yml/badge.svg"></a>
    <a href="https://github.com/sponsors/thinkyhead"><img alt="GitHub Sponsors" src="https://img.shields.io/github/sponsors/thinkyhead?color=db61a2"></a>
    <br />
    <a href="https://fosstodon.org/@marlinfirmware"><img alt="Follow MarlinFirmware on Mastodon" src="https://img.shields.io/mastodon/follow/109450200866020466?domain=https%3A%2F%2Ffosstodon.org&logoColor=%2300B&style=social"></a>
</p>

<p>Additional documentation can be found at the [Marlin Home Page](https://marlinfw.org/).
Please test this firmware and let us know if it misbehaves in any way. Volunteers are standing by!

## Marlin 2.1 Bugfix Branch

__Not for production use. Use with caution!__

Marlin 2.1 takes this popular RepRap firmware to the next level by adding support for much faster 32-bit and ARM-based boards while improving support for 8-bit AVR boards. Read about Marlin's decision to use a "Hardware Abstraction Layer" below.

This branch is for patches to the latest 2.1.x release version. Periodically this branch will form the basis for the next minor 2.1.x release.</p>


   <p> <h1>Marlin-2.1.x-BTT-SKR-MINI-E3-V3-TFT35-BLTOUCH-NEOPIXEL_LED</h1>
    <p>This repository contains the configuration files for <a href="https://marlinfw.org/">Marlin 2.1.x</a> firmware tailored for a DIY 300x300x400 3D printer. It includes settings for a BTT TFT35 V3.0.1 display, a BLTouch auto bed leveling sensor, and a BTT SKR MINI E3 V3 mainboard.</p>
    <p>
    <h2>Features</h2>
    <ul>
        <li><strong>Firmware:</strong> <a href="https://marlinfw.org/">Marlin 2.1.x</a></li>
        <li><strong>Mainboard:</strong> BTT SKR MINI E3 V3 SMT32G0B0 / SMT32G0B1</li>
        <li><strong>Display:</strong> <a href="https://bigtree-tech.com/pages/download">BTT TFT35 V3.0.1</a> configured as Stock Display</li>
        <li><strong>Auto Bed Leveling:</strong> BLTouch (connected to Z-Probe pins)</li>
        <li><strong>Printer Size:</strong> 300x300x400 mm</li>
    </ul>
    </p>
   <p> <h2>Firmware (bin file)</h2>
    <p>Copy the firmware.bin file to your sd card and update your printer.</p>

  <p> <h2>Display Configuration</h2>
    <p>The BTT TFT35 V3.0.1 is set up to communicate over specific hardware UART and SPI pins, as defined in the <code>Configuration.adv.h</code> file:</p>
    
  <p> <h3>Hardware UART Pins</h3>
    <ul>
        <li><code>UART1_TX_PIN</code>: PA9 (default usage LCD connector)</li>
        <li><code>UART1_RX_PIN</code>: PA10 (default usage LCD connector)</li>
        <li><code>UART2_TX_PIN</code>: PA2 (default usage TFT connector)</li>
        <li><code>UART2_RX_PIN</code>: PA3 (default usage TFT connector)</li>
        <li><code>UART4_TX_PIN</code>: PC10 (default usage TMC UART)</li>
        <li><code>UART4_RX_PIN</code>: PC11 (default usage TMC UART)</li>
    </ul>
    
  <p>  <h3>SPI Pins</h3>
    <ul>
        <li><code>TFT_SCK_PIN</code>: PA5 (Serial Clock)</li>
        <li><code>TFT_MOSI_PIN</code>: PA7 (Master Out Slave In)</li>
        <li><code>TFT_CS_PIN</code>: PB6 (Chip Select)</li>
        <li><code>TFT_DC_PIN</code>: PB7 (Data/Command)</li>
        <li><code>TFT_RST_PIN</code>: PB8 (Reset)</li>
    </ul>
    
  <p>  <h2>Classic Marlin UI</h2>
    <p>If you prefer using the classic Marlin UI, connect the EXP1 or EXP2 connector to the mainboard and enable it in the configuration files.</p>
    
   <p> <h2>Getting Started</h2>
    <ol>
        <li>Clone this repository to your local machine.</li>
        <li>Follow the Marlin firmware build instructions to compile and upload the firmware to your 3D printer.</li>
        <li>Ensure all connections are made according to the pin configurations mentioned above.</li>
    </ol>
    
   <p> <h2>Contributing</h2>
    <p>Feel free to open issues or submit pull requests if you have improvements or suggestions.</p>
    
  <p>  <h2>License</h2>
    <p>This project is licensed under the MIT License.</p>
    
 <p>   <hr>
    
  <p>  <p>For detailed information and support, please refer to the official <a href="https://marlinfw.org/">Marlin documentation</a>.</p>

## Contributors

Marlin is constantly improving thanks to a huge number of contributors from all over the world bringing their specialties and talents. Huge thanks are due to [all the contributors](https://github.com/MarlinFirmware/Marlin/graphs/contributors) who regularly patch up bugs, help direct traffic, and basically keep Marlin from falling apart. Marlin's continued existence would not be possible without them.

## Project Leadership

Name|Role|Link|Donate
----|----|----|----
🇺🇸 Scott Lahteine|Project Lead|[[@thinkyhead](https://github.com/thinkyhead)]|[💸 Donate](https://marlinfw.org/docs/development/contributing.html#donate)
🇺🇸 Roxanne Neufeld|Admin|[[@Roxy-3D](https://github.com/Roxy-3D)]|
🇺🇸 Keith Bennett|Admin|[[@thisiskeithb](https://github.com/thisiskeithb)]|[💸 Donate](https://github.com/sponsors/thisiskeithb)
🇺🇸 Jason Smith|Admin|[[@sjasonsmith](https://github.com/sjasonsmith)]|
🇧🇷 Victor Oliveira|Admin|[[@rhapsodyv](https://github.com/rhapsodyv)]|
🇬🇧 Chris Pepper|Admin|[[@p3p](https://github.com/p3p)]|
🇳🇿 Peter Ellens|Admin|[[@ellensp](https://github.com/ellensp)]|[💸 Donate](https://ko-fi.com/ellensp)
🇺🇸 Bob Kuhn|Admin|[[@Bob-the-Kuhn](https://github.com/Bob-the-Kuhn)]|
🇳🇱 Erik van der Zalm|Founder|[[@ErikZalm](https://github.com/ErikZalm)]|

## License

Marlin is published under the [GPL license](/LICENSE) because we believe in open development. The GPL comes with both rights and obligations. Whether you use Marlin firmware as the driver for your open or closed-source product, you must keep Marlin open, and you must provide your compatible Marlin source code to end users upon request. The most straightforward way to comply with the Marlin license is to make a fork of Marlin on Github, perform your modifications, and direct users to your modified fork.</body>
</html>

