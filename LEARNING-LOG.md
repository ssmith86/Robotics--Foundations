# Robotics Foundations Learning Log

This log documents my progression from foundational robotics concepts toward
biomedical and assistive robotics projects.

## Table of Contents

[Session 1: Sense-Decide-Act](#session-1-sense-decide-act) <br>
[Session 2: Feedback](#session-2-feedback) <br>
[Session 3: Sensor Transduction](#session-3-sensor-transduction)<br>
[Session 4: Analog and Digital Signals](#session-4-analog-and-digital-signals)<br>
[Session 5: Analog-to-Digital Conversion](#session-5-analog-to-digital-conversion)<br>

---## Session 5: Analog-to-Digital Conversion

**Date:** September 22, 2026

An analog-to-digital converter, or ADC, measures an analog voltage and
represents it with a digital number. Sampling measures the signal at a
particular moment, while quantization assigns that measurement to one of
the ADC's available levels.

In artificial skin, an ADC can convert a pressure sensor's analog voltage
into a number the controller can use. Greater resolution provides more
levels and preserves finer differences in pressure.

**Key takeaway:** An ADC connects continuously changing sensor signals to
a digital controller, but its resolution limits how much measurement
detail is preserved.



---
## Session 4: Analog and Digital Signals

**Date:** September 10, 2026

An analog signal can vary continuously across a range, making it useful when a
controller needs to know how much of a physical quantity is present. A simple
digital signal represents distinct states, such as pressed or not pressed.

A third thumb could use an analog foot-pressure signal to control how far it
bends and a digital emergency button to command an immediate release.

**Key takeaway:** The information a robot needs determines the appropriate
signal type: analog signals represent amounts, while simple digital signals
distinguish between separate states.

---
## Session 3: Sensor Transduction

**Date:** September 9, 2026

Transduction is the conversion of one physical form into another. A sensor
converts a physical quantity, such as force, into a signal that represents the
measurement and can be received by a controller.

In a pressure-sensitive robotic fingertip, applied force might be represented
by a changing voltage. The voltage is not the force itself; it carries
information about the force.

**Key takeaway:** Sensors connect an electronic controller to the physical world
by converting measurable properties into usable signals.

---

## Session 2: Feedback

**Date:** September 2, 2026

Feedback is information about a system's actual result that returns to its
controller. Open-loop control issues commands without measuring the result,
while closed-loop control uses feedback to detect changes and make corrections.

In a robotic hand, a fingertip pressure sensor can report the actual grip
pressure so the controller can continue closing, stop, or release slightly.
In a dog robot, an angle sensor can help the controller correct the head after
it is pushed away from its desired direction.

**Key takeaway:** Feedback allows a robot to check what actually happened
instead of assuming that its command produced the intended result.

---

## Session 1: Sense-Decide-Act

**Date:** September 1, 2026

### Concept

A basic robotic system receives information, processes it according to a rule,
and produces a physical action:

```text
Sense → Decide → Act
