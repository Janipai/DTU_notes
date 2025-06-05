**Cycle stealing**: the DMA device steals a CPU memory cycle in order to execute a data transfer.
During the DMA operation, the I/O transfer and the CPU program execution run in parallel

**Time-slice method**: each memory cycle is split into two adjacent time slots: one reserved
for the CPU and the other for the DMA device.

Time-slice is more expansive than cycle stealing (but more predictable)
program locality: the most frequent accesses to the main memory are limited to a small address space, a phenomenon

cache-related preemption delay (CRPD)
Direct memory access (DMA) 

- **Interrupt Handling**:
    
    - **First Approach**: All external interrupts are disabled (except the timer).
    - **Second Approach**: All interrupts are disabled, with devices managed periodically by kernel routines.
    - **Third Approach**: All external interrupts are enabled, and small drivers are used to activate dedicated device-handling tasks.
- **Device Management**:
    
    - **First Approach**: Devices are handled directly by application tasks.
    - **Second Approach**: Devices are managed by periodic kernel routines.
    - **Third Approach**: Devices are managed by dedicated tasks activated by drivers, which are scheduled by the operating system like regular tasks.
- **Busy Waiting**:
    
    - **First and Second Approaches**: Both involve busy waiting during I/O operations.
    - **Third Approach**: Eliminates busy waiting by delegating device handling to dedicated tasks.
- **Predictability and Overhead**:
    
    - **First Approach**: No overhead from kernel routines or drivers, but unbounded delays can occur in task execution due to polling.
    - **Second Approach**: Higher overhead from kernel routines but avoids unbounded delays from interrupt drivers.
    - **Third Approach**: Drastically reduces unbounded delays and eliminates busy waiting, though a small overhead from minimal drivers remains.
- **Task Prioritization**:
    
    - **First and Second Approaches**: Task priorities depend on the structure of the kernel routines or application tasks.
    - **Third Approach**: Allows independent prioritization of device-handling tasks, enabling flexibility to assign priorities based on application requirements.
- **Adoption**:
    
    - **First Approach**: Used in RK.
    - **Second Approach**: Used in the MARS system.
    - **Third Approach**: Used in ARTS, HARTIK, and SPRING systems.
___________________________________________________________
Project:
explain what you have done and be concise.

It is allowed to simplify the model - but don't simplify too much

![[Pasted image 20250207100045.png]]