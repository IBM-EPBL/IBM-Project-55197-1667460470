#LED BLINKING

import RPi.GPIO as GPIO
	from time import sleep
		
	GPIO.setwarnings(False)
	GPIO.setmode(GPIO.BOARD)
	GPIO.setup(8, GPIO.OUT, initial=GPIO.LOW)
	
	while True:                      #infinite loop
	    GPIO.output(8, GPIO.HIGH)               # Turn on
	    print("The LED is ON")
	    sleep(5)                     # Sleep for 5 second
	    
	    GPIO.output(8, GPIO.LOW)                # Turn off
	    print("The LED is OFF")
	    sleep(5)                     # Sleep for 5 second
