# VHDL Counter Overflow Bug

This repository demonstrates a common error in VHDL:  overflow in a counter. The provided VHDL code implements a simple 4-bit counter. However, it lacks proper overflow handling, leading to unexpected behavior when the counter reaches its maximum value (15). 

The `bug.vhdl` file contains the erroneous code, while `bugSolution.vhdl` provides a corrected version.

## Bug Description
The original counter increments indefinitely, resulting in an overflow when it exceeds the maximum value. This can lead to incorrect behavior in the system using this counter.

## Solution
The solution implements saturation or modulo arithmetic to handle the overflow condition.  When the counter reaches its maximum value, it either saturates (remains at the maximum value) or wraps around to zero. 

This example demonstrates the importance of carefully considering the potential for overflow when designing counters in VHDL.