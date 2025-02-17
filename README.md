 
# ບົດລາຍງານ
ວິຊາ: ໄມໂຄຣໂປຣເຊັດເຊີ ແລະ ໄມໂຄຣຄອມພິວເຕີ
ສອນໂດຍ: ອຈ. ປຕ. ລັດທິດາ ຄົມສອນລະສິນ

 ຂຽນໂດຍ: 	
           ທ້າວ ວິລະພົນ ຄໍາວົງທອງ
           ຫ້ອງ 3com2

## ສາລະບານ
ບົດນຳ ........................................................................................................................
ບົດທີ 0 Blink ...............................................................................................................
ບົດທີ 1 Experiment Blink ..............................................................................................
ບົດທີ 2 Switch ............................................................................................................
ບົດທີ 3 RGB ...............................................................................................................
ບົດທີ 4 Buzzer ............................................................................................................
ບົດທີ 5 Potentiometer ..................................................................................................
ບົດທີ 6 Relay ..............................................................................................................
ບົດທີ 7 Servo .............................................................................................................
ບົດທີ 8 Seven Segment ................................................................................................
ບົດທີ 9 Puppy Notify ....................................................................................................
ບົດທີ 10 Scoreboard Display..........................................................................................


# ບົດນຳ

ໄມໂຄຣໂປຣເຊສເຊີ ແລະ ໄມໂຄຣຄອມພີວເຕີ ເປັນອົງປະກອບທີ່ສຳຄັນໃນຄອມພິວເຕີສະໄໝໃໝ່. ລະບົບອັດຕະໂນມັດ ແລະ ລະບົບຝັງຕົວ. ໄມໂຄຣໂປຣເຊສເຊີ (microprocessor) ເຮັດຫນ້າທີ່ເປັນໜ່ວຍປະມວນຜົນກາງ (CPU) ທີ່ປະຕິບັດຄໍາສັ່ງ ແລະ ຄວບຄຸມການເຮັດວຽກຕ່າງໆ. ໄມໂຄຄອມພີວເຕີ (microcomputer) ແມ່ນການປະສົມປະສານຂອງ microprocessor ກັບໜ່ວຍຄວາມຈໍາ ແລະ ອຸປະກອນເສີມເພື່ອເຮັດໃຫ້ມັນປະຕິບັດໜ້າວຽກສະເພາະໃດໜື່ງປະສິດທິພາບ.
ບົດລາຍງານນີ້ໄດ້ສຳຫຼວດການທົດລອງທີ່ສໍາຄັນທີ່ສະແດງໃຫ້ເຫັນເຖິງການເຮັດວຽກພື້ນຖານຂອງ microcontroller ໄດ້. ລວມມີການຄວບຄຸມການປ້ອນຂໍ້ມູນ/ການສົ່ງອອກແບບດິຈິຕອນ. ການເຊື່ອມຕໍ່ເຊັນເຊີ  ແລະ ການສື່ສານກັບອຸປະກອນຕ່າງໆ. ການທົດລອງເຫຼົ່ານີ້ນໍາສະເໜີການໃຊ້ງານຕົວຈິງທີ່ຊ່ວຍໃຫ້ເຂົ້າໃຈການເຮັດວຽກ ແລະ ການປະຍຸກໃຊ້ຂອງ microcontrollers ໃນສະຖານະການຈິງ.
ຫຼັງຈາກຜ່ານການທົດສອບເຫຼົ່ານີ້, ນັກສຶກສາຈະໄດ້ຮັບປະສົບການທາງດ້ານປະຕິບັດຕົວຈິງໃນການເຊື່ອມຕໍ່ໄມໂຄຣຄອນໂທຣອນເລີກັບອຸປະກອນຕ່າງໆ, ການນຳໃຊ້ເຊັນເຊີ ແລະ ການພັດທະນາໂປຣແກຣມ, ເຊິ່ງເປັນພື້ນຖານສຳຄັນໃນການອອກແບບ ແລະ ພັດທະນາລະບົບທີ່ຊັບຊ້ອນຂຶ້ນໃນອະນາຄົດ.







# ບົດທີ 0:Blink

### 1.	ບົດນຳ
o	ຈຸດປະສົງ:
-	ຮຽນຮູ້ໃນການຄວບຄຸມ LED ເປີດ ແລະ ປິດໂດຍໃຊ້ Arduino.
-	ເຂົ້າໃຈຫຼັກການການເຮັດວຽກຂອງຄໍາສັ່ງ digitalWrite() ແລະ delay()
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	LED ໃນຕົວ (ຢູ່ pin 13)
•	Resistant (220 Ω)
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
-	LED: ໃຊ້ໄຟ LED ໃນຕົວຢູ່ pin 13 ຂອງ Arduino.
-	ການສະຫນອງພະລັງງານ: Arduino ສະຫນອງພະລັງງານໃຫ້ກັບວົງຈອນທັງຫມົດ.
 
 
### 4.	ໂຄດທີ່ໃຊ້
```cpp
// C++ code
//
void setup() {
// put your setup code here, to run once:

  pinMode(LED_BUILTIN, OUTPUT); // PIN 13
  
}

void loop() {
// put your main code here, to run repeatedly:
    
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s) = 1 second
  
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s) = 1 second
}
```
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	ກຳນົດ PIN:
-	Pin 13 ຖືກຕັ້ງເປັນ OUTPUT ເພື່ອຄວບຄຸມການເປີດ ແລະປິດ LED.
•	ເປີດ/ປິດ LED:
-	ໃຊ້ຄໍາສັ່ງ digitalWrite(13, HIGH) ເພື່ອເປີດໄຟ LED.
-	ໃຊ້ຄໍາສັ່ງ digitalWrite(13, LOW) ເພື່ອປິດໄຟ LED.
-	ໃຊ້ delay(1000) ເພື່ອລໍຖ້າ 1 ວິນາທີກ່ອນທີ່ຈະເປີດ ຫຼື ປິດ LED.
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/4RfOw8UV7aA-blink



# ບົດທີ 1 :Experiment Blink
 
