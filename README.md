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
