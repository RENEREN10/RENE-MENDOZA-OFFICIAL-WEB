# RENE-MENDOZA-OFFICIAL-WEB
Esta es mi primera pagina web: https://reneren10.github.io/RENE-MENDOZA-OFFICIAL-WEB/.
var r1 = 150;
var r2 = 70;
var lineas = 10;
var r3 = 200
var r4 = 70
var tiempoEspera;
var tiempoInicio;
var onOff = false
var velocidadRot = 1;
var r5 = 500
var r6 = 80
var r7 = 100
var r8 = 20
var angulo = 0.0
var r12 = 90
var r13 = 300


function setup() {
	createCanvas(windowWidth, windowHeight);
	frameRate(6);

	tiempoInicio = 5;
	tiempoEspera = 0
}

function draw() {

	if (width > height) {
		background(0);

		textAlign(CENTER);
		textSize(r5 / 8);
		noStroke();
		fill(202, 250, 0);
		//text("SANTIAGO",width/2,height/2);
		translate(width / 2, height / 2);

		if (millis() - tiempoInicio > tiempoEspera) {
			tiempoInicio = millis();
			if (onOff == true) {
				onOff = false;
				tiempoEspera = 100;

				velocidadRot = velocidadRot - 1;

				for (let i = 0; i < lineas; i += 1) {
					let x1
					let y1
					let x2
					let y2;

					if (i % 1 == 0) {
						x1 = (r13) * cos(i * 2 * PI / lineas + velocidadRot);
						y1 = (r12) * sin(i * 2 * PI / lineas + velocidadRot);
						x2 = (r13) * cos(i * 2 * PI / lineas + velocidadRot);
						y2 = (r12) * sin(i * 2 * PI / lineas + velocidadRot);
					}




					textAlign(CENTER);
					textSize(r5 / 8);
					noStroke();
					fill(random(33, 250));
					text("UwU", x1 * 180, y1 / 100);
					fill((random(33, 250)));
					text("UwU", x1 * 50, y1 / 10);
					//translate(width / 2, height / 2);





					for (let i = 0; i < lineas; i += 1) {
						let x1
						let y1
						let x2
						let y2;

						if (i % 1 == 0) {
							x1 = (r13) * cos(i * 2 * PI / lineas + velocidadRot);
							y1 = (r8) * sin(i * 10 * 0 * PI / lineas + velocidadRot);
							x2 = (r13) * cos(i * 2 * PI / lineas + velocidadRot);
							y2 = (r8) * sin(i * 2 * PI / lineas + velocidadRot);
						}

						textAlign(CENTER);
						textSize(x1, y1, x2, y2);
						noStroke();
						fill((random(33, 250)));
						text("UwU", x1, y1, x2 + 111, y2);





						noStroke();
						//strokeWeight(10);
						//stroke(10);
						fill(225, 23, 32, )
						rect(x1, y1, x2, y2);






					}

				}


			} else {
				onOff = true;
			}
		}
		if (onOff == true) { // ON
			tiempoEspera = 0;
			background(0);



			//rotate(angulo);
			//angulo = angulo + 0.3 

			velocidadRot = velocidadRot - 1;

			for (let i = 0; i < lineas; i += 1) {
				let x1
				let y1
				let x2
				let y2;

				if (i % 1 == 0) {
					x1 = (r1) * cos(i * 2 * PI / lineas + velocidadRot);
					y1 = (r6) * sin(i * 2 * PI / lineas + velocidadRot);
					x2 = (r2) * cos(i * 2 * PI / lineas + velocidadRot);
					y2 = (r1) * sin(i * 2 * PI / lineas + velocidadRot);
				}







				noStroke();
				//strokeWeight(10);
				//stroke(10);
				fill(100, 23, 32, )
				rect(x1, y1, x2, y2);



			}

			for (let i = 0; i < lineas; i += 1) {
				let x1
				let y1
				let x2
				let y2;

				if (i % 1 == 0) {
					x1 = (r5) * cos(i * 10 * PI / lineas + velocidadRot);
					y1 = (r7) * sin(i * 2 * PI / lineas + velocidadRot);
					x2 = (r5) * cos(i * 2 * PI / lineas + velocidadRot);
					y2 = (r7) * sin(i * 10 * 0 / lineas + velocidadRot);
					noStroke();
					//strokeWeight(10);
					//stroke(10);
					fill(33, 23, 32, )
					rect(x1, y1, x2, y2);

					if (i % 1 == 0) {
						x1 = (r7) * cos(i * 2 * PI / lineas + velocidadRot);
						y1 = (r7) * sin(i * 10 * PI / lineas + velocidadRot);
						x2 = (r1) * cos(i * 10 * 0 * lineas + velocidadRot);
						y2 = (r7) * sin(i * 10 * 0 / lineas + velocidadRot);

					}

					noStroke();
					//strokeWeight(10);
					//stroke(10);
					fill(33, 23, 32, )
					rect(x1 / 100, y1 / 10, x2 + 3, y2 / 100);

					/*textAlign(CENTER);
	textSize(x1, y1, x2, y2);
	noStroke();
	fill((random(33,225,33)));
	text("SANTIAGO",x1, y1, x2+111, y2);   */




				}
			}
		}


	}else{
		ellipse(width/2,height/2,100,100);
	}
}