### 1.	ບົດນຳ
ການທົດລອງ "Blink" ເປັນການແນະນໍາເບື້ອງຕົ້ນກ່ຽວກັບການຂຽນໂປຣແກຣມ microcontroller. ໂດຍການຄວບຄຸມ output ດິຈິຕອລໂດຍການໃຊ້ LEDs, ການທົດລອງນີ້ເປັນພື້ນຖານສໍາລັບຄວາມເຂົ້າໃຈກ່ຽວກັບການຈັດການ pin GPIO.
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	LED
•	Resistor (220 Ω)
•	Jumper wires
•	Breadboard
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
LED ແມ່ນເຊື່ອມຕໍ່ກັບ pin output ໂດຍຜ່ານຕົວຕ້ານທານ. ດ້ວຍຂາລົບທີ່ເຊື່ອມຕໍ່ກັບ GND, Microcontroller Arduino ຈະປ່ຽນສະຖານະຂອງ output ເພື່ອເຮັດໃຫ້ໄຟ LED ກະພິບ.
 
 

### 4.	ໂຄດທີ່ໃຊ້
~~~cpp
// C++ code
void setup() {
// put your setup code here, to run once:

  pinMode(LED_BUILTIN, OUTPUT); // PIN 13  
}

void loop() {
// put your main code here, to run repeatedly:
    
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s) = 1 second
  
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s) = 1 second
}
~~~
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	Arduino ກຳນົດ pin LED ເປັນ output.
•	ໂປຣແກຣມເຂົ້າໄປໃນ loop ຢ່າງຕໍ່ເນື່ອງ.
•	ໄຟ LED ຖືກເປີດໂດຍຕັ້ງ pin output ເປັນ HIGH.
•	Delay 1 ວິນາທີ.
•	ໄຟ LED ຖືກປິດໂດຍການຕັ້ງ pin output ເປັນ LOW.
•	Delay 1 ວິນາທີ.
•	ຂະບວນການນີ້ແມ່ນເຮັດຊ້ໍາຢ່າງບໍ່ມີກໍານົດ, ເຮັດໃຫ້ເກີດໄຟກະພິບ.

### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/5hAXNNXe7D9-exercise-experiment-blink-08-vilaphonh-3com2


# ບົດທີ 2: Switch
 
# 1.	ບົດນຳ
ການທົດລອງ "ສະວິດ" ສະແດງໃຫ້ເຫັນເຖິງການໃຊ້ສະວິດເພື່ອຄວບຄຸມຜົນເອົ້າພຸດເຊັ່ນ: LED ໂດຍໃຊ້ microcontroller. ນີ້ແມ່ນແນວຄວາມຄິດທີ່ສໍາຄັນໃນການຂຽນໂປຣແກຣມ ເນື່ອງຈາກວ່າມັນສະແດງໃຫ້ເຫັນວິທີການອ່ານສະຖານະຂອງ input ທາງກາຍະພາບ ແລະ ຕອບສະຫນອງຕາມຄວາມເຫມາະສົມ.
# 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	Pushbutton (Switch)
•	Resistor (220Ω)
•	Jumper wires
•	Breadboard
# 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
-	ປຸ່ມກົດແມ່ນເຊື່ອມຕໍ່ກັບ pin 2 (ການປ້ອນຂໍ້ມູນດິຈິຕອນ) ຂອງ Arduino.
-	ຂາຫນຶ່ງຂອງປຸ່ມກົດແມ່ນເຊື່ອມຕໍ່ກັບ GND ແລະ ຂາອື່ນແມ່ນເຊື່ອມຕໍ່ກັບ pin 2.
-	LED ແມ່ນເຊື່ອມຕໍ່ກັບ pin LED ໃນຕົວ (ຫຼື pin ດິຈິຕອນອື່ນ) ຜ່ານຕົວຕ້ານທານ. ຂາລົບແມ່ນເຊື່ອມຕໍ່ກັບ GND.
 

 

# 4.	ໂຄດທີ່ໃຊ້
~~~cpp
int buttonState = 0;
void setup()
{
  pinMode(2, INPUT);
  pinMode(LED_BUILTIN, OUTPUT);
  Serial.begin(9600);
}

void loop()
{
  // read the state of the pushbutton value
  buttonState = digitalRead(2);
  // check if pushbutton is pressed.  if it is, the
  // buttonState is HIGH
  if (buttonState == HIGH) {
    // turn LED on
    Serial.println("Button HIGH"); 
    digitalWrite(LED_BUILTIN, HIGH);
  } else {
    // turn LED off
    Serial.println("Button LOW"); 
    digitalWrite(LED_BUILTIN, LOW);
  }
  delay(10); // Delay a little bit to improve simulation performance
}
~~~
## 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	Arduino ເລີ່ມຕົ້ນ pin 2 ເປັນ input ສໍາລັບປຸ່ມກົດ ແລະ pin LED ໃນຕົວເປັນ output.
•	ໂປຣແກຣມເຂົ້າສູ່ loop ແລະ ຕິດຕາມສະຖານະຂອງປຸ່ມກົດຢ່າງຕໍ່ເນື່ອງ.
•	ຖ້າປຸ່ມກົດ (buttonState ແມ່ນສູງ), LED ໃນຕົວຈະເປີດ.
•	ຖ້າປຸ່ມບໍ່ໄດ້ກົດ (buttonState ຕໍ່າ), LED ຈະປິດ.
•	ຂະບວນການນີ້ເຮັດຊ້ຳຢ່າງຕໍ່ເນື່ອງ, ຕອບສະໜອງຕາມສະຖານະຂອງປຸ່ມກົດ.
## 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/2LhPBk9bi9n-switch

## ບົດທີ 3: RGB
 
