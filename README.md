# epsolar-tracer
Tools for EPsolar Tracer BN solar charge controller
===================================================
![Img](img/epsolar_tracer_bn.jpg)

This is the second generation of the EPsolar Tracer solar charge controller. 
You need RS-485 adapter for communication. The first generation controller 
used RS-232 and a different protocol. see https://github.com/xxv/tracer.

[Product link](http://www.epsolarpv.com/en/index.php/Product/pro_content/id/573/am_id/136)  
[Windows software & nice pictures](http://gwl-power.tumblr.com/tagged/tracer)

Linux driver for Exar USB UART
------------------------------
In [directory](xr_usb_serial_common-1a) there is a Linux driver for Exar based USB RS-485 adapter.  
[Original source](https://www.exar.com/common/content/default.aspx?id=10296)

Protocol
--------
[Protocol](http://www.solar-elektro.cz/data/dokumenty/1733_modbus_protocol.pdf)
See for [windows capture](archive/epsolar.txt) for some extra commands.

Python module
-------------
Uses modbus library (https://github.com/bashwork/pymodbus)  
Example output
```
# python info.py 
Manufacturer: 'EPsolar Tech co., Ltd'
Model: 'Tracer2215BN'
Version: 'V02.05+V07.12'
Charging equipment rated input voltage = 150.0V
Charging equipment rated input voltage = 150.0V
Charging equipment rated input current = 20.0A
...
```
