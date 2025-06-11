# embedded-systems---mini-project-4-solved
**TO GET THIS SOLUTION VISIT:** [Embedded-Systems – Mini Project 4 Solved](https://mantutor.com/product/embedded-systems-mini-project-4-solved/)


---

**For Custom/Order Solutions:** **Email:** mantutorcodes@gmail.com  

*We deliver quick, professional, and affordable assignment help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114504&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Embedded-Systems - Mini Project 4 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
System Requirements

Implement the following system to measure the distance using ultrasonic sensor HC-SR04 with the specifications listedbelow:

1. Use ATmega16 Microcontroller with frequency 8Mhz.

2. Measure the distance using the Ultrasonic sensor HC-SR04. Check the “HC-SR04 Ultrasonic MT Student Tutorial” pdf file to understand how to interface with this sensor.

3. The LCD should display the distance value like that:

4. The project should be design and implemented based on the layered architecture model as follow:

GPIO Driver Requirements

1. Use the Same GPIO driver implemented in the course.

ICU Driver Requirements

1. Use the Same ICU driver implemented in the course.

2. The ICU should be configured with frequency F_CPU/8 and to detect the raising edge as the first edge.

3. ICU_init and ICU_setCallBack functions should be called inside the Ultrasonic_init function.

LCD Driver Requirements

1. Use 4×16 LCD.

2. Use the Same LCD driver implemented in the course with 8-bits data mode.

3. Connect the LCD control pins and 8-bits data pins as follow:

• RS → PB0

• RW → PB1

• E → PB2

• Data Bus → all PORTA pins.

Ultrasonic Driver Requirements

1. Implement a full ultrasonic Driver using ATmega16 ICU driver.

2. The ultrasonic driver has 3 functions:

a. void Ultrasonic_init(void) • Description

➢ Initialize the ICU driver as required.

➢ Setup the ICU call back function.

➢ Setup the direction for the trigger pin as output pin through the GPIO driver.

• Inputs: None

• Return: None

b. void Ultrasonic_Trigger(void)

• Description

➢ Send the Trigger pulse to the ultrasonic.

• Inputs: None

• Return: None

c. uint16 Ultrasonic_readDistance(void)

• Description

➢ Send the trigger pulse by using Ultrasonic_Trigger function.

➢ Start the measurements by the ICU from this moment.

• Inputs: None

• Return: The measured distance in Centimeter.

d. void Ultrasonic_edgeProcessing(void) • Description

➢ This is the call back function called by the ICU driver.

➢ This is used to calculate the high time (pulse time) generated by the ultrasonic sensor.

• Inputs: None

• Return: None

The Project Hardware Connections