### 1.	ບົດນຳ
ໃນບົດນີ້, ພວກເຮົາຈະສຶກສາກ່ຽວກັບການຄວບຄຸມ RGB LED ໂດຍໃຊ້ Arduino. LED RGB ປະກອບດ້ວຍ LED 3 ຕົວ (ສີແດງ, ສີຂຽວ ແລະ ສີຟ້າ) ເຊິ່ງສາມາດປະສົມກັນເພື່ອສ້າງສີທີ່ແຕກຕ່າງກັນໂດຍການປັບຄວາມສະຫວ່າງຂອງແຕ່ລະສີ. ເຊິ່ງບົດນີ້ຈະສະແດງໃຫ້ຮູ້ເຖິງວິທີການຄວບຄຸມ RGB LED ໂດຍໃຊ້ຄໍາສັ່ງຈາກ Serial Input ເພື່ອເປີດ ຫຼື ປິດສີຕ່າງໆ ຫຼື ປະສົມສີເຫຼົ່ານີ້ເພື່ອສະແດງສີທີ່ແຕກຕ່າງ.
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	RGB LED (ประเภท Common Cathode หรือ Common Anode)
•	Resistor (220Ω)
•	Jumper wires
•	Breadboard
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
RGB LED ມີ 4 pins ຄື: pin ສໍາລັບແຕ່ລະສີ (ສີແດງ, ສີຂຽວ, ສີຟ້າ) ແລະ pin ສໍາລັບດິນ (ສໍາລັບ Common Cathode) ຫຼື VCC (ສໍາລັບ Common Anode), ແຕ່ລະສີແມ່ນເຊື່ອມຕໍ່ກັບ pin ດິຈິຕອລຂອງ Arduino ໂດຍໃຊ້ຕົວຕ້ານທານໃນວົງຈອນນີ້:
-	Pin 9: ສີແດງ
-	Pin 10: ສີຂຽວ
-	Pin 11: ສີຟ້າ
-	Cathode ທົ່ວໄປ: ເຊື່ອມຕໍ່ກັບ GND
 

 

### 4.	ໂຄດທີ່ໃຊ້
~~~cpp
int ledPins[] = {11, 10, 9};

void setup() {
  // put your setup code here, to run once:
  Serial.begin(9600);
  
  for (int i = 0; i < 3; i++){
    pinMode(ledPins[i], OUTPUT);
  }
  
  //exercise
  //change foreach to for loop
    
}

void loop() {
  // put your main code here, to run repeatedly:
  
  while (Serial.available() > 0) {
    // read input from serial monitor
    String input = Serial.readStringUntil('\n'); // Read until newline
    
    for (int i = 0; i < 3; i++){
      digitalWrite(ledPins[i], LOW);
    }
    delay(10);

    if (input == "on" or input == "rgb" or input == "rbg" or input == "grb" or input == "gbr" or input == "brg" or input == "bgr" ) {
      // turn all LEDs on
      for (int i = 0; i < 3; i++){
        digitalWrite(ledPins[i], HIGH);
      }
    }

    else if (input == "off") {
      // turn all LEDs off
      for (int i = 0; i < 3; i++){
        digitalWrite(ledPins[i], LOW);
      }
    }

    else if (input == "r") {
      digitalWrite(ledPins[0], HIGH);
    }

    else if (input == "g") {
      digitalWrite(ledPins[1], HIGH);
    }

    else if (input == "b") {
      digitalWrite(ledPins[2], HIGH);
    }
    
    else if (input == "rg" or input == "gr") {
      digitalWrite(ledPins[0], HIGH);
      digitalWrite(ledPins[1], HIGH);
    }
    else if (input == "rb" or input == "br") {
      digitalWrite(ledPins[0], HIGH);
      digitalWrite(ledPins[2], HIGH);
    }
    else if (input == "gb" or input == "bg") {
      digitalWrite(ledPins[1], HIGH);
      digitalWrite(ledPins[2], HIGH);
    }
    else {
      allColors();
    }
  }
}
void allColors(){
  //WHITE
  for(int i = 0; i < 3; i++){
        digitalWrite(ledPins[i], HIGH);
  }
  delay(100);
  for(int i = 0; i < 3; i++){
    digitalWrite(ledPins[i], LOW);
  }
  delay(100);

  //RED, GREEN, BLUE
  for(int i = 0; i < 3; i++){
        digitalWrite(ledPins[i], HIGH);
        delay(100);
        digitalWrite(ledPins[i], LOW);
        delay(100);
  }

  //RED + GREEN index 0 and index 1
  for(int i = 0; i < 2; i++){
    digitalWrite(ledPins[i], HIGH);
  }
  delay(100);
  for(int i = 0; i < 2; i++){
    digitalWrite(ledPins[i], LOW);
  }
  delay(100);

  //RED BLUE index 0 and index 2
  for(int i = 0; i < 3; i += 2){
    digitalWrite(ledPins[i], HIGH);
  }
  delay(100);
  for(int i = 0; i < 3; i += 2){
    digitalWrite(ledPins[i], LOW);
  }
  delay(100);

  // GREEN + BLUE index 1 and index 2  
  for(int i = 1; i < 3; i++){
    digitalWrite(ledPins[i], HIGH);
  }
  delay(100);

  for(int i = 1; i < 3; i++){
    digitalWrite(ledPins[i], LOW);
  }
  delay(100);
}
~~~
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	Serial Input: ລະບົບລໍຖ້າການປ້ອນຂໍ້ມູນຈາກ Serial ເຊັ່ນ "on", "off" ຫຼື ຄໍາສັ່ງແຕ່ລະສີເຊັ່ນ "r", "g", "b".
•	ການຄວບຄຸມ LED: ຂຶ້ນກັບຄໍາສັ່ງປ້ອນຂໍ້ມູນ, ລະບົບຈະເປີດ ຫຼື ປິດ LED ທີ່ສອດຄ້ອງກັນເຊັ່ນ: ເມື່ອຄໍາສັ່ງແມ່ນ "r", LED ສີແດງຈະເປີດ.
•	ການປະສົມສີ: ລະບົບສາມາດປະສົມສີໂດຍການເປີດໄຟ LED ຫຼາຍອັນໃນເວລາດຽວກັນ, ຕົວຢ່າງ "rg" ຈະເປີດສີແດງ ແລະ ສີຂຽວ ເຊິ່ງຈະເປັນສີເຫຼືອງ
•	ເອັບເຟັກສີທັງໝົດ: ຟັງຊັ່ນ allColors() ໝູນວຽນຜ່ານສີຕ່າງໆເຊັ່ນ: ສີຂາວ, ສີແດງ, ສີຂຽວ, ສີຟ້າ, ແລະ ການປະສົມຂອງສີເຫຼົ່ານີ້ເພື່ອການສະແດງຜົນແບບຄົບວົງຈອນ.
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/5O6BirnZQfT-rgb
# ບົດທີ 4 :Buzzer

### 1.	ບົດນຳ
ໃນນີ້, ພວກເຮົາຈະໃຊ້ buzzer (ຫຼື ລໍາໂພງ) ເພື່ອສ້າງສຽງທີ່ແຕກຕ່າງກັນໂດຍອີງໃສ່ໂນດດົນຕີ. ພວກເຮົາຈະໃຊ້ຄໍາສັ່ງ tone () ເພື່ອສ້າງສຽງໂດຍອີງໃສ່ຄວາມຖີ່ທີ່ກໍານົດໄວ້.
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	Buzzer
•	Jumper wires
•	Breadboard (ຖ້າຕ້ອງການ)
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
-	ເຊື່ອມຕໍ່ pin buzzer ກັບ pin 9 ຂອງ Arduino.
-	ເຊື່ອມຕໍ່ຂາອື່ນຂອງ buzzer ກັບ GND.
 

