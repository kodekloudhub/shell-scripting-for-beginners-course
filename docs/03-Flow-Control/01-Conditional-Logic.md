# Conditional Logic

  - Lets understand [Conditional-Logic](https://kodekloud.com/topic/conditional-logic/)

    #### Create and Launch Rocket

    - To Check the status of the rocket use below command: 

       ```
       $ rocket-status lunar-mission
       ```
    
    - To debug the status of the rocket.

       ```
       $ rocket-debug lunar-mission
       ```

    ![cl](../../images/cl.PNG)

    #### Conditional Statement

    - **`if`** is defined as 
      
      ```
      if [ $rocket_status = "failed" ]
      then
        rocket-debug $mission_name
      fi 
      ```

      ![if](../../images/if.PNG) 

    - **`elif`** condition is defined as

      ```
      if [ $rocket_status = "failed" ]
      then
        rocket-debug $mission_name
      elif [ $rocket_status = "success" ]
      then
        echo "This is successful"
      fi 
      ```

      ![elif](../../images/elif.PNG)

    - **`else`** is written as 

      ```
      if [ -d "/home/bob/caleston" ]
      then
        echo "Directory exists"
      else
        echo "Directory not found"
      ```

      ![el](../../images/el.PNG)

    #### Conditional Operators

    - Comparing statement can be used as:
     
      ![co](../../images/co.PNG)

    
    - Conditional Operators that works in **`bash`**

      ![cb](../../images/cb.PNG)

    
    - **`AND`** and **`OR`** Operators

      ![cond](../../images/cond.PNG)


    - Conditional operation description

      ![cond1](../../images/cond1.PNG)
      
