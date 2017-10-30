# Jupyter Notebooks and Collaboration

**Speaker:** Scott Stevenson (TODO)

**Slides:** TODO

**Video:** https://www.youtube.com/watch?v=J3k3HkVnd2c


- Jupyter notesbooks have bome a popular way of working for data science.

- Version control is as important for data science as software development.
  - Allows reproducibiltiy.
  - Tracks provenance of results.
  - Aids collaboration in teams.
  
- Notebooks can simply be added to repo as normal, but this leads to
  challenges:
  - Git considers files to be plaintext.
  - Jupyter is highly structured JSON.
    - Stores code, but also results, and metadata.
    - When notebooks are re-run git will see changes to output and metadata,
      but we don't care about these diffs.

- Improvements:
  - `git add -p` allows you to cherry pick your changes to commit.
    - Simple but, seems like a lot of work.
  - Cell -> All Output -> Clear, clears the output from the notebook.
    - Allows small focused changes.
    - There may be some cases where you do care about output.

- Tools to help:
  - File save hooks, a python function to run on the notebook automatically
    on save.
    - Can be used to auto clear the output.
    - Requires every collaborator to set this up manually.
    - Applies to all noteboks for that user. not just a single project.
  - Git filters:
    - Smudge filters, can be used to convert tabs to spaces for example.
      This is not much use to us.
    - Clean filters, can be used to remove our output from the notebook.
  - nbstripout: `pip install nbstripout` ready made notebook cleaning.
  - nbdime: diff improvements:
    - Removes notebook quotes from python code.
    - Show image changes side-by-side.
    - Aids conflict resolution graphically.
    - Can show graphical diff in browser.
    
