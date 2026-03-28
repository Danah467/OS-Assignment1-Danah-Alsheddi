# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry 1 - [March 27, 2026, 1:30 AM]
**What I did**: Started setting up the project and forked the repository.

**Details**: 
• Forked the starter repo on GitHub.
• Cloned it and opened it in VS Code.
• Updated my student ID in SchedulerSimulation.java.
• Ran the program to make sure everything worked.

**Challenges**: VS Code didn’t detect the JDK at first.

**Solution**: Reinstalled Java extensions and selected the correct JDK.

**Time spent**: 40 minutes.

---

### Entry 2 - [March 27, 2026, 8:00 AM]
**What I did**: Implemented Feature 1 (Process Priority).

**Details**: • Added a priority field to each process.
• Displayed the priority when the process enters the ready queue.
• Tested the output to confirm priorities were printed correctly.

**Challenges**: Output formatting broke because of color codes.

**Solution**: Adjusted spacing and added proper color resets.

**Time spent**: 1 hour

---

### Entry 3 - [March 27, 2026, 9:00 AM]
**What I did**: Implemented Feature 2 (Context Switch Counter).

**Details**:
• Added a static counter for context switches.
• Incremented it every time a new process started running.
• Printed the total at the end of the simulation.

**Challenges**: The counter increased twice per switch.

**Solution**: Moved the increment to the correct location.

**Time spent**: 1 hour 15 minutes.

---

### Entry 4 - [March 27, 2026, 10:30 AM]
**What I did**: Implemented Feature 3 (Waiting Time Tracking).

**Details**:
• Created a map to store waiting time for each process.
• Increased waiting time whenever a process was re‑queued.
• Printed a summary table at the end.

**Challenges**: Waiting times were incorrect at first.

**Solution**: Updated the logic to count waiting only when the process is actually in the queue.

**Time spent**: 2 hours

---

### Entry 5 - [March 27, 2026, 12:00 PM]
**What I did**: Final testing and code cleanup.

**Details**: 
• Ran the full simulation with all processes.
• Verified context switches and waiting times.
• Removed unused variables and cleaned formatting.

**Challenges**: VS Code warnings were confusing.

**Solution**: Reviewed the code and confirmed they were harmless.

**Time spent**: 45 minutes

---

### Entry 6 - [March 27, 2026, 1:00 PM]
**What I did**: Final commits and GitHub upload.

**Details**: 
• Created separate commits for each feature.
• Pushed everything to GitHub.
• Checked commit history to confirm everything uploaded correctly.

**Challenges**: Unsure if GitHub saved the latest version.

**Solution**: Opened each commit and verified the changes.

**Time spent**: 20 minutes

---

## Summary

**Total time spent on assignment**: [X hours]**~6 hours**

**Most challenging part**: Implementing waiting time because it required tracking every re‑queue.

**Most interesting learning**: Understanding how threads and Round‑Robin scheduling work together.

**What I would do differently next time**: Start earlier and break the work into smaller sessions.
