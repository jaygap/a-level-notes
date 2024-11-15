# Chapter 5 - Fundamentals of Data Representation

## Number Systems

- $\mathbb{N}$ is the set of all natural numbers (non-negative integers).
- $\mathbb{Z}$ is the set of all integers
- $\mathbb{R}$ is the set of all real numbers (rational and irrational)
- $\mathbb{Q}$ is the set of all rational numbers (numbers that can be represented as fractions)
- $\mathbb{P}$ is the set of all irrational numbers (like $\pi$, $e$)

## Number Bases

- A number base is how many unique symbols are used to represent numbers.
- Hex is often used because it is easier for humans to read but it still clearly represents the bits that are being stored.

## Data Storage

| Prefix | Symbol | Size |
| :-: | :-: | :-: |
| kilobyte | kB | $10^3$ bytes |
| megabyte | MB | $10^6$ bytes |
| gigabyte | MB | $10^9$ bytes |
| terabyte | TB | $10^{12}$ bytes |
| kibibyte | KiB | $2^{10}$ bytes |
| mebibyte | MiB | $2^{20}$ bytes |
| gibibyte | GiB | $2^{30}$ bytes |
| tebibyte | TiB | $2^{40}$ bytes |

- $n$ bits can represent $2^n$ numbers

## Binary Number System

- An unsigned number can only be positive while a signed number can be positive or negative
- Two's complement is a way of storing representing negative numbers in binary by making the most significant bit negative.
- To convert a positive number to a negative number ($+5$ to $-5$) you simply flip all the bits to the left of the least significant 1 ($00000101$ becomes $11111101$)
- Expressing fractional numbers is done with decreasing powers of 2 ($2^{-1}$, $2^{-2}$, $2^{-3}$ etc.)
	- This can lead to representational errors as some numbers cannot be represented as a sum of powers of 2 (like 0.3)
	- The absolute error is the difference between the actual value and the approximate value
	- A relative error is the absolute error divided by the actual value.
- Increasing the number of bits of the mantissa increases the precision of the number stored
- Increasing the number of bits of the exponent increases the range of the number stored
- Overflow occurs when the result of a calculation is too large
- Underflow occurs when the result of a calculation is too small

## Error Checking

- **Parity bits**
	- A bit is added onto the end of the data so that there is an even or odd number of $1$s depending on the type of parity used.
- **Majority voting**
	- Each bit in the data is replicated an odd number of times so that each block that used to represent one bit can "vote" on whether the bit should be a 0 or 1.
	- This vastly increases the number of bits transmitted.
- **Checksum**
	- A piece of data is added to the block of data that is being transmitted, this piece of data was calculated by passing the block of data through a function
	- When the data is received, passing the block through the same function should return the piece of data that was originally added.
- **Check digit**
	- Extra digit added to the beginning or end
	- Main purpose is to recognise and prevent human errors

## Representing Images

- Bitmaps store individual pixels
- Vectors store information about the shapes in the picture
- Bitmaps can store more complex images
- Vectors can be scaled without losing details
- Vectors can only be effectively used for logos or shapes

## Representing Sound

- Analogue sounds need to be converted to digital information by an ADC before they can be stored.
- A DAC is used to convert the digital information into analogue waves.
- Nyquist theorem states that the sampling rate of a recording needs to be at least twice that of the highest frequency to ensure the sound is accurately represented.
- Sampling rate is the number of samples taken each second
- Sample resolution is the number of bits used to store each sample
- A mono track is a single track while a stereo track is two mono tracks, one for each ear.
- MIDI files store instructions for how to play sounds, not the actual sounds themselves.

## Compression & Encryption

- Files are compressed so they take up less space
- Lossy compression results in the loss of data, lossless compression does not
- RLE and dictionary-encoding are examples of lossless compression
- Encryption is the process of turning plain-text to cipher-text
	- This is done so that the data cannot be understood if intercepted while being transmitted
- In a Vernam cipher, each character has its own key and so it is considered a "perfect" form of encryption if the string it is encrypting and the key used to encrypt it is of the same length.