### 4.	ໂຄດທີ່ໃຊ້
~~~cpp
// Notes frequencies (in Hz) for different pitches
#define SPEAKER 10
#define BTN 2
#define NOTE_C2 65
#define NOTE_D2 73
#define NOTE_E2 82
#define NOTE_F2 87
#define NOTE_G2 98
#define NOTE_A2 110
#define NOTE_B2 123

#define NOTE_C3 130
#define NOTE_D3 146
#define NOTE_E3 164
#define NOTE_F3 174
#define NOTE_G3 196
#define NOTE_A3 220
#define NOTE_B3 246

#define NOTE_C4 261
#define NOTE_D4 293
#define NOTE_E4 329
#define NOTE_F4 349
#define NOTE_G4 392
#define NOTE_A4 440
#define NOTE_B4 493


// Melody notes and durations
int melody[] = {
NOTE_C3, NOTE_F3, NOTE_G3, NOTE_A3, 
NOTE_G3, NOTE_F3, NOTE_A3, NOTE_G3,
NOTE_A3, NOTE_B3, NOTE_C4, NOTE_A3,
NOTE_C4, NOTE_B3, NOTE_A3, NOTE_B3,
NOTE_C4, NOTE_B3, NOTE_A3, NOTE_G3,
NOTE_E3, NOTE_D3, NOTE_E3, NOTE_F3,
NOTE_G3, NOTE_E3, NOTE_C3, NOTE_D3, 
NOTE_G2, NOTE_C3, NOTE_D3, NOTE_E3,
NOTE_F3, NOTE_G3, NOTE_F3, NOTE_A3,
NOTE_G3, NOTE_F3, NOTE_E3, NOTE_D3,
NOTE_C3, NOTE_D3, NOTE_E3, NOTE_F3,
NOTE_E3, NOTE_E3, NOTE_D3, NOTE_C3,
NOTE_D3, NOTE_E3, NOTE_G3, NOTE_E3,
NOTE_D3, NOTE_C3, NOTE_C4, NOTE_C4,
NOTE_A3, NOTE_G3, NOTE_A3, NOTE_C4,
NOTE_A3, NOTE_A3, NOTE_D4, NOTE_C4,
NOTE_A3, NOTE_G3, NOTE_E3, NOTE_G3,
NOTE_E3, NOTE_D3, NOTE_C3, NOTE_C3,
NOTE_C3, NOTE_C3, NOTE_C3, NOTE_D3,
NOTE_E3, NOTE_D3, NOTE_C3, NOTE_G3,
NOTE_G3, NOTE_G3, NOTE_G3, NOTE_E3,
NOTE_G3, NOTE_A3, NOTE_B3, NOTE_A3,
NOTE_G3, NOTE_E3, NOTE_A3, NOTE_G3,
NOTE_E3, NOTE_D3, NOTE_C3, NOTE_A2,
NOTE_G2, NOTE_A2, NOTE_C3
};
int noteDurations[] = {
  2, 2, 4, 2, 
  2, 2, 4, 2,
  2, 2, 4, 2, 
  2, 1, 2, 2,
  2, 2, 2, 2,
  4, 2, 2, 2,
  2, 2, 2, 1,
  2, 2, 3, 2,
  2, 1, 2, 2,
  2, 2, 2, 1,
  2, 2, 2, 2,
  2, 2, 3, 2,
  2, 2, 2, 2,
  2, 1, 2, 2,
  2, 3, 3, 2,
  2, 2, 2, 2,
  2, 2, 2, 1,
  3, 2, 2, 3,
  3, 3, 2, 3,
  2, 2, 2, 2,
  2, 1, 2, 2,
  2, 3, 3, 2,
  2, 2, 2, 2,
  2, 2, 2, 2,
  2, 2, 1, 
};
int btnState = 0;

void setup() {  
  Serial.begin(9600);
  pinMode(SPEAKER, OUTPUT);
  pinMode(LED_BUILTIN, OUTPUT);
  pinMode(BTN, INPUT);
}

void loop() {
   btnState = digitalRead(BTN);
  Serial.println(btnState);
    
  if(btnState == HIGH){   
    delay(500); 
    
    digitalWrite(LED_BUILTIN, HIGH);
    }
  for (int i = 0; i < 200; i++) {
    int noteDuration = 1000 / noteDurations[i]; // Note duration in milliseconds
    tone(9, melody[i], noteDuration);          // Play the note on pin 8
    delay(noteDuration * 1.3);                 // Pause between notes
    noTone(8);                                 // Stop the tone
  }
  
  delay(2000); // Pause before repeating the melody
}
~~~
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	ການຫຼິ້ນ Melody: ໃຊ້ຟັງຊັນ tone() ເພື່ອຫຼິ້ນໂນດທີ່ແຕກຕ່າງກັນຜ່ານ buzzer ທີ່ເຊື່ອມຕໍ່ກັບ pin 9 ຂອງ Arduino, ຄວາມຖີ່ຂອງໂນດແມ່ນຖືກກໍານົດຕາມພາລາມິເຕີທີ່ລະບຸ ແລະ ຄວາມຍາວຂອງໂນດແມ່ນຄວບຄຸມໂດຍຜ່ານ array noteDurations[].
•	ການຢຸດສຽງ: ຟັງຊັນ noTone() ຖືກນໍາໃຊ້ເພື່ອຢຸດສຽງເມື່ອໂນດໄດ້ສໍາເລັດການຫຼິ້ນ ແລະ ຈະມີ(delay()) ເພື່ອໃຫ້ທຸກໆໂນດມີເວລາຢຸດທີ່ເຫມາະສົມ.
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/hhq0lSBndlC-national-antheme









# ບົດທີ 5 :Potentiometer

