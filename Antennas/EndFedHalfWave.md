# End-Fed Half Wave Experiments

The first transmitting antenna I made for HF was an end-fed half wave for 40m
which consisted of a ~66' piece of wire made from some CAT5 cable pairs spliced
together, and a small 49:1 unun in a plastic food container.

## Basic Concept

The concept of an end-fed half-wave (EFHW) is easy to understand if you imagine
the antenna as a normal dipole with two quarter-wave section attached together.
In a regular dipole the feed point is at the centre with 1/4 wave radiator connected
to each half of the feed-line. This usually presents a low impedance (around 73
ohms) that can be fed directly with coax. Most often these antennas are made from
wire when used on the HF bands as they are light and can be easily supported by
insulated ropes or poles.

However this type of antenna has several drawbacks:

- It must be fed from the centre
- It must be supported in three places
- The centre of the antenna is usually the highest point in the setup (inverted-V configuration)
- Operation on multiple bands is limited since both sides of the dipole must resonate on any desired harmonic

It is often more convenient to feed an antenna from the end instead of the
middle. This could enable use of less coax from the radio, as well as allowing
the wire to be supported by only two points. Another big advantage is the ability
to use the antenna on various harmonics of the base frequency since the single wire
can resonate on any integer multiple of the base frequency.

By using a wire length of 1/2 wave the antenna still acts
mostly like a dipole, which means that the currents are balanced on both
halves of the wire with low voltage / high current in the centre, and
high-voltage / low current at the ends. Unlike a 1/4 wave ground-plane antenna
the EFHW requires little to no counterpoise / ground plane making it excellent
for portable use or installations where having ground radial wires would be impractical.

To feed an end-fed half wave antenna requires an impedance conversion since the end
of a half-wave wire presents a high-impedance. The standard method involves either
a 49:1 or 64:1 transformer to match a typically 50 ohm feed-line to several thousand
ohms. For the HF bands the most common type of impedance conversion is done with
an unun modelled as either a transformer with a common ground terminal, or an
auto-transformer.

## Experiments / First Version

It actually took a number of tries to make an unun that measured acceptably
on the bench. I tried various toroid cores that I had on hand including type 2
and type 75 types. I was not able to get any acceptable performance from them.
The type 2 (T106-2) basically didn't work at all for some reason. The type 75
material basically get a very high SWR across all HF bands with a 3.3K load on
the output. In all cases I was using a unun winding with 3 primary turns and
21 secondary turns. (there are many images online showing how to wind this)

Finally I ordered some type 43 toroids which ended up working very well from
2-10MHz, and also worked up to 30MHz after the recommended compensation capacitor
was added across the feedline. Once again it was wound with a 3/21 turn arrangement.

The first version was made to be portable:

<img src="images/2022-01-28-good_unun.jpg" width="400"/>

<img src="images/2022-01-28-portable_hf_station.jpg" width="400"/>

This actually allowed me to make a contact from a park during January 2022.
(it was -14C!) I used about 20W and ran my FT-450D off a 12V SLA battery for
about 10 minutes until my hands were freezing.

<img src="images/2022-01-29-field_day2.jpg" width="400"/>

I took the same setup out again in the spring with a friend but could not get
the antenna to tune up at all. I believe there was a loose connection in the
unun. I scrapped it and decided to make something better.

## Second Version

In preparation for my home station I built a more rugged 49:1 unun in a
weatherproof electrical box with the proper high-voltage compensation
capacitor across the feedline, and studs for permanent attachment of the
cables. I also used a high-quality SO-239 connector.

In this version the winding was changed to 2 turns primary / 14 turns secondary.
I had come across some information showing that fewer turns can improve the
performance as long as the permeability is high enough in the core material.
(probably due to less inter-winding capacitance, but I haven't confirmed this)

This version tested out great on the bench with a 2.7K load resistor but has so
far not been installed or used. It was intended for my home station but that design
changed to use a vertical antenna instead.

<img src="images/2022-06-23-efhw_unun1.jpg" width="400"/>

<img src="images/2022-06-23-efhw_unun2.jpg" width="400"/>

<img src="images/2022-06-23-efhw_unun3.jpg" width="400"/>
