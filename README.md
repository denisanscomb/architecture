# architecture
Live notes system design


iQA
Live: Robustified Index Master
- 006 Test Rig iQA
- 003 cpQA2[Master] (container)
- 005 iQAtestscript (container)

LinkedIn
- 201 Index Tracker data sheet
- 202 New accounts alert (container)

iDatabase
- 500 iDatabase
- 503 iDatabase (container). Note mega() on a daily trigger
- 505 iDatabase Archive

iProcessor
 - /iProcessorpullKey (library)
 - /libAccUpdates (library)
 - /iProcessorcollect (library)
 - /iProcessorpush (library)
 - 301.1 Test Rig Analysis Processor
 - 301.2 Test Rig iProcessor (container)
 - 304 iProcessorCollect (lib)
 - 310 Test Rig iProcessorCollect (lib)
 - 303 iProcessorpush (lib)
 - 305 iProcessorpullKey (lib)
 - 302 iProcessor (container) - multiple
 - 307 Test Rig iProcessorPush (lib)
 - 311 Test Rig iProcessorpullKey (lib)
 - 313 libAccUpdates (lib)
 - 316 Freestyle Event
 - 317 Freestyle (container)

iWriter
- /iWriteCopyOps
- DEPRECIATED 100 copyWrite[Copy] (container)
- DEPRECIATED 102 libCopyOps
- DEPRECIATED 105 Test Rig libCopyOps
- 106 iWriter Master - [copywriter name] 
- Test Rig Alison 116 iWriter Master
- 107 iWriter Container
- 108 iWrtier pull library
- 109 iWriter push library
- 110 iWrtier comp processor library
- 117 iWriter Container test rig
- 118 iWriter pull library test rig
- 119 iWriter push library test rig

Adding users
- 601 New accounts for Set Up - add new accounts here
- 602 New Account Set Up (container)
- 603 New Contact Set Up - where the analysts add links to the new contacts
- 604 Model Training - for additional searches to improve yield
- 605 Model Training Data - wrangling the searches from 604
- 606 Category Management (Library) - to push iDatabase categories to all sheets


Flux Capacitor

- 701 Flux Capacitor (container)*multiple attached to different emails. Note pullmails() and wrangler2() are set up on triggers. These triggers live in edwekkpmginde@gmail.com
- 702 Flux Data
- gmail accounts with alerts are: edwekkpmgindex@gmail.com; denistest301116@gmail.com & cristianindexalerts@gmail.com
- there are different versions of 701 mapped to the different email accounts 
- 703 LinkedIn scraper (container)
- 705 Flux archive (ss)
- 706 Flux archive management (container)
- 707 FLux Gmail Scraper (container) on groupindex7@gmail.com

Dashboard

- RETIRED 901 iDashboard
- RETIRED 902 DashCon (container)
- 905 iDashboard
- 906 idashtwo (container
- 908 User Report (Lib)
- 909 backfill for 1301 - for correcting archiving errors
- 911 Timestamp Data - weekly stats
- 914 Timeseries Driver (container) - drives the aggregate account data per week to 911
- 923 Daily Timestampt Data (ss)
- 924 Daily Data (container)

User emails
- 920 Automated Reporting - templates for automated mails
- 921 AutoG Reporting (Container) - generates automatic gmail reports


- 1201 Analysts Notes - repository for errors found by analysts or their ideas for improvement
- 1301 Data Storage
- 1301.1 Data Storage Test Rig
- 1302 Sweeper - pulls in alert info and turns it into csvs for storage 
- 1303 Data Storage second phase
- 1304 Archive maintenance (lib or container?)

- 9001 Non-Event and Unchange archive
- 9001.1 Test Rig Non-Event and Unchange archive
- 9002 Non Event scripts (container)
- 9003 Historical Non-Event and Unchange archive

- 15001 storage for swept gmails from 702 Flux
- 15002 - more storage
- 15005 - (container) sweeping from 702


iDashboard
UI LinkedIn

UI Dashboard

-EditCallback - API call to api.contacts.titus.solutions AND alert for new manual entries



UI Sendwithus

ADMIN SYSTEMS

- x1101 Index CRM
- x1102 iCRM (library) - DEPRECIATED I THINK
- x1105 CRM (container)
- x1114 iCRM bcc feeder (library) attached to denistest151116@gmail.com // the bcc for the CRM
- x1118 subCRM KPI (library)

Update process
set timing of task

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



