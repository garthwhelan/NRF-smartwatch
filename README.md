# NRF-smartwatch

Program for the nRF52810 biofeedback device I am making

To make, just type make

To program with openocd:

 sudo openocd -f ~/openocd/tcl/interface/stlink.cfg -f ~/openocd/tcl/target/nrf52.cfg -c "program _build/nrf52810_xxaa.hex verify reset exit"
 sudo openocd -f ~/openocd/tcl/interface/stlink.cfg -f ~/openocd/tcl/target/nrf52.cfg -c "program softdevice.hex verify reset exit"
 
 Sometimes takes multiple tries, but that might just be my hardware setup.
