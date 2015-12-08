//subject entry block; suffixA = Analog, suffixD = Digital
int sarwonoA = 20;int sarwonoD = 4;
int karinaA = 10;int karinaD = 10;
int brianA = 30;int brianD = 2;
int titikA = 30;int titikD = 0;
int saraA = 40;int saraD = 20;
int joyceA = 10;int joyceD = 10;
int ericA = 30;int ericD = 15;
int danvuA = 10;int danvuD = 20;
int judyA = 3;int judyD = 5;
int rachelA = 15;int rachelD = 10;
int neighA = 8;int neighD = 0;
int HSA = 0;int HSD = 40;

//total entry per subject. (reverse order)
int sarwonotot = sarwonoA +sarwonoD;
int briantot = brianA + brianD;
int karinatot = karinaA + karinaD;
int titiktot = titikA + titikD;
int saratot = saraA + saraD;
int joycetot = joyceA + joyceD;
int erictot = ericA + ericD;
int danvutot = danvuA + danvuD;
int judytot = judyA + judyD;
int racheltot = rachelA + rachelD;
int neightot = neighA + neighD;
int HStot = HSA + HSD;

//A vs. D calculation
int A = sarwonoA+karinaA+brianA+titikA+saraA+joyceA+ericA+danvuA+judyA+rachelA+neighA+HSA;
int D = sarwonoD+karinaD+brianD+titikD+saraD+joyceD+ericD+danvuD+judyD+rachelD+neighD+HSD;

//circle radius-raw calculation (overlap-mode)
int sarwonoRraw = sarwonotot;
int karinaRraw = karinatot + sarwonotot;
int brianRraw = karinaRraw + briantot;
int titikRraw = brianRraw + titiktot;
int saraRraw = titikRraw + saratot;
int joyceRraw = saraRraw + joycetot;
int ericRraw = joyceRraw + erictot;
int danvuRraw = ericRraw + danvutot;
int judyRraw = danvuRraw + judytot;
int rachelRraw = judyRraw + racheltot;
int neighRraw = rachelRraw + neightot;
int HSRraw = neighRraw + HStot;

//angle-divider calculation block
float sarwonoDiv = map(sarwonoA,0,sarwonotot,0,360);
float karinaDiv = map(karinaA,0,karinatot,0,360);
float brianDiv = map(brianA,0,briantot,0,360);
float titikDiv = map(titikA,0,titiktot,0,360);
float saraDiv = map(saraA,0,saratot,0,360);
float joyceDiv = map(joyceA,0,joycetot,0,360);
float ericDiv = map(ericA,0,erictot,0,360);
float danvuDiv = map(danvuA,0,danvutot,0,360);
float judyDiv = map(judyA,0,judytot,0,360);
float rachelDiv = map(rachelA,0,racheltot,0,360);
float neighDiv = map(neighA,0,neightot,0,360);
float HSDiv = map(HSA,0,HStot,0,360);

//circle radius-map calculation (overlap-mode)
float sarwonoRmap = map(sarwonoRraw,0,HSRraw,50,800);
float karinaRmap = map(karinaRraw,0,HSRraw,50,800);
float brianRmap = map(brianRraw,0,HSRraw,50,800);
float titikRmap = map(titikRraw,0,HSRraw,50,800);
float saraRmap = map(saraRraw,0,HSRraw,50,800);
float joyceRmap = map(joyceRraw,0,HSRraw,50,800);
float ericRmap = map(ericRraw,0,HSRraw,50,800);
float danvuRmap = map(danvuRraw,0,HSRraw,50,800);
float judyRmap = map(judyRraw,0,HSRraw,50,800);
float rachelRmap = map(rachelRraw,0,HSRraw,50,800);
float neighRmap = map(neighRraw,0,HSRraw,50,800);
float HSRmap = map(HSRraw,0,HSRraw,50,800);

void setup(){
  size(900, 900);
  noLoop();
  //noStroke();
}

