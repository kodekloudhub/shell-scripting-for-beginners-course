# Lab - Arithmetic Operations
  - Take me to [Practice Test](https://kodekloud.com/topic/lab-airthmetic-operations-2/)
  
Solutions to practice test - Arithmetic Operations

- Check the solution at /tmp/assets/calculation-answer.sh

  <details>
  
  ```
  bob@caleston-lp10:~$ cat calculation.sh
  A=20
  B=10

  echo "Sum is $(( A + B))"
  echo "Difference is $(( A - B))"
  echo "Product is $(( A * B))"
  echo "Quotient is $(( A / B))"
  ```
  ```
  $ bash calculation.sh
  ```
  </details>
  
- Check the solution at /tmp/assets/calculation-answer-2.sh
  
  <details>
  
  ```
  bob@caleston-lp10:~$ cat calculation.shA=$1
  B=$2

  echo "Sum is $(( A + B))"
  echo "Difference is $(( A - B))"
  echo "Product is $(( A * B))"
  echo "Quotient is $(( A / B))"
  ```
  </details>
  
- Check the solution at /tmp/assets/calculate-price.sh
  
  <details>
  
  ```
  bob@caleston-lp10:~$ cat calculate-price.sh
  price=$(( $1 * $2 ))

  echo "The total price for items is ${price} dollars"
  ```
  </details>
  
- The "*" should be escaped as "\*" for multiplication using expr statement.
  
  <details>
  ```
  $ cat calculate-total-apples.sh
    baskets=4
    apples_per_basket=5
    total_apples=`expr $baskets \* $apples_per_basket`
    echo "Total Apples = $total_apples"
  ```
  </details>
  
- Answer script: /tmp/assets/calculate-average-answer.sh
  
  <details>
  
  ```
  $ cat calculate-average.sh
    num1=$1
    num2=$2
    num3=$3
    sum=$(( num1 + num2 + num3 ))
    average=$(echo "$sum / 3" | bc -l)
  ```
  </details>
