# Lab - Variables
  - Take me to [Practice Test](https://kodekloud.com/courses/1029419/lectures/21505714)
  
Solutions to practice test - variables

- Check the answer file at /tmp/assets/create-and-launch-rocket-answer
  ```
  bob@caleston-lp10:~$ cat create-and-launch-rocket
  mission_name=lunar-mission

  mkdir $mission_name

  rocket-add $mission_name

  rocket-start-power $mission_name
  rocket-internal-power $mission_name
  rocket-start-sequence $mission_name
  rocket-start-engine $mission_name
  rocket-lift-off $mission_name

  rocket-status $mission_name

  ```
  ```
  $ bash create-and-launch-rocket
  ```
- Variable name must be in the same case as defined $user_name
  ```
  bob@caleston-lp10:~$ cat print-welcome-message.sh
  user_name=Michael

  echo "Hi $user_name, Welcome to xFusionCorp Industries. Weand the rest of the management are glad to have you on board"
  ```
  
- Variable name should not have a dash. Change it to uptime
  ```
  bob@caleston-lp10:~$ cat print-uptime.sh
  uptime=$(uptime)

  echo "The uptime of the system is $uptime"
  ```
- Variable should be encapsulated in { }. Change variable to ${file_name}_bkp
  ```
  bob@caleston-lp10:~$ cat backup-file.sh
  # This script creates a backup of a given file by creatinga copy as bkp# For example some-file is backed up as some-file_bkp

  file_name="create-and-launch-rocket"

  cp $file_name ${file_name}_bkp
  ```

- Make sure that the variable names that are defined are actually the ones being used in the script.
  ```
  bob@caleston-lp10:~$ cat create_files.sh
  FILE01="Japan"FILE02="South Korea"
  FILEO3="Canada"

  cd /home/bob

  echo "Creating file called $FILE01"
  touch $FILE01

  echo "Creating file called $FILE02"touch $FILE02

  echo "Creating file called $FILE03" 
  touch $FILE02
  ```
  
- This script uses an environment variable. If unclear, check out the Bash section in the Linux Basics Course
  

