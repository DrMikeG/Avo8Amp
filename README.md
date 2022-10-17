# Avo8Amp


Universal avometer model 8 mk 5 faulty not working for parts only

http://www.richardsradios.co.uk/avo8.html


Can measure volts without battery.

2.2 volts peak-to-peak

https://www.petervis.com/avo-meters/avo-8-mk-5/avo-8-mk-5.html

https://www.vintage-radio.net/forum/showthread.php?t=144169

full scale deflection (F.S.D.) 

"The two crucial characteristics of a given galvanometer are its resistance and current sensitivity. Current sensitivity is the current that gives a full-scale deflection of the galvanometer’s needle, the maximum current that the instrument can measure. For example, a galvanometer with a current sensitivity of 50 μA has a maximum deflection of its needle when 50 μA flows through it, reads half-scale when 25 μA flows through it, and so on. If such a galvanometer has a 25-Ω resistance, then a voltage of only V = IR = (50 μA)(25 Ω) = 1.25 mV produces a full-scale reading. By connecting resistors to this galvanometer in different ways, you can use it as either a voltmeter or ammeter that can measure a broad range of voltages or currents."

Figure 4 shows how a galvanometer can be used as a voltmeter by connecting it in series with a large resistance, R. The value of the resistance R is determined by the maximum voltage to be measured. Suppose you want 10 V to produce a full-scale deflection of a voltmeter containing a 25-Ω galvanometer with a 50-μA sensitivity. Then 10 V applied to the meter must produce a current of 50 μA. The total resistance must be

By 1930 the meter looked little different to the way it looked in 2008
It had a meter sensitivity of 6mA FSD which is useless for testing HT circuits in valve equipment

By the late 1940’s the AVO7 was insensitive compared to the competition

The AVO8 was introduced to the civilian market in 1951 
The extra sensitivity was provided by a new meter movement with 37.5uA FSD

20,000 Ohms per Volt sensitivity
A mechanical cut out acting directly on the meter

37.5 Microamperes = 3.75E-5 Amperes
100 μA	= 0.0001 A
37.5μA  = 0.0000375 A

3333ohms

V = I R
V = 0.0000375 * 3333
0.125V 1/8V

We know that 10V DC must cause a current of 37.5 Microamp to flow through the meter for FSD, so we need to calculate what resistance will cause a current of 37.5 Microamp to flow when 10v is applied.

Using ohm's law V = I x R
re-arranged R = V / I = 10 / 0.0000375 = 266666 ohms or 266k

47.5k + 197.5k = 245k (21k)


BUT we have not considered the coil's resistance = 100R, and this would cause errors in reading. If we used the 10k we would have a total series resistance is 10,100R and therefore the calculation which gives
I = V / R = 10 / 10,100 = 0.99mA through the meter and do not achieve the 1mA FSD - there is a 1% error.
The solution is to subtract 100 ohms from 10k - thus 10,000 - 100 = 9900 ohms.
This 9900 ohms resistor is the "Multiplier".

staggering 50uA fsd sensitivity - 37.5uA for the movement and 12.5 uA for the permashunt.





These ranges are calibrated for correct full scale deflection (F.S.D.) by using ... Our meter sensitivity is 1000 ohms per volt, pretty poor, when a good "AVO" is ...

https://brats-qth.org/training/advanced/measure0.htm

