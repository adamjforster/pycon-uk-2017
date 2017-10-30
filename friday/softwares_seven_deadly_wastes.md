# Software's Seven Deadly Wastes

**Speaker:** Jez Halford ([@jezhalford](https://twitter.com/jezhalford))

**Slides:** https://www.slideshare.net/JezHalford/seven-deadly-wastes

**Video:** https://youtu.be/HRc7RBOgV_Q


- What slows you down?

- Muda: the Toyota production system, precursor to lean manufacturing

- The seven wastes:

  1. Transport:
    - What is it?
      - movement of work
      - bouncing back and forth between dev, reviewer, tester
      - deployment
    - Solutions:
      - paring and collaboration
      - CI
      - automation
      
  2. Inventory:
    - What is it?
      - undelivered work (WIP, abandoned PRs, switching between projects)
      - Little's Law (TODO link)
    - Solutions:
      - Ship little, ship often.
      - Stop starting, start finishing.
      - Focus on one thing at a time.
      
  3. Motion:
    - What is it?
      - Moving people around the work.
      - Task switching.
      - Irregular meetings.
      - Hot-desking.
    - Solution:
      - Get Rhythm!
      - Reducing inventory reduces motion.
      
  4. Waiting:
    - What is it?
      - Waiting for other teams.
      - Waiting for outside input.
      - Waiting for clarification.
    - Solutions:
      - Consider the whole system.
      - Take ownership.
      - Take pride.
      - Communicate.
    
  5. Over processing:
    - What is it?
      - Working too hard.
      - Polishing things that don't need polishing.
      - Solving imaginary scaling issues.
      - Build all the features that may ever be needed upfront.
      - Going too generic, building libraries not operational code.
    - Solutions:
      - Delivery small, deliver often.
      - Base performance improvements on evidence.
      - Refactor when you need to.

  6. Over production:
    - What is it?
      - Doing useless work
      - Building features that are never used.
      - Every feature has costs (testing, maintenance, ...).
    - Solutions:
      - Have strong product ownership
      - Remove unused features.
      
  7. Defects:
    - What is it?
      - Bugs in production code are bad.
      - bugs before production are also bad (consume time).
    - Solutions:
      - Automated testing
      - Dev / prod parity
      - CI
      - Shared understanding (are we building what they think we're building?)
