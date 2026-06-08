//=========================================================================
// Name & Email must be EXACTLY as in Gradescope roster!
// Name: jiachang ye
// Email: jye081@ucr.edu
// 
// Assignment name: lab6
// Lab section: Thu 3pm
// TA: Allan Knight
// 
// I hereby certify that I have not received assistance on this assignment,
// or used code, from ANY outside source other than the instruction team
// (apart from what was provided in the starter file).
//
//=========================================================================

Data for hello_c indicates that separate caches are optimal: miss rate = 4.85%, cost = 43,614.
Data for hello_cpp indicates that separate caches are optimal: miss rate = 1.29%, cost = 43,614.

Regarding matrix multiplication programs, row-major order performs faster than column-major order when processing large-scale datasets.

Graph: 
![alt text](<2026-06-08 010147.png>)

hello_c and hello_cpp are dominated by instruction accesses; however, hello_c involves more data accesses due to its use of printf, resulting in a lower cache hit rate compared to hello_cpp.

The row-major matrix multiplication access pattern is cache-friendly, as the continuous access of each row places minimal demand on the instruction cache.

Column-major matrix multiplication frequently results in cache line misses, causing the execution time to far exceed that of the row-major approach.