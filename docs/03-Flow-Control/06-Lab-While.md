# Lab while

  - Lets do some practical with [while Loop](https://kodekloud.com/topic/labs-while-loops/)

  1. Solution is given below

     <default>
    
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
      
      while [ $rocket_status = "launching" ]
      do
        sleep 2
        rocket_status=$(rocket-status $mission_name)
      done
      
      if [ $rocket_status = "failed" ]
      then
        rocket-debug
      fi
      ```

     </default>

  2. Solution is given below

     <default>
     
      ```
      to_number=$1
      number=0
      while [ $number -lt $to_number ]
      do
        echo $(( number++ ))
      done
      ```
  
     </default>

  3. Solution is given below

     <default>
 
      ```
      Print the numbers from 0 to give number
      ```
   
     </default>

  4. Solution is given below

     <default>
 
      ```
      while true
      do
        echo "1. Add"
        echo "2. Subsctract"
        echo "3. Multiply"
        echo "4. Divide"
        echo "5. Quit"
      
        read -p "Enter your choice: " choice
      
        if [ $choice -eq 1 ]
        then
              read -p "Enter Number1: " number1
              read -p "Enter Number2: " number2
              echo Answer=$(( $number1 + $number2 ))
        elif [ $choice -eq 2 ]
        then
              read -p "Enter Number1: " number1
              read -p "Enter Number2: " number2
              echo Answer=$(( $number1 - $number2 ))
        elif [ $choice -eq 3 ]
        then
              read -p "Enter Number1: " number1
              read -p "Enter Number2: " number2
              echo Answer=$(( $number1 * $number2 ))
        elif [ $choice -eq 4 ]
        then
              read -p "Enter Number1: " number1
              read -p "Enter Number2: " number2
              echo Answer=$(( $number1 / $number2 ))
        elif [ $choice -eq 5 ]
        then
          break
        fi
      
      done
      ```

     </default>