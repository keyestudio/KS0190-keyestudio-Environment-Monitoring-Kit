### Project 8 Active Buzzer

![](media/image-20251203153931287.png)

**1.Introduction** 

Active buzzer is widely used on computer, printer, alarm, electronic toy, telephone, timer etc as a sound making element. It has an inner vibration source. Simply connect it with 5V power supply, it can buzz continuously.  

**2.Hardware Required**

- Arduino Board *1
- USB Cable *1
- Active Buzzer*1
- Breadboard*1 
- Breadboard Jumper Wires

**3.Circuit Connection**

![](media/wps14.jpg)

When connecting the circuit, pay attention to the positive & the negative poles of the buzzer. In the photo, you can see there are red and black lines. When the circuit is finished, you can begin programming.

**4.Sample Code**

Program is simple. You control the buzzer by outputting high/low level. 

```c
int buzzer=8;// initialize digital IO pin that controls the buzzer

void setup() 
{ 
    pinMode(buzzer,OUTPUT);// set pin mode as “output”
}

void loop() 
{
	digitalWrite(buzzer, HIGH); // produce sound
}
```

**5.Result**
After downloading the program, the buzzer experiment is completed. You can see the buzzer is ringing.