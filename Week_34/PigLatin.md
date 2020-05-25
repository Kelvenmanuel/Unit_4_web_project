### pig Latin
```.py
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Pig Latin</title>
    <style>
            h2{color: white; text-height: 2.5em; text-align: center}
            body{background-color: purple}
            #PigLatin {font-size: 30px; color: white; font-style: italic }

    </style>
</head>
<body>

<h2> Welcome to the Pig Latin game of alterations <br> </h2>
<p id="PigLatin"> Pig Latin Game </p>

<from n="Form">
    <label for="input">Enter word:</label> <br>
    <input type="text"  value="word" id="input"><br>
</from>

<button onclick="convert_to()">Convert to Pig Latin</button> <br>
<p id="demo"></p>

</body>
<script>


    function convert_to() {

        var k = document.form['form']['input'].value
        console.log(k)
        var a = k.charAt(0);
        var b = k.substring(1);
        c = b + '-' + a + "Ay"
        console.log(c)
        document.getElementById("demo").innerHTML = c;
    }
</script>
</html>
```
