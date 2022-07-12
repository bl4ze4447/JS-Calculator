# JS-Calculator
A calculator made in JavaScript/HTML/CSS

A calculator that can handle basic arithmetic operations like:
  - Addition
  - Substraction
  - Multiplication
  - Division
  - Square roots
  - Exponentiation	
  

>![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)  
  ```
  function loadItems(){
    sessionStorage.setItem("num1", "");
    sessionStorage.setItem("num2", "");
    sessionStorage.setItem("operation", "");
    sessionStorage.setItem("waitForInp", "y");
    sessionStorage.setItem("waitForInp2", "y");
    sessionStorage.setItem("num1Dot", "n");
    sessionStorage.setItem("num2Dot", "n");
}
window.onload(loadItems());

function cargusRadioactivus(){
    window.onclick = ev => {
    let num1 = sessionStorage.getItem("num1");
    let num2 = sessionStorage.getItem("num2");
    let op = sessionStorage.getItem("operation");
    let waitForInp = sessionStorage.getItem("waitForInp");
    let waitForInp2 = sessionStorage.getItem("waitForInp2");
    let dot1 = sessionStorage.getItem("num1Dot");
    let dot2 = sessionStorage.getItem("num2Dot");
    // Cifra numar 1
    if(ev.target.id == "1" && op == "" && num1 == ""){
        num1 = "1";
    }
    else if(ev.target.id == "2" && op == "" && num1 == ""){
        num1 = "2";
    }
     else if(ev.target.id == "3" && op == "" && num1 == ""){
        num1 = "3";
    }
     else if(ev.target.id == "4" && op == "" && num1 == ""){
        num1 = "4";
    }
     else if(ev.target.id == "5" && op == "" && num1 == ""){
        num1 = "5";
    }
     else if(ev.target.id == "6" && op == "" && num1 == ""){
        num1 = "6";
    }
     else if(ev.target.id == "7" && op == "" && num1 == ""){
        num1 = "7";
    }
     else if(ev.target.id == "8" && op == "" && num1 == ""){
        num1 = "8";
    }
     else if(ev.target.id == "9" && op == "" && num1 == ""){
        num1 = "9";
    }
     else if(ev.target.id == "0" && op == "" && num1 == ""){
        num1 = "0";
    }

    //Operatie
    if(ev.target.id == "+" && op == "" && num1 != ""){
        op = "+";
    }
    else if(ev.target.id == "-" && op == "" && num1 != ""){
        op = "-";
    }
    else if(ev.target.id == "x" && op == "" && num1 != ""){
        op = "x";
    }
    else if(ev.target.id == "%" && op == "" && num1 != ""){
        op = "%";
    }
    else if(ev.target.id == "pow" && op == "" && num1 != ""){
        op = "pow";
    }
    else if(ev.target.id == "sqrt" && op == "" && num1 != ""){
        op = "sqrt";
    }

    // Cifra numar 2
    if(ev.target.id == "1" && op != "" && num2 == ""){
        num2 = "1";
    }
    else if(ev.target.id == "2" && op != "" && num2 == ""){
        num2 = "2";
    }
     else if(ev.target.id == "3" && op != "" && num2 == ""){
        num2 = "3";
    }
     else if(ev.target.id == "4" && op != "" && num2 == ""){
        num2 = "4";
    }
     else if(ev.target.id == "5" && op != "" && num2 == ""){
        num2 = "5";
    }
     else if(ev.target.id == "6" && op != "" && num2 == ""){
        num2 = "6";
    }
     else if(ev.target.id == "7" && op != "" && num2 == ""){
        num2 = "7";
    }
     else if(ev.target.id == "8" && op != "" && num2 == ""){
        num2 = "8";
    }
     else if(ev.target.id == "9" && op != "" && num2 == ""){
        num2 = "9";
    }
     else if(ev.target.id == "0" && op != "" && num2 == ""){
        num2 = "0";
    }

    // Adaugare cifra dupa numar 1
    if(ev.target.id == "1" && op == "" && num1 != "" && waitForInp == "n"){
        num1 += "1";
    }
    else if(ev.target.id == "2" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "2";
    }
     else if(ev.target.id == "3" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "3";
    }
     else if(ev.target.id == "4" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "4";
    }
     else if(ev.target.id == "5" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "5";
    }
     else if(ev.target.id == "6" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "6";
    }
     else if(ev.target.id == "7" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "7";
    }
     else if(ev.target.id == "8" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "8";
    }
     else if(ev.target.id == "9" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "9";
    }
     else if(ev.target.id == "0" && op == "" && num1 != ""&& waitForInp == "n"){
        num1 += "0";
    }

    // Adaugare cifra dupa numar 2
    if(ev.target.id == "1" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "1";
    }
    else if(ev.target.id == "2" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "2";
    }
     else if(ev.target.id == "3" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "3";
    }
     else if(ev.target.id == "4" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "4";
    }
     else if(ev.target.id == "5" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "5";
    }
     else if(ev.target.id == "6" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "6";
    }
     else if(ev.target.id == "7" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "7";
    }
     else if(ev.target.id == "8" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "8";
    }
     else if(ev.target.id == "9" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "9";
    }
     else if(ev.target.id == "0" && op != "" && num2 != ""&& waitForInp2 == "n"){
        num2 += "0";
    }

    // Adaugare punct numar 1
    if(ev.target.id == "." && op == "" && num1 != "" && dot1 == "n"){
        num1 += ".";
        dot1 = "y";
    }

    //Adaugare punct numar 2
    else if(ev.target.id == "." && op != "" && num2 != "" && dot2 == "n"){
        num2 += ".";
        dot2 = "y";
    }

    // Calcul
    if(num2 != "" && ev.target.id == "="){
        let Num1 = Number.parseFloat(num1, 10);
        let Num2 = Number.parseFloat(num2, 10);
        if(op == "%"){
            Num1 = Num1/Num2;
        }
        else if(op == "x"){
            Num1 = Num1*Num2;
        }
        else if(op == "-"){
            Num1 = Num1-Num2;
        }
        else if(op == "+"){
            Num1 = Num1+Num2;
        }
        else if(op == "pow"){
            Num1 = Math.pow(Num1, Num2);
        }
        else if(op == "sqrt"){
            Num1 = Math.sqrt(Num1);
        }
        if(op != "pow"){
        document.querySelector(".lastOp").innerHTML = document.querySelector(".number").innerHTML + " =";}
        else{
            document.querySelector(".lastOp").innerHTML = num1 + num2.sup() + " =";
        }
        op = "";
        num2 = "";
        num1 = Num1 + "";
        waitForInp2 = "y";
        dot2 = "n";
        if(!(num1.includes("."))){
            dot1 = "n";
        }
        document.querySelector(".number").innerHTML = "";
    }
    else if(op == "sqrt"){
        let Num1 = Number.parseFloat(num1, 10);
        Num1 = Math.sqrt(Num1);
        document.querySelector(".lastOp").innerHTML = "√" + document.querySelector(".number").innerHTML + " =";
        op = "";
        num2 = "";
        num1 = Num1 + "";
        waitForInp2 = "y";
        dot2 = "n";
        if(!(num1.includes("."))){
            dot1 = "n";
        }
        document.querySelector(".number").innerHTML = "";
    }
    
    // Backspace
    if(ev.target.id == "del"){
        if(op == ""){
            num1 = num1.substring(0, num1.length-1);
        }
        else{
            num2 = num2.substring(0, num2.length-1);
        }
    }

    // Display
    if(num1 != ""){
    document.querySelector(".number").innerHTML = num1;}
    if(op != "" && op != "pow"){
        document.querySelector(".number").innerHTML += " " + op + " ";
    }
    else if(op == "pow"){
        document.querySelector(".number").innerHTML += " ^ ";
    }
    if(num2 != ""){
        document.querySelector(".number").innerHTML += num2;
    }

    // waitForInp1
    if(num1 != ""){
    waitForInp = "n";
    }
    // Verificare waitForInp2
    if(num2 != ""){
        waitForInp2 = "n";
    }

    // Clear
    if(ev.target.id == "c"){
        num1 = "";
        num2 = "";
        dot1 = "n";
        dot2 = "n";
        waitForInp = "y";
        waitForInp2 = "y";
        op = "";
        document.querySelector(".lastOp").innerHTML = "0 + 0 =";
        document.querySelector(".number").innerHTML = "0";
    }

    // Valori de sesiune
    sessionStorage.setItem("num1Dot", dot1);
    sessionStorage.setItem("num2Dot", dot2);
    sessionStorage.setItem("waitForInp", waitForInp);
    sessionStorage.setItem("waitForInp2", waitForInp2);
    sessionStorage.setItem("num1", num1);
    sessionStorage.setItem("num2", num2);
    sessionStorage.setItem("operation", op);
}
}
```