With the meter terminals shorted as shown the current will be 1mA, giving us a FSD (Full Scale Deflection, which indicates zero ohms and the scale would be marked as such.

Meters 101

Notice the dials on the front of each meter these are used to select the range of the display. For the analogue meter this is particularly important so that the meter needle is not driven hard against the end stop due to the measured voltage being higher than the range.

The dial on the meter is a multi position switch used to select from a range of voltages or current. 
These ranges are calibrated for correct full scale deflection (F.S.D.) by using multiplier resistors for measuring voltages and shunt resistors for measuring currents.

A 10V FSD VOLT METER

Let's look at a typical example of an analogue multimeter. 
If we have a basic meter movement which has I FSD = 1 milliamp and R coil = 100 ohms. So what voltage applied to the meter gives the FSD.

From V = I x R V = 0.001 x 100 = 0.1 volts.

Maximum output voltage drive	150mV (0.15v)


"The Avometer cut-out mechanism sometimes does not lock into place, and when you push the cut-out knob, it does not stay in. In this article, we look at some of the basic simple things you can so to repair it.

Firstly, people often do not realise, that it only works when the meter is lying on its back, which is the proper way to use the meter. Usually the cut-out knob will not lock in if the meter is upright."



## 2021.06.16 ##

I just received these short blue LED strips. They have a 9volt battery connector.
They are actually marked as 12V
DC12V-2835
60D 20R 8mm

Using my multimeter in series I measured the current draw for one strip of 6 LEDS as 11.75mA

## 2021.07/06 ##

https://www.giangrandi.org/electronics/vu-meter/vu-meter.shtml


"The audio volume is often expressed using a logarithmic scale because the feeling of sound intensity we get from our ears is also logarithmic and a direct power reading in Watts would not be very representative of the perceived volume.

For example
- a few millivolts on an 8 Ω speaker are clearly audible. 
- when listening at low volume, the voltage on the speakers is only a few hundreds millivolts (these are only milliwatts). 
- when the volume is raised to a medium setting, the voltage on the speaker is around few volts (the power is around a Watt) 
- only when the volume is very high that all the watts of the amplifier are required.

There is a way to build a simple and passive logarithmic VU-meter with only a few parts.


The circuit is shown below and is really very simple. It's based on a standard 200 μA microammeter which is very very common for this kind of applications. Its internal resistance is not critical at all and is usually between 500 Ω and 1 kΩ. The circuit is intended to fit an amplifier capable of 80 WRMS driving a 8 Ω load, but can easily be adapted to other power levels or impedances. Similar power levels requires no modification, for much higher or lower levels, R4 must be modified and maybe also R2 and R3.

200 microamps (μ) = 0.2 milliamps (m)


![Alt text](/img/vu-meter-circuit.gif)

First the AC signal across the speaker is rectified by diode D1.

D1 should be a germanium diode or a Shottky diode to minimize the voltage drop across it. Every millivolt lost here will reduce the sensitivity at low volume. But D1 has to stand twice the peak voltage of the speaker, so the reverse voltage of the diode has to be selected accordingly. 

For example, 80 W over 8 Ω have a voltage of √ 80 W · 8 Ω  = 25.3 VRMS and a peak voltage of √ 2  · 25.3 V = 35.8 Vpeak, so the diode will get 2 · 35.8 V = 71.6 V on its leads.
```
1W through an 8Ω load must be 2.83V. (sqrt(1*8))
sqrt(2) * 2.83 = 4 Vpeak 
so the diode will get 8V on its leads.
```
Germanium diodes have a low voltage drop, about 0.25-0.3 V, but the majority of them have breakdown voltages between 30 and 40 V! Small signal Schottky diodes can have voltage drops in the 0.2-0.4 V range depending on the model and can easily deal with reverse voltages up to 100 V. Don't use high current Schottky diodes or silicon diodes because their voltage drop is in the 0.5-0.7 V range and is too high for this application.

10 x 1N5817 1A 20V Schottky Rectifier Diode 
(no resistor 0.01a)
5 x BAT85 Schottky Small Signal Diode Rectifier (no resistor 0.01)
10x BAT43 Small Signal Schottky Diode (no resistor)

C1 4u7 63v

Resistor R1 is a very good idea because it increases the impedance of the meter and limits the (non-linear) current drawn by this circuits so that it can be neglected compared to the main speaker current. Otherwise, connecting a rectifier in parallel with a speaker could introduce some distortion.

The 10 kΩ of R1 are high enough compared to the 8 Ω of the speaker to make sure that the total harmonic distortion won't be affected. R1 will also limit the current in D1 if the maximum diode reverse voltage is exceeded, preventing damages in case of small peaks.

Capacitor C1 integrates the rectified signal and provides only DC to the meter. The time constant is below 50 ms, low enough not to slow down the meter that has usually a time constant in the 300 ms range.

Now the tricky part: for low voltages, D2, D3 and D4 do not conduct. These are regular small signal silicon diodes with a forward drop of 0.6 V; here a high voltage drop is important. So for low voltages D2, D3, D4, R2 and R3 can be neglected and the current can flow directly in the meter. This can be observed in the graph below (the one on the left): for input voltages below 0.6 V, the current in the meter (blue trace) is linear and D2 (green trace) and D3-D4 (yellow trace) conduct no current. As soon as the voltage rises, D2 starts conducting and robs current to the meter making it less sensitive to higher voltages. On the same graph, above 0.6 V the current in D2 (green trace) starts rising and the current in the meter (blue trace) rises with a lower slope. For even higher voltages (about 10 V, graph on the right), D3 and D4 will start conducting as well robbing even more current (yellow trace). The effect is that the meter current slope (blue trace) is further reduced approximating a nice logarithmic function. To calculate this circuit (especially the values of R2 and R3), the common approximation of the 0.6 V threshold voltage is not enough. One has to use the diode characteristic exponential function, but equations get complicated and I wasn't able to solve it with just a pencil and a piece of paper. Fortunately, free SPICE software is available and the circuit can easily be simulated and a reasonable solution can be found by modifying the values of these to resistors until a suitable response is achieved.

Trimmer R4 is used to set the full scale of the meter. The easiest way to adjust it is, before connecting this circuit to your stereo set, to turn it for the maximum possible resistance, than temporarily connect a DC source to the input corresponding to the maximum peak voltage (35.8 V in this case) and turn it in the other direction to align the needle with the full scale reading. Because of the logarithmic characteristic of this circuit, the correct adjustment of R4 is not critical at all.

Another way to adjust R4 is to install the circuit at the output of the amplifier as usual, apply a test signal to the input, turn the volume for the maximum power and adjust the trimmer for the full scale. The problem with this second method is that the speaker must be connected while doing the adjustment and it's a very loud operation. Of course, you could replace the speaker with a suitable dummy load, if you have one.

In this way, the meter will read the output power of the amplifier and not real VU units, and I think this is the most useful reading. If you prefer real VU units or dBm units, you can still apply the same procedure and adjust for a given power and aim a given mark on the meter instead of the full scale. If not adjusting for full scale at full power, verify that the needle won't hit the full scale end at full power; otherwise the meter could be damaged.

Please remark that the type of rectifier used in this circuit requires a DC path in the source side. This is usually not a problem: tube amplifiers have transformer output that conducts DC, push-pull amplifier with dual power supply are DC coupled as well. Single supply transistor amplifiers, on the other hand, have a capacitor coupled output and a DC path does not exist in the amplifier. But a DC path always exists in the speaker and as long as the speaker is connected the VU-meter will work fine. Don't worry about this DC current, because of the high value R1, its value is only 0.08 % of the main speaker current and can be neglected.

One of the big advantages of this simple circuit is that it's completely passive and requires no power supply. This means it can be connected directly in parallel with the amplifier output (or the speaker) without warring about the amplifier output configuration. No matter if it's a push-pull, a single-ended, an H-bridge, a transformer output or whatsoever. There is no risk of shorting to ground half of the output transistors or shorting together the left and right channel: just connect it fully floating in parallel of the output.

## Honeytone pots ##
19mm square variety
type A are logarithmic
type B are linear. 

A50k for volume (in addition to an on/off switch, modification 6 .), 
B100k (type B 100,000 ohm) 
A50k POT for overdrive.


## Mode tinkering with the circuit ##

Measuring the output from the speaker, I get about 1V AC.
The forward voltage drop of the initial signal diode is 0.2V
With the capacitor and the diode, I can read a DC voltage of about 0.5V.

With the full circuit in place, using a 1k initial resistor, on 0.3 milliamp (300 microamp scale) I get a good swing.

The meter itself is 37.5 microamps (0.0375 milli amps)


The voltage divider looks to work by increasing the resistance of the path to ground as the input current increases.
For 10A - the path to ground is only 0.05 ohms.
For 1A - the path to ground is 0.05 + 0.45 ohms
For 100mA - the path to ground is 0.05 + 0.45 + 4.5 ohms
For 10mA - the path to ground is 0.05 + 0.45 + 4.5 + 42 ohms
For 1mA - the path to ground is 0.05 + 0.45 + 4.5 + 42 + 450 ohms
For 300uA - the path to ground is 0.05 + 0.45 + 4.5 + 42 + 450 + 300 + 1.2k ohms
For 50uA - the path to ground is 0.05 + 0.45 + 4.5 + 42 + 450 + 300 + 1.2k + 8k ohms

| Amp     | Resistors | R1    | V   |
|---------|-----------|-------|-----|
| 10      | 0.05      | 0.05  | 0.5 |
| 1       | 0.45      | 0.5   | 0.5 |
| 0.1     | 4.5       | 5     | 0.5 |
| 0.01    | 45        | 50    | 0.5 |
| 0.001   | 450       | 500   | 0.5 |
| 0.00025 | 1500      | 2000  | 0.5 |
| 0.00005 | 8000      | 10000 | 0.5 |
| 0.00030 |           | 1666  | 0.5 |

If you multiply the max current input by the resistance on the path to ground, there is a constant value of 0.5V.

3333 + 2000 = 5333

(3333/5333) to the meter = 0.625 * 0.00025 = 0.00015625 amp

Regardless of why it works, I think I should need 1666 ohm division to ground to make the meter work, connecting up to points A and B.


# Connecting up my LED strip #

![Alt text](/img/Led_connection.png)

Reasonably easy access to a ~+8V DC supply (post switch) to supply my LED strip, once I have removed the old LED.


Removed jack socket

![Alt text](/img/jack_socket.png)

Tested pins.

![Alt text](/img/jack_socket2.png)

Shortest leg is tip
Middle leg is sleeve


![Alt text](/img/power_connection.png)

On the little jack socket, the tip has round pad, L-shaped leg on the back. The other two are ground

# Conclusion #

This project is approaching its natural end. It's functioning as I planned, with a few predictable idiosyncrasies. I'm sure I will return to it to make improvements or fixes, but for now I've done what I set out to do.

I do still need to 3D print a 9v battery holder, but because the battery leads fit through a small hole in the rear case, leading into the original internal battery compartment, so I didn't start working on this until I've sealed the front panel into the case for what I hope is the last time.

I've really enjoyed this project. I've had a huge number of learning opportunities and it's rumbled on for multiple months, in parallel with the rest of my life and various other projects.

One of the unique points about this project, it that I've been working with vintage hardware - and that has provided some interesting challenges, and no small amount of soul-searching.

At the start of this project, I voiced some doubts about whether chopping up a working AVO meter was ethical, and talked myself into continuing.
An alternative would have been to spend me time instead restoring in an effort to achieve full work order.

Towards the end of the project, I read an interview with Matthew Read, conservator of automata and clocks for the Royal Observatory in Greenwich, the Bowes Museum, and the National Trust. talking about his work in clock repairs.

"The kind of people who get involved with clock repair... many of them are second-generation engineers or something like that. Really highly trained people, inevitably, they see an old thing, and they think they can make it better.

"And I say, 'No, no, no, don't make it better'. [There's] a really simple answer to this, and it's the relationship between craft and new making. If you're powered to do something really well, just make a new thing. It's much more difficult to do that than to muck up somebody else's work."

