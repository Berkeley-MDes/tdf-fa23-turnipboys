# Report #4 - Week of 9/21/2023

## Aylish Turner

### Reflections

#### Class Recap

I was so happy to turn in my phone stand on Thursday and then be done with the first project after submitting my PDF on Monday. I enjoyed the process, but it was a lot of mental labor. I'm very curious to learn what we'll be doing in this second project.

Also on Monday, Jeff gave a very interesting lecture on microcontrollers and the Digital Ecosystem. I was already familiar with the term "digital ecosystem" (which I had actually learned about in an art class!), but my knowledge on microcontrollers is far more limited. I've worked with a Raspberry Pi before and just did very very simple things many years ago. I don't know much about electronics, wires, and all of this other stuff, so I'm genuinely very excited to learn more about it. It makes me feel like a mad scientist. :P

#### Homework - Photon2 Tutorial

I set up my Particle account. Note: I must use the Google Chrome browser to run the Particle setup (does not work with Firefox).

I connected my P2 device to my computer. It then installed Device OS onto my P2. In order to do this, it put the P2 into Device Firmware Upgrade (DFU) mode. This made the P2 start rapidly blinking with a green light (the blue light remained on). As it was updating, the light began blinking at different rates in different colors.

The P2 when I connected it to my laptop:

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/20230920_194419.jpg)

The P2 as it was updating:

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/20230920_194639.jpg)

On the "Organize your Particle device" page, it told me to select an existing organization and product for my device. My only organization available was my "Personal Sandbox," so I selected that. I didn't have any products available, so I created a new one and named it Baby Worm Photon 2 / P2s (this is because my laptop is called "Worm"). The name is baby_worm :)

I then connected my baby_worm to the Wi-Fi. I had a lot of trouble with this step because my only available options were berkeley-visitor and berkeley-iot. But neither of these would work (both required a password, but iot Wi-Fi wouldn't work without the Mac Address and the visitor Wi-Fi didn't have a password that I could put in). I decided to set up my hotspot and by a miracle it actually worked (I've had a lot of hotspot issues). So yayyyy.

After that I followed the directions for finding the Mac Address of my P2. I will not reveal it...but it is a satisfying combination of numbers. >:)

I created a new device for my baby_worm under the Berkeley-IOT Wi-Fi using the Mac Address.

Then baby_worm was finally connected to the Berkeley-IOT network! Yayyyyyy!!!!!!!

#### Hello World

Oh...the classic. Every time I learn a new language or IDE I always do the "Hello World" script! I've never used Particle Web IDE but I've used in-browser IDEs that are very similar. I learned that the Particle Web IDE programming language is Arduino C. I know C# and Python, so I thought that it looked somewhat familiar.

Here it is running the Hello World print loop:

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/helloWorld.PNG)

And here it is introducing itself as Baby Worm!:

![](https://github.com/Berkeley-MDes/tdf-fa23-turnipboys/blob/main/weekly-reports/babyWorm.PNG)

#### Blinking LED

Blinking blue LED code:
```
// We define MY_LED to be the LED that we want to blink.
//
// In this tutorial, we're using the blue D7 LED (next to D7 on the Photon
// and Electron, and next to the USB connector on the Argon and Boron).
const pin_t MY_LED = D7;

// The following line is optional, but recommended in most firmware. It
// allows your code to run before the cloud is connected. In this case,
// it will begin blinking almost immediately instead of waiting until
// breathing cyan,
SYSTEM_THREAD(ENABLED);

// The setup() method is called once when the device boots.
void setup()
{
	// In order to set a pin, you must tell Device OS that the pin is
	// an OUTPUT pin. This is often done from setup() since you only need
	// to do it once.
	pinMode(MY_LED, OUTPUT);
}

// The loop() method is called frequently.
void loop()
{
	// Turn on the LED
	digitalWrite(MY_LED, HIGH);

	// Leave it on for one second
	delay(1s);

	// Turn it off
	digitalWrite(MY_LED, LOW);

	// Wait one more second
	delay(1s);

	// And repeat!
}
```

Controlling LED blink over Internet code:
```
// We define MY_LED to be the LED that we want to blink.
//
// In this tutorial, we're using the blue D7 LED (next to D7 on the Photon
// and Electron, and next to the USB connector on the Argon and Boron).
const pin_t MY_LED = D7;

// The following line is optional, but recommended in most firmware.
// It allows your code to run before the cloud is connected.
SYSTEM_THREAD(ENABLED);

// This function is called when the Particle.function is called
int ledToggle(String command)
{
    if (command.equals("on"))
    {
        digitalWrite(MY_LED, HIGH);
        return 1;
    }
    else if (command.equals("off"))
    {
        digitalWrite(MY_LED, LOW);
        return 0;
    }
    else
    {
        // Unknown option
        return -1;
    }
}

// The setup() method is called once when the device boots.
void setup()
{
    // In order to set a pin, you must tell Device OS that the
    // pin is an OUTPUT pin.
    // This is often done from setup() since you only need to
    // do it once.
    pinMode(MY_LED, OUTPUT);

    // This registers a function call. When the function "led"
    // is called from the cloud, the ledToggle() function above
    // will be called.
    Particle.function("led", ledToggle);
}

void loop()
{
}
```
#### Blink an External LED

Here are the LEDs that I found in the Edge AI kit (and the photo transistor, which is the clear piece with a flat top):

### Speculations
