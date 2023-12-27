# ODD23-24-WT-JavaScript
NAME: MYTHILI.V

REFERENCE NUMBER: 23012444

DEPARTMENT: COMPUTER SCIENCE ENGINEERING

PROGRAM 1


AIM:
To create a form with java script code to calculate electricity bill.

DESIGNING PROCEDURE:


STEP 1: Start define the document as HTML.

STEP 2: Open the HTML structure with necessary head and body .Give the script type as text/javascript.

STEP 3: Define the function for the program as calc().

STEP 4: Give the necessary input that is required for calculating the electricity bill like var prev,curr,units,amt. Get the number for input using document.getElementById.

STEP 5: Give the necessary condition using if-else condition. Close the script and head tags.

STEP 6: Give the input type in the body of the HTML.

STEP 7 : End the HTML structure.

PROGRAM:
```
<html>
<head>
<script type="text/javascript">
function calc()
{
var prev,curr,units,amt;
prev=Number(document.getElementById("t1").value);
curr=Number(document.getElementById("t2").value);
units=curr-prev;
if(units<=100)
	amt=100;
else if(units>100&&units<=300)
	amt=100+(units-100)*3;
else
	amt=100+600+(units-300)*5;
document.getElementById("t3").value=amt;
}
</script>
</head>
<body>
<h2>Electricity Bill</h2>
<form>
Enter Previous Reading 
<input type="text" id="t1">Enter Current Reading
<input type="text" id="t2">
<input type="button"  onclick="calc()" value="Generate Bill">
<input type="text" id="t3">
</form>
</body>
</html>
```
OUTPUT:

![elepic](https://github.com/Mythili7339267708/ODD23-24-WT-JavaScript/assets/144260246/38bdb461-64cf-4481-9d90-dd38e44601b1)

RESULT:

Thus the java code executed to calculate the electricity bill.

PROGRAM 2


AIM:


To create a form with java script code to compute the factorial of a given number without recursion.

DESIGNING PROCEDURE:


STEP 1: Start define the document as HTML.

STEP 2: Open the HTML structure with necessary head and body .Give the script type as text/javascript.

STEP 3: Define the function for the program as show().

STEP 4: Give the necessary input that is require to compute the factorial like var i, n, fact. Get the number for input using document.getElementById.

STEP 5: Using for-loop condition calculate the factorial. Close the script and head tags.

STEP 6: Give the input type in the body of the HTML.

STEP 7 : End the HTML structure.

PROGRAM:
```
<html>
<head>
<script type="text/javascript">
function show()
{
var i, n, fact;
fact=1;
n=Number(document.getElementById("num").value);
for(i=1; i<=n; i++)  
{
fact= fact*i;
}  
document.getElementById("answer").value= fact;
}
</script>
</head>
<body>
<form>
Enter Number: <input type="text" id="num">
<button onclick="show()">Factorial</button>
<input type="text" id="answer">
</form>
</body>
</html>
```
OUTPUT:

![facpic](https://github.com/Mythili7339267708/ODD23-24-WT-JavaScript/assets/144260246/59f17e82-a88e-4ac2-9638-7389a10dec25)

RESULT:

Thus the java code executed to compute the factorial of a given number without recursion.

PROGRAM 3

AIM:

To construct a JavaScript code to generate ‘N’ prime numbers.

DESIGNING PROCEDURE:

STEP 1: Start define the document as HTML.

STEP 2: Open the HTML structure with necessary head and body .Give the script type as text/javascript.

STEP 3: Define the function for the program as show().

STEP 4: Give the necessary input that is required to construct a java code to generate ‘N’ prime numbers . Get the number for input using document.getElementById.

STEP 5: Using for-loop condition generate ‘N’ prime numbers. Close the script and head tags.

STEP 6: Give the input type in the body of the HTML.

STEP 7 : End the HTML structure.

PROGRAM:
```
<html>
<head>
<script type="text/javascript">
function show()
{
var low=Number(document.getElementById("n1").value);
var high=Number(document.getElementById("n2").value);
var i,j;
for(i=low;i<=high;i++) 
{
var flag=0;
for(j=2;j<i;j++) 
{
if(i%j==0) 
{
flag=1;
break;
}
}
if(flag==0&&i>1) 
alert(i);
}
}
</script>
</head>
<body>
<form>
    Enter Number:
<input type="text" id="n1">
<input type="text" id="n2">
<input type="button" onclick="show()" value="Generate">
</form>
</body>
</html>
```
OUTPUT:

![nprimepic](https://github.com/Mythili7339267708/ODD23-24-WT-JavaScript/assets/144260246/f1544754-96af-4339-b8aa-d881bd6cdfca)
