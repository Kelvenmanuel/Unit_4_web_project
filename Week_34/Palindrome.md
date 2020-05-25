### Palindrome
```.py
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>CheckPalindrome</title>
    <style>
        body{background-color: cadetblue}
        h2{font-size: 50px}
    </style>
</head>
<body>
<h2> Check if a string is an Palindrome <br> </h2>
<p id="PigLatin"> Pig Latin Game </p>

<from n="Form">
    <label for="input">Enter word:</label> <br>
    <input type="text"  value="word" id="input"><br>
</from>

<button onclick="invert_to()">Invert to palindrome</button> <br>
<p id="demo"></p>

</body>
</html>
<script>
    function invert_to() {
        var input = document.forms["Form"]["input"].value;
        var i;
        var to_convert= ""
        //console.log(input)
        for (i=1; i<= input.length; i++){
            console.log(input)
            to_convert += input.substr(-1*i, 1)
            if (to_convert == input){
                var check = "The input wrote " + input + "is a palindrome"
            }else{
                check = "The input wrote" + input + "is not a Palindrome"
            }
        }
        document.getElementById("demo").innerHTML = to_convert + "<br>" + check;
        // console.log(to_convert)
    }
</script>
```
