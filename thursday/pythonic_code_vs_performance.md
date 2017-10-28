# Pythonic Code vs. Performance

**Speaker:** Lukasz Kakol (@llanga)

**Slides:** http://lukkol.pl/pyconuk2017-performance

**Video:** TODO


- Performance aspects:
  - CPU time, 50% of web users abandon a page after waiting 3 seconds too load.
  - Memory, we don't care about it until we run out!
  - I/O operations, DBs ...
  
- Improve performace:
  - Plan.
  - Measure.
  - Monitor.
  - Identify bottlenecks and simple fixes.
  - Don't try to optimise everything, low cost, high profit.
  
- Profile tools:
  - cProfile.
  - memory_profiler.
  - psutil, plugin for memory_profiler.
  - dis, used to disassemble the code.
  
- Demo: see slides
