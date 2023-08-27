### PROJECT CALCULATOR 
### HTML & JAVASCRIPT

<html>
    <head>
    <title>SIMPLE CALCULATOR</title>
    <link type="text/css" rel="stylesheet" href="calculator.css" />

    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@100&display=swap" rel="stylesheet">

</head>
<body>

    <div id="appBg">
     <form name="simpleCalculator"class="contenedor">
          
          <input type="textfield" name="ans" value="" autocomplete="off" readonly class="display">
          <br>
          <input type="button" value="7" onclick="document.simpleCalculator.ans.value+='7'" class="button1">
          <input type="button" value="8" onclick="document.simpleCalculator.ans.value+='8'" class="button1">
          <input type="button" value="9" onclick="document.simpleCalculator.ans.value+='9'" class="button1">
          <input type="button" value="+" onclick="document.simpleCalculator.ans.value+='+'" class="button1">
          <br>
          <input type="button" value="4" onclick="document.simpleCalculator.ans.value+='4'" class="button1">
          <input type="button" value="5" onclick="document.simpleCalculator.ans.value+='5'" class="button1">
          <input type="button" value="6" onclick="document.simpleCalculator.ans.value+='6'" class="button1">
          <input type="button" value="-" onclick="document.simpleCalculator.ans.value+='-'" class="button1">
          <br>  
          <input type="button" value="1" onclick="document.simpleCalculator.ans.value+='1'" class="button1">
          <input type="button" value="2" onclick="document.simpleCalculator.ans.value+='2'" class="button1">
          <input type="button" value="3" onclick="document.simpleCalculator.ans.value+='3'" class="button1">
          <input type="button" value="*" onclick="document.simpleCalculator.ans.value+='*'" class="button1">
          <br>
          <input type="button" value="0" onclick="document.simpleCalculator.ans.value+='0'" class="button1">
          <input type="reset" value="C"class="button1">
          <input type="button" value="=" onclick="document.simpleCalculator.ans.value=eval(document.simpleCalculator.ans.value)"class="button1">
          <input type="button" value="/" onclick="document.simpleCalculator.ans.value+='/'"class="button1">
          <br>
          <input type="button" value="←" onclick="document.simpleCalculator.ans.value=document.simpleCalculator.ans.value.slice(0,-1)"class="button2">
      </form>
 </div>
</body>
