## ERA ##

Embedded Rack Architecture 2.0 Specifications and Reference Designs 

-----------------------------------------------------

This repository contains Open Source Hardware Reference Designs for ERA 2.0

-----------------------------------------------------

The Backplane Reference is a simple, passive, fourteen (14) slot Backplane in a compact form factor.
The Embedded Rack Architecture supports the following signals:

* Ground (GND)        (4 pins)
* +12V DC (1A min)    (2 pins)
* -12V DC (.5A min)   (2 pins)
* +5V DC (1A min)     (2 pins)
* Control Voltage In  (1 pin)   (-5.0 to 5.0 volts)
* Control Voltage Out (1 pin)   (-5.0 to 5.0 volts)
* Gate In             (1 pin)   (0.0 - 5.0 volts)
* Gate Out            (1 pin)   (0.0 - 5.0 volts)
* I2C SDA             (1 pin)   (0.0 - 5.0 volts)
* I2C SCL             (1 pin)   (0.0 - 5.0 volts)

Because a reverse polarity power connection can short the SDA & SCL pins to the +12V DC pins,
the ERA specification includes a simple N-Channel Mosfet circuit that provides both Level Shifting 
(for lower voltage CPU interfaces) and over-voltage/reverse-voltage protection on the ERA I2C Signals (SDA & SCL). 
The circuit is described in the ERA Module Reference Design.

-----------------------------------------------------
For more information, please see the [ERA Wiki](https://github.com/patternagents/ERA/wiki)!
-----------------------------------------------------

![Embedded Rack 2.0 Backplane Reference Design](https://github.com/patternagents/ERA/blob/master/revisions/Backplane_Reference_R2_0/images/Backplane_Reference_R2_0_top.png)

-----------------------------------------------------
