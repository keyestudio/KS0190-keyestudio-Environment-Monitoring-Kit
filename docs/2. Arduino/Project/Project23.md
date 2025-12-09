### Project 23 TEMT6000 Ambient Light Sensor

![](media/image-20251204092248449.png)

**1.Introduction** 

TEMT6000 is an audion photoconductive sensor. Its illumination intensity is proportional to current of base electrode. It is very easy to use. Just connect the base electrode to input of analog voltage. You can know current intensity by detecting the voltage value.

**2.Hardware Required**

- Arduino Board *1
- V5 Shield*1
- USB Cable*1
- Ambient Light Sensor*1
- Dupont Line*3

**3.Circuit Connection**

![](media/wps5-1764811486080-1.png)

**4.Sample Code**

```c
void setup() 
{
  // initialize serial communication at 9600 bits per second:
  Serial.begin(9600);
}

// the loop routine runs over and over again forever:
void loop() 
{
  // read the input on analog pin 0:
  int sensorValue = analogRead(A0);
  // print out the value you read:
  Serial.println(sensorValue);
  delay(1);        // delay in between reads for stability
}
```

**5.Result**

After uploading the codes, open serial monitor, and you can see the value decrease with intensity decreasing. Otherwise, the value increases.