### 1.	ບົດນຳ
Potentiometer ຫຼື ຕົວປັບແຮງດັນແມ່ນຕົວຕ້ານທານທີ່ສາມາດປັບໄດ້, ສາມາດເຊື່ອມໂຍງກັບຄ່າຕ່າງໆເຊັ່ນ: ການຄວບຄຸມຄວາມສະຫວ່າງຂອງ LED ຫຼື ຄວາມໄວຂອງມໍເຕີ, ຂຶ້ນຢູ່ກັບການປັບຂອງຜູ້ໃຊ້. ການທົດລອງນີ້ຈະແນະນໍາວິທີການອ່ານຈາກອະນາລັອກ ແລະ ວິທີການໃຊ້ງານ ເພື່ອຄວບຄຸມການດໍາເນີນງານໃນແອັບພິເຄຊັ່ນຕ່າງໆ.
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	Potentiometer 
•	LED
•	Resistor (220Ω)
•	Jumper wires
•	Breadboard
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
o	ເຊື່ອມຕໍ່ potentiometer ກັບ Arduino ດັ່ງຕໍ່ໄປນີ້:
-	ຂາ potentiometer ຊ້າຍໄປຫາ 5V ໃນ Arduino.
-	ຂາ potentiometer ຂວາໄປຫາ GND.
-	pin ກາງ (wiper) ຂອງ potentiometer ແມ່ນເຊື່ອມຕໍ່ກັບ Analog A0 pin ຂອງ Arduino.
o	ເຊື່ອມຕໍ່ LED ກັບ pin 11 ໃນ Arduino.
-	ຂາຍາວ (Anode pin) ຂອງ LED ໄປກັບ pin 11.
-	ຂາສັ້ນ (ຂາ Cathode) ຂອງ LED ໂດຍຜ່ານ 220Ω resistor ຕໍ່ກັບ GND.
 

 
### 4.	ໂຄດທີ່ໃຊ້
~~~cpp
int analogValue = 0;
int ledValue = 0;

void setup() {
  Serial.begin(9600);
  pinMode(11, OUTPUT);
  
}

void loop() {
  analogValue = analogRead(A0);
  Serial.println(analogValue);

  ledValue = map(analogValue, 0, 1023, 0, 255);
  Serial.println(ledValue);
  
  analogWrite(11, ledValue);
  delay(10);
  
  Serial.print("Potentiometer: ");
  Serial.println(map(1023, 0, 1023, 0, 255)); //255
  
  Serial.print("LED: ");
  Serial.println(map(255, 0, 255, 0, 1023));//1023
}
~~~
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	potentiometer ແມ່ນເຊື່ອມຕໍ່ກັບ pin A0 ຂອງ Arduino ແລະ LED ແມ່ນເຊື່ອມຕໍ່ກັບ pin 11.
•	ການອ່ານຄ່າຈາກ potentiometer: ຟັງຊັນ analogRead(A0) ອ່ານຄ່າຈາກ potentiometer ເຊິ່ງຈະໄດ້ຮັບຄ່າລະຫວ່າງ 0 ຫາ 1023
•	ການແປງຄ່າ Potentiometer ຈະຖືກປ່ຽນຈາກຊ່ວງ 0-1023 ເປັນ 0-255 ໂດຍໃຊ້ຟັງຊັນ map().
•	ການຄວບຄຸມຄວາມສະຫວ່າງຂອງ LED: ຟັງຊັນ analogWrite(11, ledValue) ຈະປັບຄວາມສະຫວ່າງຂອງ LED ໂດຍອີງໃສ່ຄ່າທີ່ປ່ຽນໄດ້.
•	ຈໍສະແດງຜົນ Serial: ຄ່າ Potentiometer ແລະ ຄວາມສະຫວ່າງ LED ຖືກສະແດງຢູ່ໃນ Serial Monitor.
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/7OCThiI5mlE-potentiometer-08-vilaphonh-khamvongthong









# ບົດທີ 6 : Relay

### 1.	ບົດນຳ
ຣີເລ (Relay) ແມ່ນອຸປະກອນທີ່ໃຊ້ເພື່ອຄວບຄຸມວົງຈອນໄຟຟ້າແຮງດັນສູງດ້ວຍສັນຍານຄວບຄຸມແຮງດັນຕໍ່າຈາກ Arduino ເຊິ່ງເຮັດໃຫ້ພວກເຮົາສາມາດເປີດ-ປິດອຸປະກອນໄຟຟ້າພາຍນອກເຊັ່ນ: ດອກໄຟ, ມໍເຕີ, ຫຼື ອຸປະກອນທີ່ໃຊ້ໄຟຟ້າໃນຄົວເຮືອນ.
ໃນບົດນີ້, ພວກເຮົາຈະໃຊ້ relay 5V ເພື່ອຄວບຄຸມການເປີດ-ປິດຂອງ LED ໂດຍໃຊ້ Arduino.
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	Relay Module
•	LED
•	Resistor (220Ω)
•	Jumper wires
•	Breadboard
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
o	ເຊື່ອມຕໍ່ Relay ກັບ Arduino.
-	IN PIN (ສັນຍານຄວບຄຸມ) ຂອງ Relay → LED_BUILTIN pin (pin 13) ຂອງ Arduino.
-	GND pin ຂອງ relay → GND ຂອງ Arduino
-	VCC pin ຂອງ relay → 5V ຂອງ Arduino
-	ເຊື່ອມຕໍ່ LED ກັບ relay ໄດ້.
-	COM (ທົ່ວໄປ) pin ຂອງ relay →ເຊື່ອມຕໍ່ກັບ pole ບວກຂອງ LED ໄດ້.
-	NO (ເປີດປົກກະຕິ) pin of relay → ເຊື່ອມຕໍ່ກັບ 5V ຂອງ Arduino.
-	ຂົ້ວລົບຂອງ LED → 220Ω resistor → GND ຂອງ Arduino.
 

 
### 4.	ໂຄດທີ່ໃຊ້
~~~cpp
// C++ code
void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop()
{
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
}
~~~
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	Arduino ຄວບຄຸມ relay: ເມື່ອສັນຍານ HIGH ຖືກສົ່ງໄປຫາ LED_BUILTIN (pin 13), relay ຈະປິດວົງຈອນ (ເປີດ LED).
•	Delay 1 ວິນາທີ: Arduino ຈະລໍຖ້າ 1 ວິນາທີກ່ອນທີ່ຈະປ່ຽນສະຖານະ.
•	ປ່ຽນສະຖານະ: Arduino ປ່ຽນສັນຍານເປັນ LOW, ເຊິ່ງເຮັດໃຫ້ Relay ເປີດວົງຈອນ (ປິດໄຟ LED).
•	ເຮັດຊ້ຳ: ລະບົບເປີດ ແລະ ປິດໄຟ LED ທຸກ 1 ວິນາທີ.
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/7eFe0CF2B3q-relay-08-vilaphonh-khamvongthong

