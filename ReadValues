import time
import Adafruit_GPIO.SPI as SPI
import Adafruit_MCP3008
# Hardware SPI configuration (its best with the ADC)
SPI_PORT = 0
SPI_DEVICE = 0
mcp = Adafruit_MCP3008.MCP3008(spi=SPI.SpiDev(SPI_PORT, SPI_DEVICE))
# read in the value from channel 0 of the ADC
input_value = mcp.read_adc(0)
# input_value2 = mcp.read_adc(2)
# print the value
while True:
	input_value = mcp.read_adc(0)
	# input_value = mcp.read_adc(2)		
	print 'input_value is: ' + str(input_value)
	# print 'input value2 is: ' + str(input_value2)
	time.sleep(0.5)

