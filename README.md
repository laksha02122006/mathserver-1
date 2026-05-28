# Ex.05 Design a Website for Server Side Processing
# Date: 28/05/2026
# Name: V.B.Laksha
# Reg.no: 212224220051
# AIM:
To design a website to calculate the power of a lamp filament in an incandescent bulb in the server side.

# FORMULA:
P = I2R
P --> Power (in watts)
 I --> Intensity
 R --> Resistance

# DESIGN STEPS:
## Step 1:
Clone the repository from GitHub.

## Step 2:
Create Django Admin project.

## Step 3:
Create a New App under the Django Admin project.

## Step 4:
Create python programs for views and urls to perform server side processing.

## Step 5:
Create a HTML file to implement form based input and output.

## Step 6:
Publish the website in the given URL.

# PROGRAM :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GST Bill Calculator</title>

    <style>
        body{
            font-family: Arial, sans-serif;
            background: linear-gradient(to right, #74ebd5, #ACB6E5);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .container{
            background-color: white;
            padding: 30px;
            width: 400px;
            border-radius: 15px;
            box-shadow: 0px 0px 15px gray;
            text-align: center;
        }

        h1{
            color: darkblue;
            margin-bottom: 20px;
        }

        input{
            width: 90%;
            padding: 10px;
            margin: 10px 0;
            border-radius: 5px;
            border: 1px solid gray;
            font-size: 16px;
        }

        button{
            background-color: green;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }

        button:hover{
            background-color: darkgreen;
        }

        .result{
            margin-top: 20px;
            background-color: #f2f2f2;
            padding: 15px;
            border-radius: 10px;
        }

        p{
            font-size: 18px;
        }

        .footer{
            margin-top: 20px;
            font-size: 16px;
            color: darkblue;
            font-weight: bold;
        }
    </style>
</head>

<body>

    <div class="container">

        <h1>GST Bill Calculator</h1>

        <input type="number" id="amount" placeholder="Enter Product Amount">

        <input type="number" id="gst" placeholder="Enter GST Percentage">

        <br><br>

        <button onclick="calculateGST()">Calculate</button>

        <div class="result" id="output">

            <p>GST Amount : ₹ 0</p>

            <p>Total Amount : ₹ 0</p>

        </div>

        <div class="footer">
            Created By V.B.Laksha
        </div>

    </div>

    <script>

        function calculateGST(){

            let amount = parseFloat(document.getElementById("amount").value);

            let gst = parseFloat(document.getElementById("gst").value);

            let gstAmount = (amount * gst) / 100;

            let total = amount + gstAmount;

            document.getElementById("output").innerHTML = `
                <p>Original Amount : ₹ ${amount}</p>
                <p>GST (${gst}%) : ₹ ${gstAmount}</p>
                <p><strong>Total Amount : ₹ ${total}</strong></p>
            `;
        }

    </script>

</body>
</html>
```
# SERVER SIDE PROCESSING:
<img width="1118" height="273" alt="image" src="https://github.com/user-attachments/assets/3d6e654f-bddc-4058-80dc-39e16687c728" />
# HOMEPAGE:
<img width="1919" height="1081" alt="Screenshot 2026-05-28 215736" src="https://github.com/user-attachments/assets/a74753eb-e952-4eaf-9b59-8f33edda37f1" />
<img width="1919" height="1085" alt="Screenshot 2026-05-28 215759" src="https://github.com/user-attachments/assets/9693fed6-119e-42f7-8958-eecd9b4821e0" />

# RESULT:
The program for performing server side processing is completed successfully.
