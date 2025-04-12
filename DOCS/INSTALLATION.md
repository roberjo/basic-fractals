# Installation and Setup Guide

## Prerequisites

Before installing the Fractal Generator, ensure you have:
- Apple IIe computer with 64K RAM
- Working 5.25" floppy disk drive
- High-resolution graphics capability
- Applesoft BASIC in ROM or on disk

## Installation Steps

### 1. Prepare the Disk

1. Format a blank 5.25" floppy disk
2. Label the disk "FRACTAL GENERATOR"

### 2. Copy Program Files

1. Insert the source disk containing the program
2. Copy the following files to your formatted disk:
   - `FRACTAL.BAS` (main program)
   - Any additional support files

### 3. Verify Installation

1. Insert the disk into your Apple IIe
2. Boot the system
3. Type `CATALOG` to verify files are present
4. Type `LOAD FRACTAL.BAS` to load the program
5. Type `RUN` to start the program

## Memory Management

The program requires careful memory management due to the Apple IIe's limited RAM:

- Program size: ~16K
- Graphics buffer: ~54K
- Variables and arrays: ~8K
- Free memory: ~2K

### Memory Optimization Tips

1. Clear memory before loading:
   ```
   NEW
   ```
2. Remove unnecessary programs from memory
3. Use `CLEAR` command to reset variables
4. Consider using a RAM expansion card if available

## Troubleshooting Installation

### Common Issues

1. **"OUT OF MEMORY" Error**
   - Clear memory with `NEW`
   - Remove other programs
   - Check for memory expansion

2. **"FILE NOT FOUND" Error**
   - Verify disk is inserted
   - Check file name spelling
   - Ensure disk is properly formatted

3. **Graphics Issues**
   - Verify high-resolution graphics capability
   - Check monitor connection
   - Ensure proper video mode

## Advanced Setup

### Custom Configuration

You can modify the following parameters in the program:
- Screen dimensions
- Default iteration count
- Color schemes
- Memory allocation

### Disk Space Requirements

- Program file: ~16K
- Saved configurations: ~1K each
- Documentation: ~8K

## Support

For additional installation help:
1. Refer to the troubleshooting guide
2. Check the technical reference
3. Contact support through the program's help menu 