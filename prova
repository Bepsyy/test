
import smbus
import time

bus = smbus.SMBus(1)

DEVICE  = 0x23 #indirizzo dispositivo
IODIRA  = 0x00 #banco A
IODIRB  = 0x01 #banco B
OLATA   = 0x14 #registro di output A
OLATB   = 0x15 #registro di output B
GPIOA   = 0x11 #registro di input A
GPIOB   = 0x12 #registro di input B


bus.write_byte_data(DEVICE,IODIRA,0)
bus.write_byte_data(DEVICE,IODIRB,0)

# tutti i bit a 0
bus.write_byte_data(DEVICE,OLATA,0)
bus.write_byte_data(DEVICE,OLATB,0)

bus.write_byte_data(DEVICE,OLATA,128)
#bus.write_byte_data(DEVICE,OLATB,2)

time.sleep(5)

# tutti i bit a 0
bus.write_byte_data(DEVICE,OLATA,0)
bus.write_byte_data(DEVICE,OLATB,0)
