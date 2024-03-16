# SPI
This Verilog module implements a simple Serial Peripheral Interface (SPI) block flow controller. It facilitates communication between a master device (e.g., microcontroller) and a slave device using the SPI protocol. The module generates SPI signals such as chip select (spi_cs_l), clock (spi_clk), and data (spi_data) based on the provided clock signal (clk) and input data (indata). It also provides a counter (counter) indicating the current state of data transmission.

Module Ports:

clk (input): Clock input signal for synchronization.
rst (input): Reset signal to initialize the module's state.
indata (input[15:0]): Input data to be transmitted via SPI.
spi_cs_l (output): SPI chip select signal.
spi_clk (output): SPI clock signal.
spi_data (output): SPI data signal.
counter (output[4:0]): Counter indicating the current state of data transmission.
Usage:
Instantiate this module in your Verilog design and provide appropriate connections to the input and output ports. Ensure that the clock signal (clk) and reset signal (rst) are properly connected and synchronized. Connect the input data (indata) to be transmitted via SPI.
