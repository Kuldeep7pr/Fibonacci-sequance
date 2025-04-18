<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>Fibonacci Sequence</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.5/dist/css/bootstrap.min.css" rel="stylesheet"/>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.5/dist/js/bootstrap.bundle.min.js"></script>
</head>
<body class="bg-black">
    <h1 class="text-center mt-5 fs-4 font-monospace text-white">This is Fibonacci Sequence</h1>
    <p id="fibonacciSequence" class=" fs-4 rounded-2 w-75 mx-auto text-white border border-white p-3 text-center"></p>

    <script>
        let a = 0, b = 1;
        let output = `${a}, ${b}`

        for (let i = 0; i <= 20; i++) {
            let temp = a + b;
            output += `, ${temp}`;
            a = b;
            b = temp;
        }

        document.getElementById('fibonacciSequence').innerHTML = output;
    </script>
</body>
</html>
