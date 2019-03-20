# RENE-MENDOZA-OFFICIAL-WEB
Esta es mi primera pagina web
var img;

function preload(){
	img = loadImage("infinito.png");
}

function setup() {
	createCanvas(windowWidth, windowHeight);
	background(255);
}

function draw() {
		image(img, 500, 30);
	 	
		rect(20, 20, 5, 100);
		strokeWeight(10);
		strokeCap(SQUARE);
		stroke(0);
	
		rect(30, 20, 100, 5);
		strokeWeight(10);
		strokeCap(SQUARE);
		stroke(0);
	
		rect(1230, 20, 100, 5);
		strokeWeight(10);
		strokeCap(SQUARE);
		stroke(0);
	
		rect(1330, 20, 5, 100);
		strokeWeight(10);
		strokeCap(SQUARE);
		stroke(0);
	
		rect(1230, 580, 100, 5);
		strokeWeight(10);
		strokeCap(SQUARE);
		stroke(0);
	
		rect(1330, 485, 5, 100);
		strokeWeight(10);
		strokeCap(SQUARE);
		stroke(0);
	
		rect(30, 580, 100, 5);
		strokeWeight(10);
		strokeCap(SQUARE);
		stroke(0);
	
		rect(20, 485, 5, 100);
		strokeWeight(10);
		strokeCap(SQUARE);
		stroke(0);
	
	
	
	
	
	
	
}
