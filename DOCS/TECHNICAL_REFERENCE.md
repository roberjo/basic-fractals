# Technical Reference

## Program Structure

### Memory Layout

```
$0800-$0FFF: Program Code
$1000-$1FFF: Variables and Arrays
$2000-$3FFF: Graphics Buffer 1
$4000-$5FFF: Graphics Buffer 2
$6000-$7FFF: Color Buffer
$8000-$BFFF: Free Memory
```

### Key Variables

```basic
C%(280,192): Color buffer array
P%(280,192): Pixel buffer array
L%(16): Lookup table for iterations
K$(10): Keyboard buffer
```

## Graphics Implementation

### Screen Modes

- High-Resolution Graphics Mode 2 (HGR2)
- 280×192 pixel resolution
- 6-color palette

### Color Mapping

```basic
COLOR 0: Black
COLOR 1: Green
COLOR 2: Violet
COLOR 3: White
COLOR 4: Black
COLOR 5: Orange
COLOR 6: Blue
```

## Mathematical Implementation

### Mandelbrot Set Algorithm

```basic
Z(n+1) = Z(n)² + C
where:
Z = complex number
C = constant
```

### Optimization Techniques

1. Fixed-point arithmetic
2. Early escape testing
3. Symmetry exploitation
4. Lookup tables for common values

## Performance Considerations

### Memory Usage

- Program: 16K
- Graphics: 54K
- Variables: 8K
- Free: 2K

### Speed Optimization

1. Use integer math where possible
2. Minimize floating-point operations
3. Precompute common values
4. Use FOR-NEXT instead of WHILE-WEND where appropriate

## File Formats

### Configuration Files

```
Line 1: XMIN,XMAX
Line 2: YMIN,YMAX
Line 3: MAXITER
Line 4: ESCAPE
Line 5: COLORSCHEME
```

### Saved Images

- Binary format
- 280×192 resolution
- 6-color palette
- ~54K per image

## Error Handling

### Common Error Codes

```
1: OUT OF MEMORY
2: FILE NOT FOUND
3: INVALID PARAMETER
4: DISK ERROR
5: GRAPHICS ERROR
```

### Recovery Procedures

1. Clear memory with NEW
2. Reset video mode
3. Check disk status
4. Verify parameters

## System Calls

### Apple IIe Specific

```basic
CALL -1998: Clear screen
HGR2: Enter high-res mode
HCOLOR=: Set color
HPLOT: Plot point
```

## Development Notes

### Code Organization

1. Main program structure
2. Fractal calculation routines
3. Graphics handling
4. User interface
5. File operations

### Testing Procedures

1. Memory usage verification
2. Graphics mode testing
3. Calculation accuracy
4. User input handling
5. File operations

## Limitations

### Hardware Constraints

1. 64K RAM limit
2. 1MHz processor speed
3. 6-color palette
4. 280×192 resolution

### Software Constraints

1. Applesoft BASIC limitations
2. Floating-point precision
3. File system capacity
4. Memory fragmentation

## Future Enhancements

### Planned Features

1. Additional fractal types
2. Enhanced color schemes
3. Improved file handling
4. Memory optimization
5. User interface improvements 