# Lab Conditional Logic

  - Take me to the [Lab](https://kodekloud.com/topic/lab-conditional-logic/)


  1. See the solution
    
     <details>
    
      ```
      mission_name=$1

      mkdir $mission_name
      
      rocket-add $mission_name
      
      rocket-start-power $mission_name
      rocket-internal-power $mission_name
      rocket-start-sequence $mission_name
      rocket-start-engine $mission_name
      rocket-lift-off $mission_name
      
      rocket_status=$(rocket-status $mission_name)
      
      echo "The status of launch is $rocket_status"
      
      if [ $rocket_status = "failed" ]
      then
        rocket-debug $mission_name
      fi     
      ```
      </details>

  2. See the solution
    
     <details>
    
      ```
      if [ -d "/home/bob/caleston" ]
      then
        echo "Directory exists"
      else
        echo "Directory not found"
      fi
      ```
      </details>

  3. See the solution
    
     <details>
    
      ```
      if [ $1 -gt $2 ]
      then
          echo $1
      else
          echo $2
      fi
      ```
      </details>

  4. See the solution
    
     <details>
    
      ```
      month_number=$1
      
      if [ -z $month_number ]
      then
        echo "No month number given. Please enter a month number as a command line argument."
        echo "eg: ./print-month-number 5"
        exit
      fi
      
      if [[ $month_number -lt 1 && $month_number -gt 12 ]]
      then
        echo "Invalid month number given. Please enter a valid number - 1 to 12."
        exit
      fi
      
      if [ $month_number -eq 1 ]
      then
        echo "January"
      elif [ $month_number -eq 2 ]
      then
        echo "February"
      elif [ $month_number -eq 3 ]
      then
        echo "March"
      elif [ $month_number -eq 4 ]
      then
        echo "April"
      elif [ $month_number -eq 5 ]
      then
        echo "May"
      elif [ $month_number -eq 6 ]
      then
        echo "June"
      elif [ $month_number -eq 7 ]
      then
        echo "July"
      elif [ $month_number -eq 8 ]
      then
        echo "August"
      elif [ $month_number -eq 9 ]
      then
        echo "September"
      elif [ $month_number -eq 10 ]
      then
        echo "October"
      elif [ $month_number -eq 11 ]
      then
        echo "November"
      elif [ $month_number -eq 12 ]
      then
        echo "December"
      fi 
      ```
      </details>
