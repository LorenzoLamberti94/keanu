# Notes

### General
- `ScatterND` is used to assign values to specific positions in a tensor based on indices. It's typically employed in operations like masking or setting certain values at specific indices in a tensor.


### Quantization Results
- Only negligibel differences in performance for different images as input
    - Main layers exactly the same
    - E.g. softmax in the end a bit slower / faster
    - Operations exactly the same, differences only for cycle count

- Performance:
    - NE16 off: 5.28e6 cyc -- 14.3 ms @ 370 MHz -- 33 FPS @ 170 MHz
    - NE16 on:  8.16e5 cyc --  2.2 ms @ 370 MHz -- ?? 450 FPS @ 370 MHz
    - 