# ບົດທີ 7 :Servo

### 1.	ບົດນຳ
ມໍເຕີເຊີໂວ (Servo Motor) ແມ່ນມໍເຕີທີ່ສາມາດ rotate ກັບຕໍາແຫນ່ງທີ່ຊັດເຈນ. ມັນຖືກນໍາໃຊ້ທົ່ວໄປໃນຫຸ່ນຍົນ ຫຼື ລະບົບການຄວບຄຸມອັດຕະໂນມັດ. ບົດນີ້ແມ່ນກ່ຽວກັບວິທີການຄວບຄຸມ servo motor ໂດຍໃຊ້ Potentiometer
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	Servo motor 
•	Potentiometer
•	Jumper wires
•	Breadboard
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
-	ເຊື່ອມຕໍ່ຂາ VCC ຂອງ servo ກັບ 5V ໃນ Arduino.
-	ເຊື່ອມຕໍ່ GND pin ຂອງ servo ກັບ GND ຂອງ Arduino.
-	ເຊື່ອມຕໍ່ສາຍສັນຍານຂອງ servo ກັບ pin 9 ຂອງ Arduino.
-	ເຊື່ອມຕໍ່ pin 1 ຂອງ potentiometer ກັບ 5V ໃນ Arduino.
-	ເຊື່ອມຕໍ່ pin 2 (ກາງ) ຂອງ Potentiometer ກັບ A0 ຂອງ Arduino.
-	ເຊື່ອມຕໍ່ pin 3 ຂອງ Potentiometer ກັບ GND ຂອງ Arduino.
 

 

### 4.	ໂຄດທີ່ໃຊ້
~~~cpp
#include <Servo.h>
Servo myservo;  // create servo object to control a servo

int potpin = A0;  // analog pin used to connect the potentiometer
int val;    // variable to read the value from the analog pin

void setup() {
  Serial.begin(9600);
  myservo.attach(9);  // attaches the servo on pin 9 to the servo object
}

void loop() {
  val = analogRead(potpin);           // reads the value of the potentiometer (value between 0 and 1023)
  Serial.print("pot = ");
  Serial.print(val);
  Serial.print(", servo = ");
  val = map(val, 0, 1023, 0, 180);     // scale it to use it with the servo (value between 0 and 180)
  
  Serial.println(val);
  myservo.write(val);                  // sets the servo position according to the scaled value
  delay(15);                           // waits for the servo to get there
}
~~~

### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	Arduino ອ່ານຄ່າຈາກ potentiometer ທີ່ມີລະດັບ 0-1023.
•	ໃຊ້ຟັງຊັນ map(val, 0, 1023, 0, 180); ແປງຄ່າເປັນມຸມ 0-180 ອົງສາ.
•	ໃຊ້ myservo.write(val); ເພື່ອສັ່ງໃຫ້ servo motor ໝຸນໄປກັບມຸມທີ່ຕ້ອງການ
•	ຄ່າມຸມແມ່ນສະແດງຢູ່ໃນ Serial Monitor.
•	ໃນເວລາທີ່ໝຸນ potentiometer ເຫັນໄດ້ວ່າ servo motor ໝຸນຕາມມຄ່າທີ່ໄດ້ຮັບ.
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/8723ERcBl5m-servo-08-vilaphonh-khamvongthong

# ບົດທີ 8 :Seven Segment

### 1.	ບົດນຳ
7-Segment Display ເປັນອຸປະກອນສະແດງຜົນທີ່ໃຊ້ກັນຢ່າງກວ້າງຂວາງເຊັ່ນ: ໃນເຄື່ອງຄິດເລກ ຫຼື ໂມງດິຈິຕອນ ເຊິ່ງກ່ຽວກັບການນຳໃຊ້ 7-Segment Display ແບບ1 ຫຼັກດ້ວຍ Arduino ເພື່ອສະແດງຕົວເລກ 0-9.
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	7-Segment Display LED
•	Resistor (220Ω)
•	Jumper wires
•	Breadboard
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
ຈໍສະແດງຜົນ 7-Segment ມີ 7 pins (a-g) ເພື່ອສະແດງຕົວເລກ ແລະ common cathode (CC) ຫຼື common anode (CA) pin ເພື່ອກໍານົດປະເພດຂອງການດໍາເນີນງານ.
-	ເຊື່ອມຕໍ່ pins a-g ຂອງ 7-Segment ກັບ Arduino pins:
a → 2, b → 3, c → 4, d → 5, e → 6, f → 7, g → 8
-	ເຊື່ອມຕໍ່ cathode ທົ່ວໄປ (CC) ຫຼື anode ທົ່ວໄປ (CA) pin ກັບ GND ຫຼື 5V ຕາມປະເພດຂອງ 7-Segment.
-	ໃຊ້ຕົວຕ້ານທານ 220Ω ເປັນຊຸດກັບແຕ່ລະ pin a-g ເພື່ອຫຼຸດຜ່ອນກະແສໄຟຟ້າ.
 

 

### 4.	ໂຄດທີ່ໃຊ້
~~~cpp
// Define the pins for each segment of the display 

int segmentPins[] = {2, 3, 4, 5, 6, 7, 8}; // Adjust based on your wiring 

// Digits representation for common cathode display 

byte digits[] = { 

  B11111100, // 0 

  B01100000, // 1 

  B11011010, // 2 

  B11110010, // 3 

  B01100110, // 4 

  B10110110, // 5 

  B10111110, // 6 

  B11100000, // 7 

  B11111110, // 8 

  B11110110  // 9 

}; 

 

void setup() { 

  // Set all segment pins as OUTPUT 

  for (int i = 0; i < 7; i++) { 

    pinMode(segmentPins[i], OUTPUT); 

    digitalWrite(segmentPins[i], LOW); // Turn off all segments initially 

  } 

} 

 

