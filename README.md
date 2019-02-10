
function setup() {
  createCanvas(400, 400);
}

function draw() {
  var leftLineX = 260;
  var rightLineX = 120;
  var middleLineY = 150;
  var bottomLineY = 280;

  background(240);
  noStroke();
  strokeCap(SQUARE);

  fill(100, 200,300); // Red
  rect(leftLineX, 0, width-leftLineX, middleLineY); // small rectangle

  fill(50,100, 300); // Blue
  rect(0, middleLineY, leftLineX, height-middleLineY); // large blue rectangle

  fill(0, 200, 100, 100);  // Yellow
  rect(rightLineX, bottomLineY, width-rightLineX, height-bottomLineY); // green rectangle

  stroke(0); // Black
  strokeWeight(25);
  line(0, middleLineY, width, middleLineY); // middle horizontal
  line(leftLineX, 0, leftLineX, height); // left vertical
  line(rightLineX, middleLineY, rightLineX, height); // right vertical

  strokeWeight(10);
  line(rightLineX, bottomLineY, width, bottomLineY); // bottom horizontal

}
