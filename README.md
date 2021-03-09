# About BufferOverFlow
```
Buffers are memory storage regions that temporarily hold data while it is being transferred 
from one location to another.
A buffer overflow (or buffer overrun) 
occurs when the volume of data exceeds the storage capacity of the memory buffer. 
As a result, the program attempting
to write the data to the buffer overwrites adjacent memory locations.

```
<br>
<img src="https://raw.githubusercontent.com/walczy/BufferOverFlow/main/1.png"></img>
<br>

With the buffer overflow vulnerability, we can easily inject 💉 malicious code into the memory
of the running program. 

To jump to the malicious code that we have injected into the target stack, we need to know
the absolute address of 
👉 EIP 👈. If we know the address,
we can use this address to overwrite the memory that holds the return address and when the
function returns, it will return to our malicious code.
and  boom you will gain root access . 
