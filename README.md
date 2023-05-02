Download Link: https://assignmentchef.com/product/solved-cpe434-exam1
<br>
1 <strong>.Fragmentation and Page Sizes</strong>:

Many modern Intel processors support multiple page sizes such as 4KB and 2MB pages.

<ul>

 <li>What is the difference between external fragmentation and internal fragmentation?</li>

 <li>What is the impact of page size on fragmentation?</li>

</ul>

The page table approach to memory management emerged at a time when machine’s address space vastly exceeded the size of physical memory.  While the address space has gotten larger and larger physical memory has also gotten larger to the extent that overhead from paging small pages has gotten excessive. One solution to this problem has been to have different size pages. For example, the modern  Intel processor can have 4 KB and 2MB pages.  With large pages the number of TLB misses and page faults go down

<ul>

 <li>One approach to choosing page sizes might be to let the user decide. Windows does in fact have a system call (VirtualAlloc) that lets you choose different page sizes for a specific allocation.  Another approach would be to have the operating system make measurements and change the page size accordingly (remember, the user logical address space would not change).  Propose an algorithm similar to the working set algorithm for dynamically choosing the page size. Describe in as much detail as possible. About 1 page.</li>

</ul>

<ol start="2">

 <li><strong>Page Tables </strong></li>

</ol>

An engineer has been hired to design a multilevel page table system for a machine with 32  bit addresses.  Vaguely recalling from class a three level page table design, they choose a three level page table with field widths for each portion of the virtual address is 5, 6, and 7 bits respectively

For the following questions SHOW ALL WORK

<ul>

 <li>for the smallest program possible, consisting of one page of text and heap starting at address 0 and one page of stack starting at the highest address (0xff…f) what is the size of the page table  structure in bytes.</li>

 <li>is this a good architecture. (yes or no) Explain your answer.</li>

 <li>for the largest program possible, consisting of all pages starting at address 0 and 5+6+7 bits) running to the highest address possible (0xff…f) what is the size of the index structure in bytes.</li>

</ul>

<ol start="3">

 <li><strong>Scheduling</strong></li>

</ol>

<ul>

 <li>Given the following processes and execution times</li>

</ul>

Process Time

P1         13

P2           5

P3         23

P4           3

P5         31

P6           3

P7         14

Calculate the completion time for each task for round robin, first come first served and shortest job first scheduling algorithms? Assume that a quantum of 5 is being used when a quantum of time is necessary.  SHOW ALL WORK

4-  TLB

<ul>

 <li>Assuming a three level page table, a tlb hit time of 10 ns, a main memory access time of 50 ns, a hit rate of 95%, what is the average memory access time?  SHOW ALL WORK</li>

 <li>What cache hit rate do you need for an average access time of 90ns</li>

 <li>What cache hit rate do you need for an average access time of 150n</li>

</ul>

<ol start="5">

 <li><strong>Synchronization</strong></li>

</ol>

<ul>

 <li>What is a critical section and what is it used for?</li>

 <li>Explain what counting semapores, mutex semaphores, and synchronization semaphores are and give an example of their use.</li>

 <li>Do you need synchronization capabilities like semaphores if you only have a single core processor? Explain your answer</li>

</ul>