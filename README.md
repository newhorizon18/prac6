# Experiment No. 6

## Title: Program Using DOM to Change Background Colour Every 5 Seconds

## 1. Program Code

**File Name: index.html**

```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">

    <title>Background Color Changer</title>

    <style>
        body {
            transition: background-color 1s;
            font-family: Arial, sans-serif;
            text-align: center;
            padding-top: 100px;
        }
    </style>
</head>

<body>

    <h1>
        Background Color Changes Every 5 Seconds
    </h1>

    <script>

        // Array of colors to cycle through
        const colors = [
            '#FF5733',
            '#33FF57',
            '#3357FF',
            '#F1C40F',
            '#9B59B6',
            '#1ABC9C',
            '#E74C3C'
        ];

        let index = 0;

        // Function to change background color
        function changeBackgroundColor() {

            document.body.style.backgroundColor =
                colors[index];

            index = (index + 1) % colors.length;
        }

        // Change color every 5 seconds
        setInterval(changeBackgroundColor, 5000);

    </script>

</body>
</html>
```

## 2. Aim

To write a JavaScript program using the Document Object Model (DOM) to change the background colour of a webpage automatically every 5 seconds.

## 3. Theory

- **DOM:** Allows JavaScript to access and modify HTML elements.
- **JavaScript:** Used to change the webpage dynamically.
- **Array:** Stores multiple background colours.
- **setInterval():** Executes a function repeatedly after a fixed time.
- **backgroundColor:** Changes the background colour of the webpage.
- **5000 Milliseconds:** Equal to 5 seconds.

## 4. Steps to Execute

1. Open Visual Studio Code.
2. Create a file named `index.html`.
3. Paste the program code.
4. Save the file.
5. Open the webpage using Live Server.
6. Observe the background colour changing every 5 seconds.

## 5. Output

The webpage displays:

```text
Background Color Changes Every 5 Seconds
```

After every 5 seconds, the background colour changes automatically.

Example colour sequence:

```text
Orange-Red → Green → Blue → Yellow → Purple
```

The process continues repeatedly.

## 6. Conclusion

Thus, the JavaScript program using DOM was successfully implemented to change the background colour of a webpage automatically every 5 seconds using an array and the setInterval() function.
