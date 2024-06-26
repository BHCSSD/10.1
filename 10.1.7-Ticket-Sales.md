# 10.1.7-Ticket-Sales
S&T


```javaScript
let event = "Big Fish";
let preSales;
let daySales;
let prePrice = 15;
let dayPrice = 20;
let totalSales;

function setup() {
 createCanvas(600, 400);
 background(150,50,50);
 textSize(18);
 preSales = 200;
 //daySales = window.prompt("How many tix did we sell today?");
 // window.alert("Total tickets sold is "           );
}

function draw() {
  background(150,250,250);
  textSize(40);
  text(event, 50,50);
  textSize(18);
  text("Presales: "       , 50, 100);
  text("Price $"          , 200, 100);
  
  text("Today sales: "         50, 125);
  text("Price $"              200, 125);
  
 // totalSales = 
  text("Our total is $" + totalSales,50,200);
  
}

function keyPressed(){
  daySales++;
}

```
