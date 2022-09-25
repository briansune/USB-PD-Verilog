# USB-PD-Verilog

This example shows how to trigger USB Type-C Power Delivery via BMC "Biphase Mark Coding"

The on board IO bank can be tuned to the voltage level of USB type-C CC lines while the restriction of this FPGA dev board is avoiding to do so.

Meanwhile, the purpose of additional PCB is to create a differential voltage for LVDS and an additional driver to the CC1,CC2 line.

The overall bill-of-materials (BOM) can be as low as two resistor as long as the IO bank voltage is meeting the voltage requirement of CC line.

| Type	| Usage |
|-------|-------|
| LUT	| 863	|
| FF	| 912	|
| IO	| 11	|
| BUFG	| 2	|
| MMCM	| 1	|

# Demo Board and FPGA - Spartan 7

![Alt text](image/demo.JPG?raw=true "Title")

## Reference Links:
1: https://www.usbzh.com/article/detail-368.html

2: http://kevinzhengwork.blogspot.com/2014/09/usb-power-delivery-protocol-layer.html

3: https://www.embedded.com/usb-type-c-and-power-delivery-101-power-delivery-protocol/

4: https://usbchargingblog.wordpress.com/2020/02/22/how-to-sniff-pd-source-capability-and-monitor-pd-negotiations-without-a-pd-analyzer/

5: https://www.chromium.org/chromium-os/twinkie/

6: https://blog.csdn.net/xp562870732/article/details/108501283