void loop() { 

  // Display numbers 0 to 9 

  for (int i = 0; i <= 9; i++) { // Start from 0 

    displayDigit(i); 

    delay(1000); // Wait for 1 second 

  } 

 

  // Turn off the display for 1 second 

  clearDisplay(); 

  delay(1000); 

 

  // Display numbers 9 to 0 

  for (int i = 9; i >= 0; i--) { // Go down to 0 

    displayDigit(i); 

    delay(1000); // Wait for 1 second 

  } 

 

  // Turn off the display for 1 second 

  clearDisplay(); 

  delay(1000); 

} 

 

void displayDigit(int num) { 

  byte segments = digits[num]; 

  for (int i = 0; i < 7; i++) { 

    digitalWrite(segmentPins[i], bitRead(segments, 7 - i) ? HIGH : LOW); // Update each segment 

  } 

} 

 

void clearDisplay() { 

  for (int i = 0; i < 7; i++) { 

    digitalWrite(segmentPins[i], LOW); // Turn off all segments 

  } 

}
void displayDigit(int num) {
  byte segments = digits[num];
  for (int i = 0; i < 7; i++) {
    digitalWrite(segmentPins[i], bitRead(segments, 7 - i) ? HIGH : LOW); // Update each segment
  }
}

void clearDisplay() {
  for (int i = 0; i < 7; i++) {
    digitalWrite(segmentPins[i], LOW); // Turn off all segments
  }
}
~~~
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	Arduino ສົ່ງສັນຍານໄປຫາ 7-Segment Display ຜ່ານ pins ທີ່ກໍານົດໄວ້.
•	ໃຊ້ອາເຣ digits[] ເພື່ອກໍານົດລໍາດັບທີ່ LED ແຕ່ລະອັນຈະເປີດແລະປິດເພື່ອສະແດງຕົວເລກທີ່ຖືກຕ້ອງ.
•	ໃນວົງ()
•	ສະແດງຕົວເລກ 0-9, ແຕ່ລະຕົວເລກໃຊ້ເວລາ 1 ວິນາທີ.
•	ປິດໄຟທັງໝົດເປັນເວລາ 1 ວິນາທີ.
•	ສະແດງຕົວເລກ 9-0 ໂດຍແຕ່ລະຕົວເລກໃຊ້ເວລາ 1 ວິນາທີ.
•	ປິດໄຟທັງໝົດເປັນເວລາ 1 ວິນາທີ.
•	ໃຊ້ຟັງຊັນ displayDigit(int num) ເພື່ອສະຫຼັບແຕ່ລະ 7-Segment ເປີດ/ປິດ.
•	ໃຊ້ຟັງຊັນ clearDisplay() ເພື່ອລ້າງຈໍສະແດງຜົນ.
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/kkktBanlqvG-7-segment-08-vilaphonh-khamvongthong




# ບົດທີ 9 :Puppy Notify

### 1.	ບົດນຳ
Puppy Notify ເປັນເຄື່ອງສົ່ງສຽງ ແລະ ແສງ ເພື່ອແຈ້ງເຕືອນໃຫ້ເຮົາຮູ້ເວລາທີ່ສັດລ້ຽງຂອງເຮົາຫິວເຂົ້າ ຫຼຶ ຕ້ອງການສິ່ງຕ່າງໆໂດຍໃຊ້ RGB LEDs ແລະ Buzzer ໂດຍອີງຕາມການປ່ຽນສີຂອງໄຟ LED RGB ແລະ ສຽງຕາມປຸ່ມທີ່ກົດ.
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	Push Button
•	LED RGB
•	Resistor (220Ω)
•	Buzzer
•	Jumper wires
•	Breadboard
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
-	LED ເຊື່ອມຕໍ່ກັບຂາອອກດິຈິຕອນ 8, 9, 10 ພ້ອມກັບຕົວຕ້ານທານ.
-	ປຸ່ມກົດ (Button) ເຊື່ອມຕໍ່ກັບຂາເຂົ້າ 2, 3, 4 ໂດຍມີດ້ານໜຶ່ງເຊື່ອມກັບ GND.
-	ບັຊເຊີ (Buzzer) ເຊື່ອມກັບ Pin 11 ແລະ GND.
-	ເສັ້ນຈ່າຍໄຟ (Power rails) ຕໍ່ກັບ 5V ແລະ GND ຈາກ Arduino.
 

### 4.	ໂຄດທີ່ໃຊ້

~~~cpp
// Define LED pins
#define LED_RED 8
#define LED_GREEN 9
#define LED_BLUE 10

// Define button pins
#define BUTTON1 2
#define BUTTON2 3
#define BUTTON3 4

// Define buzzer pin
#define BUZZER 11

void setup() {
  // Initialize LED pins as output
  pinMode(LED_RED, OUTPUT);
  pinMode(LED_GREEN, OUTPUT);
  pinMode(LED_BLUE, OUTPUT);

  // Initialize button pins as input with pull-down resistors
  pinMode(BUTTON1, INPUT);
  pinMode(BUTTON2, INPUT);
  pinMode(BUTTON3, INPUT);

  // Initialize buzzer pin as output
  pinMode(BUZZER, OUTPUT);
}

void loop() {
  // Check if Button 1 is pressed
  if (digitalRead(BUTTON1) == HIGH) {  // Button pressed
    digitalWrite(LED_RED, HIGH);      // Turn on red LED
    tone(BUZZER, 440);                // Play 440 Hz tone
    delay(500);                       // Wait for 500ms
    digitalWrite(LED_RED, LOW);       // Turn off red LED
    noTone(BUZZER);                   // Stop buzzer
  }

  // Check if Button 2 is pressed
  if (digitalRead(BUTTON2) == HIGH) {  // Button pressed
    digitalWrite(LED_GREEN, HIGH);     // Turn on green LED
    tone(BUZZER, 600);                 // Play 600 Hz tone
    delay(500);                        // Wait for 500ms
    digitalWrite(LED_GREEN, LOW);      // Turn off green LED
    noTone(BUZZER);                    // Stop buzzer
  }

  // Check if Button 3 is pressed
  if (digitalRead(BUTTON3) == HIGH) {  // Button pressed
    digitalWrite(LED_BLUE, HIGH);      // Turn on blue LED
    tone(BUZZER, 800);                 // Play 800 Hz tone
    delay(500);                        // Wait for 500ms
    digitalWrite(LED_BLUE, LOW);       // Turn off blue LED
    noTone(BUZZER);                    // Stop buzzer
  }
}
~~~
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
•	ເມື່ອກົດປຸ່ມ 1, LED ແດງ ຈະເປີດ ແລະ buzzer ຈະສົ່ງສຽງ 440 Hz
•	ເມື່ອກົດປຸ່ມ 2, LED ຂຽວ ຈະເປີດ ແລະ buzzer ຈະສົ່ງສຽງ 600 Hz
•	ເມື່ອ ກົດປຸ່ມ 3, LED ນ້ຳເງິນ ຈະເປີດ ແລະ buzzer ຈະສົ່ງສຽງ 800 Hz
•	ທຸກໆ LED ຈະປິດລົງຫຼັງຈາກ 500 milliseconds
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/7qZb1BtvrSf-vilaphon-khamvongthong-no-08


