# Assignment 5
## 1.HTML
'''
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Webpage Design</title>
    <link rel="stylesheet" href="style.css">
    <script src='https://kit.fontawesome.com/a076d05399.js' crossorigin='anonymous'></script>
</head>
<body>
    <h1>Calculator</h1>
    <div class="main">
    <div class="cal">
        <div class="inp">
            <input class="inp" type="text" placeholder="0" id="dis">
        </div>
        <div class="grid-container">
            <div class="item1"><button type="button" onclick="cler()">AC</button></div>
            <div class="item2"><button type="button" onclick="del()">DEL</button></div>
            <div class="item3"><button type="button" onclick="display('.')">.</button></div>  
            <div class="item4"><button type="button" onclick="display('/')">/</button></div>
            <div class="item5"><button type="button" onclick="display(7)">7</button></div>
            <div class="item6"><button type="button" onclick="display(8)">8</button></div>
            <div class="item7"><button type="button" onclick="display(9)">9</button></div>
            <div class="item8"><button type="button" onclick="display('*')">*</button></div>  
            <div class="item9"><button type="button" onclick="display(4)">4</button></div>
            <div class="item10"><button type="button" onclick="display(5)">5</button></div>
            <div class="item11"><button type="button" onclick="display(6)">6</button></div>  
            <div class="item12"><button type="button" onclick="display('-')">-</button></div>
            <div class="item13"><button type="button" onclick="display(1)">1</button></div>
            <div class="item14"><button type="button" onclick="display(2)">2</button></div>
            <div class="item15"><button type="button" onclick="display(3)">3</button></div>
            <div class="item16"><button type="button" onclick="display('+')">+</button></div>  
            <div class="item17"><button type="button" onclick="display('%')">%</button></div>
            <div class="item18"><button type="button" onclick="display('0')">0</button></div>
            <div class="item19"><button type="button" onclick="result()">=</button></div> 
          </div>

    </div>
    <script>
        let outputdis=document.getElementById("dis");
        function display(num){
            outputdis.value+=num;
        }
        function result(){
            try{
                outputdis.value=eval(outputdis.value);
            }
            catch(err){
                alert("Invalid");
            }
        }
        function del(){
            outputdis.value=outputdis.value.slice(0,-1);
        }
        function cler(){
            outputdis.value="";
        }
    </script>
    </div>
</body>
</html>

'''
## Style.css
'''
.main{
    display: flex;
    justify-content: center;
    align-items: center;
    padding-top: 200px;
}
h1{
    text-align: center;
}
.cal{
    height: 400px;
    width: 350px;
    background-color: aquamarine;
    padding: 25px;
    border: 1px solid;
}
.inp{
    width: 345px;
    height: 100px;
    font-size: 50px;
    text-align: right;
    /* margin-right: 40px; */
}
.grid-container{
    display: grid;
    width: 100%;
    grid-template-columns: auto auto auto auto;
    gap: 10px;
    
    padding-top: 10px;
}
.grid-container>div{
    /* background-color: rgba(255, 255, 255, 0.8); */
  text-align: center;
  /* padding: 20px 0; */
  height: 50px;
  width: auto;
  font-size: 20px;
}
.item19 {
    grid-column:span 2;
  }
button{
    width: 100%;
    height: 100%;
}
'''

## Output
![image](https://github.com/manojvenaram/Calculatorjavascript/assets/94165064/4bbe1d1a-ba10-4ed1-8502-6880fe36095a)
![image](https://github.com/manojvenaram/Calculatorjavascript/assets/94165064/c720947d-7b31-4e2e-9ab6-04ff0bc87081)

