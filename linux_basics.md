# Linux Command Notes

## Navigation 
- 'cd'              # change directory
- 'ls'              # list files
- 'pwd'             # shows where I am
- 'ls'              # shows whats in the folder
- 'cd'              # moves me around folders

## File Management
- 'touch'           # create file
- 'echo'            # write to file
- 'cat'             # print file
- 'rm'              # remove file
- 'mkdir'           # create folder 
- 'rmdir'           # remove folder

## Real-World Practice
jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ mkdir automation

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ mdir inputs logs outputs
bash: mdir: command not found

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ mkdir inputs logs outputs

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ ls
README.md  automation/  git_basics.md  inputs/  linux_basics.md  logs/  outputs/  test.text

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ rmdir inputs logs outputs

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ cd automation

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation (main)
$ mkdir inputs logs outputs

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation (main)
$ ls
inputs/  logs/  outputs/

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation (main)
$ cd logs

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/logs (main)
$ touch test_run.log

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/logs (main)
$ echo "Test run completed successfully at jackson" > test_run.log

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/logs (main)
$ cat test_run.log
Test run completed successfully at jackson

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/logs (main)
$ cd..
bash: cd..: command not found

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/logs (main)
$ cd

jacks@JJs-Surface-Pro MINGW64 ~
$ cd ^[[200~C:\Users\jacks\Cybersecurity_Learning\phase1-dev-journal~
bash: cd: $'\E[200~C:UsersjacksCybersecurity_Learningphase1-dev-journal~': No such file or directory

jacks@JJs-Surface-Pro MINGW64 ~
$ cd C:\Users\jacks\Cybersecurity_Learning\phase1-dev-journal
bash: cd: C:UsersjacksCybersecurity_Learningphase1-dev-journal: No such file or directory

jacks@JJs-Surface-Pro MINGW64 ~
$ ls
 -1.14-windows.xml                                                                             'OneDrive - Florida State University'/
 AppData/                                                                                       PrintHood@
'Application Data'@                                                                             PycharmProjects/
 BitVector/                                                                                     Recent@
 Box/                                                                                          'Saved Games'/
'C Programs'/                                                                                   Searches/
 CPP/                                                                                           SendTo@
 C_Programming/                                                                                'Shape Inheritance'/
 CofeeCustData/                                                                                'Simple Vector'/
 CoffeeCustByMethodData/                                                                       'Start Menu'@
 CoffeeCustClass/                                                                               SteakSurveyData/
 Contacts/                                                                                      Templates@
 Cookies@                                                                                      'VirtualBox VMs'/
 Cybersecurity_Learning/                                                                        exam3Practice/
'Date Program'/                                                                                 football_predictor.ipynb
 Documents/                                                                                     getdocker.sh*
 Downloads/                                                                                     linkList/
 Dropbox/                                                                                      'matrix multiplication'/
 Favorites/                                                                                     moviers/
 IntelGraphicsProfiles/                                                                         ntuser.dat.LOG1
'Jupyter Lab'/                                                                                  ntuser.dat.LOG2
 Links/                                                                                         ntuser.ini
'Local Settings'@                                                                               source/
'Lottery Numbers'/                                                                              stack/
'MIPS Practice'                                                                                 terraform.tfstate
'My Documents'@                                                                                 test/
 NTUSER.DAT                                                                                     untitled/
 NTUSER.DAT{1cb79d27-10b1-11f0-984b-abfa2a370668}.TM.blf                                        untitled1/
 NTUSER.DAT{1cb79d27-10b1-11f0-984b-abfa2a370668}.TMContainer00000000000000000001.regtrans-ms   untitled2/
 NTUSER.DAT{1cb79d27-10b1-11f0-984b-abfa2a370668}.TMContainer00000000000000000002.regtrans-ms   untitled3/
 NetHood@                                                                                       untitled4/
 OneDrive/

jacks@JJs-Surface-Pro MINGW64 ~
$ cd Cybersecurity_Learning/

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning
$ ls
COP4530/  Learning_Python/  Terraform/  cpp_Basics/  docker-nginx-app/  phase1-dev-journal/

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning
$ cd phase1-dev-journal/

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ ls
README.md  automation/  git_basics.md  linux_basics.md  test.text

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ cd automation/logs

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/logs (main)
$ ls
test_run.log

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/logs (main)
$ cd.
bash: cd.: command not found

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/logs (main)
$ cd ..

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation (main)
$ cd outputs

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/outputs (main)
$ touch temp.bak

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/outputs (main)
$ rm temp.bak

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/outputs (main)
$ ls

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/outputs (main)
$ pwd
/c/Users/jacks/Cybersecurity_Learning/phase1-dev-journal/automation/outputs

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/outputs (main)
$ ls

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation/outputs (main)
$ cd ..

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation (main)
$ pwd
/c/Users/jacks/Cybersecurity_Learning/phase1-dev-journal/automation

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation (main)
$ ls
inputs/  logs/  outputs/

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal/automation (main)
$ cd ..

jacks@JJs-Surface-Pro MINGW64 ~/Cybersecurity_Learning/phase1-dev-journal (main)
$ ls
README.md  automation/  git_basics.md  linux_basics.md  test.text
