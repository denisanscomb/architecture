# architecture
Live notes system design

Update process
1. Write down user stories / tasks
2. Define the unknowns in building the new features & decide a process
3. Check github code is the same as live code. If not committ live code to GitHub
4. Pull code to test rigs and build updates
5. Switch the sheet IDs from live to test
6. Test with a user
7. Update the notation on the script
7. Switch from test to live sheet IDs
8. Committ to live system

General tips

Have a separate window for tabs relating to the work
Close them all afterwards


iDatabase
- 500 iDatabase
- 503 iDatabase (container)

iProcessor
 - /iProcessorpullKey (library)
 - /libAccUpdates (library)
 - /iProcessorcollect (library)
 - 304 iProcessorCollect (lib)
 - 310 Test Rig iProcessorCollect (lib)
 - 303 iProcessorpush (lib)
 - 305 iProcessorpullKey (lib)
 - 302 iProcessor (container) - multiple
 - 307 Test Rig iProcessorPush (lib)
 - 311 Test Rig iProcessorpullKey (lib)
 - 313 libAccUpdates (lib)


iWriter
- /iWriteCopyOps
- 100 copyWrite[Copy] (container)
- 102 libCopyOps
- 105 Test Rig libCopyOps

iQA
Live: Robustified Index Master
Test: Test Rig iQA
- 003 cpQA2[Master] (container)

Flux Capacitor

- 701 Flux Capacitor (container)*multiple attached to different emails
- 703 LinkedIn scraper (container)

Admin:

1201 Analysts Notes - repository for errors found by analysts or their ideas for improvement


iDashboard
UI LinkedIn
UI Dashboard
UI Sendwithus


