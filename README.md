#java script
<!DOCTYPE html>
<html>
<head>
    <title>Online Calculator</title>
    <style>
        table {
            margin: auto;
            border-collapse: collapse;
        }
        input[type=text] {
            width: 100%;
            text-align: right;
            font-size: 2em;
        }
        button {
            width: 100%;
            height: 50px;
            font-size: 1.5em;
        }
    </style>
</head>
<body>
    <table>
        <tr>
            <td colspan="4"><input type="text" id="screen" readonly></td>
        </tr>
        <tr>
            <td><button type="button" onclick="main('1')">1</button></td>
            <td><button type="button" onclick="main('2')">2</button></td>
            <td><button type="button" onclick="main('3')">3</button></td>
            <td><button type="button" onclick="main('+')">+</button></td>
        </tr>
        <tr>
            <td><button type="button" onclick="main('4')">4</button></td>
            <td><button type="button" onclick="main('5')">5</button></td>
            <td><button type="button" onclick="main('6')">6</button></td>
            <td><button type="button" onclick="main('-')">-</button></td>
        </tr>
        <tr>
            <td><button type="button" onclick="main('7')">7</button></td>
            <td><button type="button" onclick="main('8')">8</button></td>
            <td><button type="button" onclick="main('9')">9</button></td>
            <td><button type="button" onclick="main('*')">*</button></td>
        </tr>
        <tr>
            <td><button type="button" onclick="main('0')">0</button></td>
            <td><button type="button" onclick="main('.')">.</button></td>
            <td><button type="button" onclick="calculate()">=</button></td>
            <td><button type="button" onclick="main('/')">/</button></td>
        </tr>
        <tr>
            <td colspan="4"><button type="button" onclick="clearScreen()">C</button></td>
        </tr>
    </table>

    <script>
        function main(key) {
            var screen = document.getElementById("screen");
            screen.value = screen.value + key;
        }

        function calculate() {
            var screen = document.getElementById("screen");
            try {
                screen.value = eval(screen.value);
            } catch (e) {
                screen.value = "Error";
            }
        }

        function clearScreen() {
            document.getElementById("screen").value = "";
        }
    </script>
</body>
</html>

# Online-Calculator
 it's a project to create a simple online calculator using HTML, CSS, and JavaScript.
https://docs.google.com/presentation/d/e/2PACX-1vScx2KoK3LCzfQKk2VqhYExTHDqJjOhaFgrKQF6Jo3LFqWbkZLCdCNvKKhMIpQBOAfNgUcnvvV60Fz9/pub?start=true&loop=true&delayms=3000 
# Online Calculator Project

[Google Slides Presentation]([YOUR_GOOGLE_SLIDES_LINK](https://docs.google.com/presentation/d/e/2PACX-1vScx2KoK3LCzfQKk2VqhYExTHDqJjOhaFgrKQF6Jo3LFqWbkZLCdCNvKKhMIpQBOAfNgUcnvvV60Fz9/pub?start=true&loop=true&delayms=3000 ))
