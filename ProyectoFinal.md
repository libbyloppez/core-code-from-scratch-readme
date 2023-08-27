### PROYECTO CALCULADORA
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

### CSS

```
.contenedor{
    background-color: rgba(225, 20, 48, 0.824);
    width: max-content;
    padding: 10px;
    border-radius: 5px;

}

```

.display{
    width: 100%;
    height: 40px;
    margin-bottom: 10px;
    color:white;
    background-color:rgb(186, 178, 184) ;

    
}

.button1{
    
    width: 50px;
    height: 50px;
    margin-bottom: 4px;
    color:white;
    background-color: rgb(248, 13, 201);
    border: 2px solid #e6f1e6;
    border-radius: 5px;
    transition: 0.5s;
}

.button1:hover{
    cursor: pointer;
    background-color: rgb(203, 46, 49);
    transition: 0.5s;
    transform: scale(1.3);
}

.button2{
    width: 100%;
    height: 50px;
    color:white;
    background-color: rgb(248, 13, 201);
    border: 2px solid #f0efe9;
    border-radius: 5px;
    transition: 0.5s;
}

.button2:hover{
    cursor: pointer;
    background-color: rgb(241, 9, 83);
    transition: 0.5s;
    transform: scale(1.07);
}
```

### PROYECTO DASHBOARD


    




