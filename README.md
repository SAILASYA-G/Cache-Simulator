# Cache-Simulator

Author: Sailasya Gangavarapu

Designed and developed a flexible cache and memory hierarchy simulator in Python

CACHE is configurable in terms of supporting any cache size, associativity, and block size, specified at the beginning of simulation: 
  o SIZE: Total bytes of data storage.
  o ASSOC: The associativity of the cache (ASSOC = 1 is a direct-mapped cache). 
  o BLOCKSIZE: The number of bytes in a block.
  
Successfully implemented three different Replacement Policies namely:
  o LRU (Least Recently Used)
  o FIFO (First In First Out)
  o Optimal Policy
  
Inputs to the Simulator:
  a. BLOCKSIZE 
  b. L1_SIZE 
  c. L1_ASSOC 
  d. L2_SIZE 
  e. L2_ASSOC 
  f. REPLACEMENT_POLICY (0 for LRU, 1 for FIFO, 2 for Optimal)
  g. INCLUSION_PROPERTY (0 for non-inclusive, 1 for inclusive)
  h. trace_file

Outputs from the Simulator:
  a. number of L1 reads
  b. number of L1 read misses
  c. number of L1 writes
  d. number of L1 write misses
  e. L1 miss rate
  f. number of writebacks from L1 to next level
  g. number of L2 reads
  h. number of L2 read misses if there is a L2 cache
  i. number of L2 writes
  j. number of L2 write misses
  k. L2 miss rate
  l. number of writebacks from L2 to memory
  m. total memory traffic 
  
Commands to run the code:
- Open command prompt and navigate to the folder with the sim_cache.py code.
- Run the following command once in the code directory:
    python sim_cache.py BLOCKSIZE L1_SIZE L1_ASSOC L2_SIZE L2_ASSOC REPLACEMENT_POLICY INCLUSION_PROPERTY trace_file