void draw(){
  //circle reference. (450,450) size 800x800total
  //order:fill/resetradius-fill/analog-fill/digital, repeat
  println("HORRIBU:", HSRraw, "/", HStot, "/", HSA, "/", HSD);
  println("SARARmap/Rraw:", saraRraw, "/", saraRmap);
  println("SARADiv:", saraDiv, "/", radians(saraDiv));
  println("SarwonoDiv:", sarwonoDiv, "/", radians(sarwonoDiv));
  println("ANALOG:",A,"/","DIGITAL:",D);
  
  //c2=analog, c1=digital
  int c1 = 120;
  color c2 = #FFCC00;

  fill(c2);
  arc(450,450,HSRmap,HSRmap,radians(0),radians(HSDiv),PIE);
  fill(c1);
  arc(450,450,HSRmap,HSRmap,radians(HSDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,neighRmap,neighRmap);
  fill(c2);
  arc(450,450,neighRmap,neighRmap,radians(0),radians(neighDiv),PIE);
  fill(c1);
  arc(450,450,neighRmap,neighRmap,radians(neighDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,rachelRmap,rachelRmap);
  fill(c2);
  arc(450,450,rachelRmap,rachelRmap,radians(0),radians(rachelDiv),PIE);
  fill(c1);
  arc(450,450,rachelRmap,rachelRmap,radians(rachelDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,judyRmap,judyRmap);
  fill(c2);
  arc(450,450,judyRmap,judyRmap,radians(0),radians(judyDiv),PIE);
  fill(c1);
  arc(450,450,judyRmap,judyRmap,radians(judyDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,danvuRmap,danvuRmap);
  fill(c2);
  arc(450,450,danvuRmap,danvuRmap,radians(0),radians(danvuDiv),PIE);
  fill(c1);
  arc(450,450,danvuRmap,danvuRmap,radians(danvuDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,ericRmap,ericRmap);
  fill(c2);
  arc(450,450,ericRmap,ericRmap,radians(0),radians(ericDiv),PIE);
  fill(c1);
  arc(450,450,ericRmap,ericRmap,radians(ericDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,joyceRmap,joyceRmap);
  fill(c2);
  arc(450,450,joyceRmap,joyceRmap,radians(0),radians(joyceDiv),PIE);
  fill(c1);
  arc(450,450,joyceRmap,joyceRmap,radians(joyceDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,saraRmap,saraRmap);
  fill(c2);
  arc(450,450,saraRmap,saraRmap,radians(0),radians(saraDiv),PIE);
  fill(c1);
  arc(450,450,saraRmap,saraRmap,radians(saraDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,titikRmap,titikRmap);
  fill(c2);
  arc(450,450,titikRmap,titikRmap,radians(0),radians(titikDiv),PIE);
  fill(c1);
  arc(450,450,titikRmap,titikRmap,radians(titikDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,brianRmap,brianRmap);
  fill(c2);
  arc(450,450,brianRmap,brianRmap,radians(0),radians(brianDiv),PIE);
  fill(c1);
  arc(450,450,brianRmap,brianRmap,radians(brianDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,karinaRmap,karinaRmap);
  fill(c2);
  arc(450,450,karinaRmap,karinaRmap,radians(0),radians(karinaDiv),PIE);
  fill(c1);
  arc(450,450,karinaRmap,karinaRmap,radians(karinaDiv),radians(360),PIE);
  
  fill(255);
  ellipse(450,450,sarwonoRmap,sarwonoRmap);
  fill(c2);
  arc(450,450,sarwonoRmap,sarwonoRmap,radians(0),radians(sarwonoDiv),PIE);
  fill(c1);
  arc(450,450,sarwonoRmap,sarwonoRmap,radians(sarwonoDiv),radians(360),PIE);
 
  fill(255);
  ellipse(450,450,50,50);
  
  fill(c2);
  rect(0,0,10,A);
  fill(c1);
  rect(10,0,10,D);
}
