MULTI-WAY  BRANCHING 
Simple Calculator Algorithm
Step 1 : Start
Step 2 : Read operands a and b Step 3 : Display operation menu Step 4 : Read option
Step 5 : If option = 1 then Calculate c = a + b
Step 5.1 : else if option = 2 then Calculate c = a – b Step 5.2 : else if option = 3 then Calculate c = a * b Step 5.3 : else if option = 4 then Calculate c = a / b Step 5.4 : else if option = 5 then Calculate c = a % b
Step 5.5 : else
Print "Invalid option" Step 6 : Print c
Step 7 : Stop
Program
# Arithmetic operations--multiple statements in a block echo -n "Enter the two numbers : "
read a b
echo " 1. Addition" echo " 2. Subtraction" echo " 3. Multiplication" echo " 4. Division"
echo " 5. Modulo Division" echo -n "Enter the option : " read option case $option in
1)	c=`expr $a + $b` echo "$a + $b = $c";;
2)	c=`expr $a - $b` echo "$a - $b = $c";;
3)	c=`expr $a \* $b` echo "$a * $b = $c";;
4)	c=`expr $a / $b` echo "$a / $b = $c";;
5)	c=`expr $a % $b` echo "$a % $b = $c";;
*) echo "Invalid Option" esac
Output
[student@krce ~]$ shsimplecal.sh Enter the two numbers : 2 4
1.	Addition
2.	Subtraction
3.	Multiplication
4.	Division
5.	Modulo Division Enter the option : 1 2 + 4 = 6

