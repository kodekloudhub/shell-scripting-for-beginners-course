# Lab - Command Line Arguements and Read Inputs
  - Take me to [Practice Test](https://kodekloud.com/courses/1029419/lectures/21505834)
 
Solutions to the practice test - Command Line Arguments and Read Inputs
- Check the answer file at /tmp/assets/create-and-launch-rocket-answer
  ```
  bob@caleston-lp10:~$ cat create-and-launch-rocket
  mission_name=$1
  mkdir $mission_name

  rocket-add $mission_name

  rocket-start-power $mission_name
  rocket-internal-power $mission_name
  rocket-start-sequence $mission_name
  rocket-start-engine $mission_name
  rocket-lift-off $mission_name

  rocket-status $mission_name
  ```
- Run the script
  ```
  $ bash print-capital.sh
  ```
- Check the answer file at /tmp/assets/print-capital-answer.sh
  ```
  bob@caleston-lp10:~$ cat print-capital.sh
  echo "Capital city of $1 is $2"
  ```
- Check the answer file at /tmp/assets/backup-file-answer.sh
  ```
  bob@caleston-lp10:~$ cat backup-file.sh
  # This script creates a backup of a given file by creating a copy as bkp
  # For example some-file is backed up as some-file_bkp
  set -e

  file_name=$1

  cp $file_name ${file_name}_bkp

  echo "Done"
  bob@caleston-lp10:~$
  ```
- cat the script file and check the command-line arguments such as $1, $2
  
  
- There is a syntax issue in which the arguments are used for the usermod command. Fix it.
  ```
  new_shell=$2
  user_name=$1
  
  useradd -s $new_shell $user_name
  ```

