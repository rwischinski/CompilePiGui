# CompilePiGui
 Python GUI for ComfilePi (http://comfiletech.com/linux-panel-pc/) to display status/control CP-IO22-A4-2 - Digital & Analog IO Board.
 
 ComfilePi is an industrial Panel PC, using Raspberry's Compute module.
 
 Also successfully tested (but not included in executable): Modbus RTU Client, using ComfilePi's RS485 port.
 
 Single file executable (ComfileGPIO) created with pyinstaller.
 
 Runs in full screen when launched. Press Escape to exit full screen mode.
 
 * 100% pure Python3
 * Uses tkinter
 * uses PIGPIO daemon (by default installed and running on ComfilePi) for GPIO communication
 * uses I2C for ADS1115 (4 analog inputs) and MCP4725 (2 analog outputs) communication
 * all GPIO communication and GUI updates run in separate thread; results in very responsive interface
 * includes the following widgets:
   * Indicator: LED
   * Gauge
   * Slide switch
   * Numeric popup keypad
   * Alphanumeric popup keypad
