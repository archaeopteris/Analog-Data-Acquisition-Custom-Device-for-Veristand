# Analog-Data-Acquisition-Custom-Device-for-Veristand
This is a Custom Device for **Veristand 2019** that reads analog input data from the DAQ card. PXIe-6356 has been used as an example, but any other DAQ card should also work, provided that it could be used using NI DAQmx drivers.

## Device Interface
The Custom Device accept 4 input parameters that should be configured prior to deploying to the target throught the System Explorer of the Veristand.

![CD Interface](https://raw.githubusercontent.com/archaeopteris/Analog-Data-Acquisition-Custom-Device-for-Veristand/master/Picd/CD%20Main%20Page.PNG?raw=true)

The DAQmx Physical Channels names should match the names found in NI Measurement and Automation.

The number of analog input channels that is going to be read, as well as the analog input terminal configuration has been hard codded in this example, but it could be easily changed with slight modifications to the code. The Input terminal configuration is set to differential.
![Channel selection](https://raw.githubusercontent.com/archaeopteris/Analog-Data-Acquisition-Custom-Device-for-Veristand/master/Picd/Channel%20Specification.PNG?raw=true)


