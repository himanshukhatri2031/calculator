<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        #result{background-color: white;
        color: black;
    padding: 10px;
margin: 10px;}

        table{
            
    margin-left: 670px;
font-size: 20px;
}
td{
    padding: 5px;

}
#s{
    padding: 10px;
    border-radius: 10px;
    background-color: grey;
    color: white;
    border: 1px solid red;
    
}
#c{
    background-color: red;
    padding: 10px;
    border-radius: 10px;
    color: white;
    border: 1px solid black;
}


h1{text-align: center;}

#img{size: 10px;}


    </style>
</head>
<body>
    
    
    <table>
        
        <h1>Calculator </h1>
        
        <tr >
            
            <td colspan="4"> <input type="text" id="result">
                
            </td>
        </tr>
        <tr>
            <td >
                <input type="button" value="c" onclick="clr()" id="c">
            </td>
            <td>
                <input type="button" value="√" onclick="disp('√')" id="s">
            </td>
            <td>
                <input type="button" value="%" onclick="disp('%')" id="s">
            </td>
            <td>
                <input type="button" value="⌫"
                onclick="cancel()" id="s">
            </td>
        </tr>

        <tr>
            <td>
                <input type="button" value="7" onclick="disp('7')" id="s">
            </td>
            <td>
                <input type="button" value="8" onclick="disp('8')" id="s">
            </td>
            <td>
                <input type="button" value="9" onclick="disp('9')" id="s">
            </td>
            <td>
                <input type="button" value="/" onclick="disp('/')" id="s">
            </td>

        </tr>
        <tr>
            <td>
                <input type="button" value="4" onclick="disp('4')" id="s">
            </td>
            <td>
                <input type="button" value="5" onclick="disp('5')" id="s">
            </td>
            <td>
                <input type="button" value="6" onclick="disp('6')" id="s">
            </td>
            <td>
                <input type="button" value="*" onclick="disp('*')" id="s">
            </td>

        </tr>
        <tr>
            <td>
                <input type="button" value="1" onclick="disp('1')" id="s">
            </td>
            <td>
                <input type="button" value="2" onclick="disp('2')" id="s">
            </td>
            <td>
                <input type="button" value="3" onclick="disp('3')" id="s">
            </td>
            <td>
                <input type="button" value="-" onclick="disp('-')" id="s">
            </td>

        </tr>

        <tr>

            <td>
                <input type="button" value="0" onclick="disp('0')" id="s">
            </td>
            <td>
                <input type="button" value="." onclick="disp('.')" id="s">
            </td>
            <td>
                <input type="button" value="=" onclick="equal()" id="s">
            </td>
            <td>
                <input type="button" value="+" onclick="disp('+')" id="s">
            </td>
        </tr>

    </table>

    <script>
        var x=document.getElementById("result");
        function disp(value)
        {x.value += value; }
        function clr()
        {x.value="";}
        function cancel()
        {
            console.log(x.value.length);
            x.value=x.value.substr(0,x.value.length-1);}
        function equal()
        {x.value= eval(x.value); }
        
        

    </script>
    
</body>
</html>