# Chapter 6 - Fundamentals of Computer Systems

## Software Categories

### Application Software

- Software that is used to help the user complete a task the user wants to complete
	- Word processors
	- Spreadsheet software
	- Image editing software
- Application software can be split into 3 categories:
	- General purpose software can be used to complete a variety of tasks
	- Special purpose software can only be used for a particular task
	- Bespoke software is designed to meet a client's specific needs

### System Software

- Software that controls the hardware of the computer
	- Operating system
		- Provides a platform for other software to run on
		- Manage resources such as memory and compute time
	- Utility software
		- Ensures the computer is running efficiently
			- Disk-defragmentation software
			- Anti-malware software
			- File managers
	- Libraries
		- Collections of prewritten instructions that can be repurposed to be used in other programs
	- Translators

## Programming Languages

- **Low-level languages**
	- Machine code + assembly
	- Have a one-to-one relationship with processor instructions
	- Processor architecture specific
	- Allows for individual control of registers
	- Typically require less memory and execute faster than high-level languages
	- Allow for the creation of highly optimised programs
	- More difficult to learn
	- Used in embedded systems and device drivers
- **High-level languages**
	- Must be translated to machine code before they are run
	- Easier for humans to understand when compared to low-level languages
	- Single line of code can represent multiple processor instructions
	- Portable (not processor specific)
	- Come with libraries of pre-written code

## Translators

- **Compilers**
	- Translates the whole code into a different language that is executable by the computer. This allows for the distribution of the executable.
- **Interpreters**
	- Translates the code line by line and halts if it finds an error
- **Assemblers**
	- Translates assembly into machine code directly as they have a one-to-one relationship

## Boolean Algebra

- **Associative Law**
	- $X \cdot (Y \cdot Z) = (X \cdot Y) \cdot Z$
	- $X + (Y + Z) = (X + Y) + Z$
- **Absorption Law**
	- $X + (X \cdot Y) = X$
	- $X \cdot (X + Y) = X$
- **Distributive Law**
	- $X \cdot (Y + Z) = (X \cdot Y) + (X \cdot Z)$
	- $X + (Y \cdot Z) = (X + Y) \cdot (X + Z)$
- **De Morgan's Law**
	- $X \cdot Y= \overline{\overline{X} + \overline{Y}}$
	- $X + Y= \overline{\overline{X} \cdot \overline{Y}}$

## Common Circuits

- **Half-adder**
	- Adds 2 binary digits and outputs the sum and carry

![[Half_Adder.jpg]]

- **Full-adder**
	- Adds 3 binary digits and outputs the sum and carry
	- Putting many of these together allows you to multi-bit binary adders

![[fullAdder-1-1024x473.png]]

- **Edge Triggered D-type flip-flop**
	- Used to store a single binary digit
	- Only changes when given given a high bit from the clock signal

![[d-flip-flop2.png]]

# Chapter 7 - Fundamentals of Computer Organisation and Architecture

## Internal Components of a Computer

- Processor
- Main Memory
	- RAM is involved in the fetch-execute cycle
	- ROM is involved in the boot process
- Input/Output Controllers
	- Provide the ability to take inputs from external devices
	- Provide the ability to output to external devices
	- Interface between a computer and its peripherals
	- Provide a set of addressable registers that the CPU can access to communicate with I/O devices
	- Physical ports provide a connection to the peripheral
	- A device driver is software that provides a software interface for the peripheral device
- Buses
	- The components of a computer system are connected by buses
	- System bus
		- A set of parallel connections that allow internal components to communicate with each other
	- Data bus
		- Transfers data and instructions and is bidirectional
	- Address bus
		- Specifies the memory address to read/write to
	- Control bus
		- Sends control signals that manage and orchestrate operations

## Computer Architecture

- **Von Neumann**
	- Instructions and data are stored together
	- Consists of:
		- Processor
		- Main memory
		- Secondary Storage
		- Connections for I/O
- **Harvard**
	- Instructions and data are stored separately
		- The instruction memory and data memory have their own data and address buses

