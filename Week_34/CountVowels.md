### Count Vowels
```.py
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title> Count Value Kelven</title>
    <style>
        body{background-color: mediumturquoise}
        h2{font-size: 50px}
    </style>
</head>
<body>
<h2> Count Values website <br> </h2>


<from n="Form">
    <label for="input">Enter a sentence below :</label> <br>
    <input type="text"  value="word" id="input"><br>
</from>

<button onclick="count_val()">Count</button> <br>
<p id="demo"></p>
</body>
</html>
<script>
    var a
    var array = ["a", "e", "i", "o", "u"];
    var letter=""
    for (a = 0; a<5; a++) {
        letter += array[a] + ":" + "<br>" + "<br>"
        document.getElementById("demo").innerHTML = letter;
    }
    function count_val() {
            //var array = ["a", "e", "i", "o", "u"];
            var input = document.forms["Form"]["input"].value;
            //console.log(input)
            var ans = "";

            for (i = 0; i < array.length; i++) {
                //console.log(input[b])
                b = array[i];
                var a = 0;
                var c;
                var b;
                var d;
                for (c = 0; c < input.length; c++) {
                    //console.log(input[b])
                    d = input[c];
                    if (b == d) {
                        a += 1;
                        //console.log(b, a)
                    }
                }
                ans += b + ":" + " " + a + "<br>" + "<br>";
                document.getElementById("demo").innerHTML = ans;
                console.log(ans)
            }
    }
</script>
```
