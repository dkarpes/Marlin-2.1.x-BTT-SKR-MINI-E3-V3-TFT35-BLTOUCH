<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
</head>
<body>
    <h1>Marlin-2.1.x-BTT-SKR-MINI-E3-V3-TFT35-BLTOUCH-NEOPIXEL_LED</h1>
    <p>This repository contains the configuration files for <a href="https://marlinfw.org/">Marlin 2.1.x</a> firmware tailored for a DIY 300x300x400 3D printer. It includes settings for a BTT TFT35 V3.0.1 display, a BLTouch auto bed leveling sensor, and a BTT SKR MINI E3 V3 mainboard.</p>
    <p>
    <h2>Features</h2>
    <ul>
        <li><strong>Firmware:</strong> <a href="https://marlinfw.org/">Marlin 2.1.x</a></li>
        <li><strong>Mainboard:</strong> BTT SKR MINI E3 V3 SMT32G0B0 / SMT32G0B1</li>
        <li><strong>Display:</strong> <a href="https://bigtree-tech.com/pages/download">BTT TFT35 V3.0.1</a> configured as TFTGLCD_PANEL_I2C</li>
        <li><strong>Auto Bed Leveling:</strong> BLTouch (connected to Z-Probe pins)</li>
        <li><strong>Printer Size:</strong> 300x300x400 mm</li>
    </ul>
    
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
</body>
</html>