# ບົດທີ 10 : Scoreboard Display

### 1.	ບົດນຳ
scoreboard display ເປັນເຄື່ອງສະແດງໂຕເລກ 0-9 ໂດຍໃຊ້ 7-Segment display ສາມາດນຳໄປໃຊ້ນັບຄະແນນໃນກິດຈະກຳຕ່າງໆ, ສາມາດປັບຄ່າໄດ້ຕາມຕ້ອງການໂດຍການກົດປຸ່ມ.
### 2.	ອູປະກອນ
•	Microcontroller (Arduino)
•	Button
•	Resistor (220Ω)
•	7-sagment (common cathode)
•	Jumper wires
•	Breadboard
### 3.	ການເຊື່ອມຕໍ່ວົງຈອນ
o	ການເຊື່ອມຕໍ່ Button:
-	Button 1 (ປຸ່ມເພີ່ມຄ່າ) ເຊື່ອມກັບ pin 10 ແລະ GND.
-	Button 2 (ປຸ່ມລົດຄ່າ) ເຊື່ອມກັບ pin 9 ແລະ GND.
o	ການເຊື່ອມຕໍ່ 7-segment display:
-	ເຊື່ອມຕໍ່ pins a, b, c, d, e, f, g ຂອງ 7-segment display ກັບ pins 2-8 ຂອງ Arduino.
-	pins ເຫຼົ່ານີ້ຄວບຄຸມການສະແດງຕົວເລກຈາກ 0-9.
-	Resistor ເຊື່ອມຂາ Cathode ແລະ Anode ຂອງ 7-segment display
o	ການເຊື່ອມຕໍ່ວົງຈອນໄຟຟ້າ:
-	ເຊື່ອມຕໍ່ GND ຂອງ Arduino ກັບ GND ຂອງທຸກພາກສ່ວນ.
-	ໃຫ້ແນ່ໃຈວ່າການສະໜອງພະລັງງານຂອງ Arduino ແມ່ນເຊື່ອມຕໍ່ກັບ 5V.
 

### 4.	ໂຄດທີ່ໃຊ້
~~~cpp
// Define the pins for the 7-segment display
const int segmentPins[] = {2, 3, 4, 5, 6, 7, 8}; // a, b, c, d, e, f, g

// Define the pins for the buttons
const int btnPlus = 10;
const int btnMinus = 9;

// Variables to store button states
int lastPlusState = HIGH;
int lastMinusState = HIGH;

// Counter value
int counter = 5;

// 7-segment display digit encoding (common cathode)
const byte digits[] = {
  0b00111111, // 0
  0b00000110, // 1
  0b01011011, // 2
  0b01001111, // 3
  0b01100110, // 4
  0b01101101, // 5
  0b01111101, // 6
  0b00000111, // 7
  0b01111111, // 8
  0b01101111  // 9
};

void setup() {
  // Set up the segment pins as OUTPUT
  for (int i = 0; i < 7; i++) {
    pinMode(segmentPins[i], OUTPUT);
  }

  // Set up button pins as INPUT_PULLUP
  pinMode(btnPlus, INPUT_PULLUP);
  pinMode(btnMinus, INPUT_PULLUP);

  // Display the initial value
  displayDigit(counter);
}

void loop() {
  // Read the button states
  int plusState = digitalRead(btnPlus);
  int minusState = digitalRead(btnMinus);

  // Check if the plus button is pressed
  if (plusState == LOW && lastPlusState == HIGH) {
    counter++;
    if (counter > 9) counter = 0; // Wrap around if counter exceeds 9
    displayDigit(counter);
    delay(200); // Debounce delay
  }

  // Check if the minus button is pressed
  if (minusState == LOW && lastMinusState == HIGH) {
    counter--;
    if (counter < 0) counter = 9; // Wrap around if counter goes below 0
    displayDigit(counter);
    delay(200); // Debounce delay
  }

  // Update the last button states
  lastPlusState = plusState;
  lastMinusState = minusState;
}

// Function to display a digit on the 7-segment display
void displayDigit(int num) {
  byte segments = ~digits[num];
  for (int i = 0; i < 7; i++) {
    digitalWrite(segmentPins[i], (segments >> i) & 0x01);
  }
}
~~~
### 5.	ການເຮັດວຽກຂອງວົງຈອນ
o	ຄ່າໂຕເລກທີ່ສະແດງ
•	ຈໍສະແດງຜົນ 7-segment ຄວບຄຸມໂດຍການໃຊ້ array of binary value(digit encoding)
•	ຟັງຊັນ displayDigit(counter) ຈະເຮັດໃຫ້ຈໍສະແດງຕົວເລກປະຈຸບັນ
o	ການເຮັດວຽກຂອງປູ່ມກົດ (button)
•	ເມື່ອກົດປຸ່ມ 1 (Pin 10) ຄ່າ counter ຈະເພີ່ມຂຶ້ນ
•	ເມື່ອກົດປຸ່ມ 2 (Pin 9) ຄ່າ counter ຈະລົດລົງ
•	ຄ່າຈະວົນຈາກ 0 ຫາ 9 ແລະ ກັບມາເລີ່ມໃໝ່ຖ້າເກີນຂີດຈຳກັດ
o	ເວລາໜ່ວງເພື່ອປ້ອງກັນການກົດຊຳ້
•	ຕັ້ງຄ່າ ເວລາໜ່ວງ 200ms ເພື່ອປ້ອງກັນການກົດຫຼາຍຄັ້ງໂດຍບໍ່ໄດ້ຕັ້ງໃຈ
### 6.	ແຫຼ່ງອ້າງອີງ
 
https://www.tinkercad.com/things/f820pPn40t2-scoreboard-display-08-vilaphonh-khamvongthong