### Stored Program Concept

- Machine code instructions stored in main memory are fetched and executed serially by the processor

## Processor

- Arithmetic and Logic Unit (ALU)
	- Responsible for arithmetic and logic operations
- Control Unit
	- Organises the sequence in which instructions are executed and decodes instructions
- Clock
	- Sends signals at regular intervals to synchronise the operations of the CPU
- Registers
	- General-purpose registers are temporary stores of data
	- Program Counter (PC)
		- Holds the address of the next instruction to be executed
	- Memory Address Register (MAR)
		- Holds the address of the memory that needs to be accessed
	- Memory Buffer Register (MBR)
		- Holds the data that was read from memory or is going to be written into memory
	- Current Instruction Register (CIR)
		- Holds the address of the current instruction being executed
	- Status Register (SR)
		- Stores information about the result of the last instruction the ALU executed

### Fetch-Execute Cycle

1. PC copied to MAR
2. PC incremented by 1, data at address in MAR is copied to MBR
3. Instruction is copied to CIR
4. Decoded by the control unit
5. Executed

### Interrupts

- A signal sent to the processor that requires immediate attention
- The CPU checks for interrupts between fetch-execute cycles
- Interrupt Service Routines (ISRs) are designed to process interrupts
- If interrupts are found the instruction then the instruction in the PC is added to a stack and any interrupts are also added to the stack. Then the instruction at the top of the stack is completed until the stack is empty

### Factors Affecting CPU Performance

- Number of cores
- Cache size
- Clock speed
- Word length/size
	- The amount of data that can be handled by the processor at once
- Data bus width
	- The number of bits that can be transferred in one operation
- Address bus width
	- The number of bits that can be used to specify an address

## Input & Output Devices

- Barcode
	- Black and white lines reflect different amounts of light so 0s and 1s can be encoded
	- Usually include a check digit
- Barcode reader
	- Light is shone at the barcode
	- More light is reflected by the light parts than the dark ones which is captured by photoelectric cells that generate a set of electric pulses
	- These pulses are then converted into binary
- RFID
	- Passive RFID use the energy in the radio waves they receive to power the chip (very short range, <1m)
	- Active RFID have a battery to power them and have much longer range
	- Used in employee/student ID cards
	- Can be read-only or read-write
- Inkjet printers
	- Use liquid ink to produce images
	- Better colours than laser printers
- Laser printers
	- Use powdered ink 
	- Faster than inkjet printers
	- Laser shines on a rotating drum, charging the powdered ink causing it to stick to the paper and then passed through a fuser that fuses the ink and paper together (which is why the paper is warm once finished)

## Secondary Storage

- Magnetic Hard Disk
	- Read/write head polarises platters on the disks so that they correspond to binary numbers
- Solid State Drive (SSD)
	- Made of NAND flash memory cells
	- Data is read by page and can also be written by page
	- To update data, it has to be written to a different location
	- Become slower as they fill up
- Optical Storage
	- Discs spin very quickly
	- Light is shone on them and a sensor detects changes in light as pits and lands reflect different amounts of light
	- To write, the laser is used at a higher intensity that burns tiny dots into a chemical layer which reflects a different amount of light. This is reversible

# Chapter 8 - Consequences of Computing

## Legislation

- **Copyright, Designs and Patents Act 1988**
- **Computer Misuse Act 1990** - introduced legal provisions in UK law governing the use and misuse of computer systems
- **Regulation of Investigatory Powers Act 2000** - regulates electronic surveillance by public bodies
- **General Data Protection Regulation (GDPR)** - ensures data protection and privacy for all EU citizens
- **Data Protection Act 2018**

- **Surveillance**
	- 
- **Big Data**
- **Storage of personal data**
- **Personalised algorithms**
- **Artificial Intelligence**
	- Generative AI is often used to 

# Chapter 9 - Fundamentals of Networking

# Chapter 10 - Fundamentals of Databases

# Chapter 11 - Big Data

# Chapter 12 - Functional Programming