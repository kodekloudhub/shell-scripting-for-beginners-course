# Lab - Creating your first shell script
  - Take me to [Practice Test](https://kodekloud.com/topic/lab-creating-your-first-shell-script/)
  
Solutions to the practice test
- Create a script

  <details>
  
  ```
  vi create-and-launch-rocket
  
  mkdir lunar-mission
  rocket-add lunar-mission
  rocket-start-power lunar-mission
  rocket-internal-power lunar-mission
  rocket-start-sequence lunar-mission
  rocket-start-engine lunar-mission
  rocket-lift-off lunar-mission
  rocket-status lunar-mission
  
  ```
  </details>
  
- Run the command chmod +x create-and-launch-rocket

  <details>
  
  ```
  $ chmod +x create-and-launch-rocket
  ```
  </details>
  
- Run the command ./create-and-launch-rocket or bash create-and-launch-rocket
  
  <details>
  
  ```
  $ ./create-and-launch-rocket (or)
  $ bash create-and-launch-rocket
  ```
  </details>
  
- Run chmod +x /home/bob/say_hello.sh to add execute permissions to the script.
  
  <details>
  
  ```
  $ chmod +x /home/bob/say_hello.sh
  ```
  </details>
  
- The solution script is located at /tmp/assets/create-directory-structure-answer.sh Check it out.
  
  <details>
  
  ```
  $ vi create-directory-structure.sh
  
    mkdir countries
    cd countries
    mkdir USA India UK
    echo "Washington, D.C" > USA/capital.txt
    echo "London" > UK/capital.txt
    echo "New Delhi" > India/capital.txt
    uptime
    
  ```
  </details>
  
- Check the cd countries line within the script. It changes the PWD to within the countries folder. From there you do not need to specify countries within the path. To solve this, either remove the cd statement and modify the rest of the script to use countries in the path, or remove countries in the path while creating capital.txt files.
  
  <details>
  
  ```
  vi create-directory-structure-v2.sh
  
  mkdir countries

  mkdir -p countries/USA countries/India countries/UK

  echo "Washington, D.C" > countries/USA/capital.txt
  echo "London" > countries/UK/capital.txt
  echo "New Delhi" > countries/India/capital.txt

  uptime
  ```
  </details>
