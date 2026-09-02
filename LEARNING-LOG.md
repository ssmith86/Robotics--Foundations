# Robotics Foundations Learning Log

This log documents my progression from foundational robotics concepts toward
biomedical and assistive robotics projects.

## Table of Contents

[Session 1: Sense-Decide-Act](#session-1-sense-decide-act) <br>
[Session 2: Feedback](#session-2-feedback) <br>

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

## Session 1: Sense-Decide-Act

**Date:** September 1, 2026

### Concept

A basic robotic system receives information, processes it according to a rule,
and produces a physical action:

```text
Sense → Decide → Act
