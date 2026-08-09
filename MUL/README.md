# 4:1 Multiplexer using Verilog

## Description

A **4:1 Multiplexer (MUX)** selects one of four input signals and forwards it to a single output based on two select lines.

### Inputs

- I0
- I1
- I2
- I3
- S1
- S0

### Output

- Y

## Truth Table

| S1 | S0 | Output |
|----|----|--------|
| 0 | 0 | I0 |
| 0 | 1 | I1 |
| 1 | 0 | I2 |
| 1 | 1 | I3 |

## Files

- multiplexer.v
- multiplexer_tb.v
- README.md

## Compile

```bash
iverilog -o mux multiplexer.v multiplexer_tb.v
```

## Run

```bash
vvp mux
```

## Expected Output

```
-----------------------------------------------
 I0 I1 I2 I3 | S1 S0 | Y
-----------------------------------------------
 0  1  0  1 | 0  0 | 0
 0  1  0  1 | 0  1 | 1
 0  1  0  1 | 1  0 | 0
 0  1  0  1 | 1  1 | 1
```

## Author

Nikhila Ummadisetty