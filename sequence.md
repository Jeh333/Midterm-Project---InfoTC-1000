<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Fibonacci Sequence</title>


 <input type text="text" id="txtloop" />
        <input type="button" id="btnEnter" value="Enter" onclick="fibonacci_series(txtloop.value)" />

        <p id="output"></p>
<p id="demo"></p>

<script> 
    var fibonacci_series = function (n) 
    {
    if (n==1) 
    {
    var loop = [0, 1];
    document.getElementById("output").innerHTML = loop;
    return loop;
    } 
    else 
    {
        var s = fibonacci_series(n - 1);
        s.push(s[s.length - 1] + s[s.length - 2]);
        document.getElementById("output").innerHTML =s;
        return s;
    }
    
    };


</script>

</head>

<body onload="fibonacci_series()">
<div id="display">

</div>
</body>

</html>