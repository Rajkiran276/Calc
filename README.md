# Ex.08 Design of a Standard Calculator
## Date:08/05/2024

## AIM:
To design a web application for a standard calculator with minimum five operations.

## DESIGN STEPS:

### Step 1:
Clone the github repository and create Django admin interface.

### Step 2:
Change settings.py file to allow request from all hosts.

### Step 3:
Use CSS for creating attractive colors.

### Step 4:
Write JavaScript program for implementing five different operations.

### Step 5:
Validate the HTML and CSS code.

### Step 6:
Publish the website in the given URL.

## PROGRAM :
```C
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>STANDARD CALCULATOR</title>
    <style>
        .out-container{
            width: 25%;
            margin: auto;
            margin-top: 3rem;
            background-color: rgb(17, 11, 11);
            text-align: center;
            color: white;
            font-weight: bold;
            font-size: 2rem;
            padding: 15px;
            padding-bottom: 30px;
            border-radius: 30px;
            height: 70%;
        }
        .inp{
            width: 90%;
            height: 2rem;
            margin: 5px;
            border-radius: 15px;
            border: none;
        }
        .btn-container{
            display: flex;
            flex-direction: row;
            justify-content: space-around;
        }
        .btn{
            width: 4rem;
            height: 4rem;
            padding: 5px;   
            margin:10px auto;
            cursor: pointer;
            display: grid;
            place-content:center;
            border-radius: 50%;
        }

        .yellow{
            background-color: rgb(255, 81, 0);
            width: 90%;
            margin: 5px auto;
            border-radius: 15px;
            height: 3rem;
        }
        .blue{
            background-color: rgb(45, 4, 252);
        }
        .red{
            background-color: rgb(253, 66, 66);
        }
        .green{
            background-color: rgb(1, 9, 253);
        }
        h5{
            margin: 15px auto;
        }
        .inp{
            font-size: 2rem;
            padding: 10px 5px; 
        }
    </style>
</head>
<body>
    <div class="out-container">
        <h5>RAJKIRAN.J(212222043006)</h5>
        <input type="text" name="" id="inp" class="inp">
        
        <div class="btn-container">
            <div onclick = "fn(this)" class="btn lightblue">(</div>
            <div onclick = "fn(this)" class="btn  lightblue">)</div>
            <div onclick = "fn(this)" class="btn green">C</div>
            <div onclick = "fn(this)" class="btn green" id="green">&lt;</div>
        </div>

        <div class="btn-container">
            <div onclick = "fn(this)" class="btn red">1</div>
            <div onclick = "fn(this)" class="btn red">2</div>
            <div onclick = "fn(this)" class="btn red">3</div>
            <div onclick = "fn(this)" class="btn lightblue">/</div>
        </div>

        <div class="btn-container">
            <div onclick = "fn(this)" class="btn red">4</div>
            <div onclick = "fn(this)" class="btn red">5</div>
            <div onclick = "fn(this)" class="btn red">6</div>
            <div onclick = "fn(this)" class="btn lightblue">*</div>
        </div>

        <div class="btn-container">
            <div onclick = "fn(this)" class="btn red">7</div>
            <div onclick = "fn(this)" class="btn red">8</div>
            <div onclick = "fn(this)" class="btn red">9</div>
            <div onclick = "fn(this)" class="btn lightblue">-</div>
        </div>

        <div class="btn-container">
            <div onclick = "fn(this)" class="btn red">0</div>
            <div onclick = "fn(this)" class="btn red">.</div>
            <div onclick = "fn(this)" class="btn lightblue">%</div>
            <div onclick = "fn(this)" class="btn lightblue">+</div>    
        </div>
        <div class="btn yellow" onclick = "fn(this)">=</div>

    </div>

    <script>
        const fn = (e) => {
            if(e.innerHTML =="="){
                inp.value = eval(inp.value);
            }
            else if(e.innerHTML =="C"){
                inp.value = "";
            }
            else if(e.id=="back"){
                data = inp.value;
                inp.value = data.substring(0,data.length-1);
            }
            else{
                inp.value += e.innerHTML;
            }
        }
    </script>
</body>
</html>
```

## OUTPUT:
![Screenshot (55)](https://github.com/Rajkiran276/Calc/assets/147471453/39c78d31-5849-43f4-b3ca-d58ee2289b15)
![Screenshot (56)](https://github.com/Rajkiran276/Calc/assets/147471453/164d9ec4-620e-4103-af0b-8fadac5e80ae)


## RESULT:
The program for designing a standard calculator using HTML and CSS is executed successfully.
