# Gebruiksaanwijzing

### opladen / vervangen batterijen
Als de batterijen van de Linefollower leeg zijn moeten ze vervangen worden. De batterijhouder staat tussen de wielen van de Linefollower. Indien u de batterijen wilt hergebruiken moet er een opladers voor aangekocht worden.
### draadloze communicatie
#### verbinding maken
De app waarmee we verbinden met de Linefollower is de "Serial Bluetooth Terminal". De Bluetooth module waarmee er moet geconnecteerd worden is de "HC-05" waarvan de code 1234 is. Om hiermee te verbinden moet druk je op de stekker rechtsboven in de app, tik dan op de "HC-05" en geef de code in.

#### commando's
debug [on/off]  
start  
stop  
set cycle [µs]  
set power [0..255]  
set diff [0..1]  
set kp [0..]  
set ki [0..]  
set kd [0..]  
calibrate black  
calibrate white  

### kalibratie
Er zijn 2 commando's voor de kalibratie waaronder één voor wit te kalibreren van de Linefollower en één voor zwart te kalibreren. Zet de robot op een schoon wit vlak en geef in de Serial Bluetooth Terminal het commando "calibrate white", om de kalibratie voor wit uit te voeren. Idem voor zwart maar op een zwart vlak en met het commando "calibrate black".

### settings
De robot rijdt stabiel met volgende parameters: Cycle time: 2500, Power: 200, diff: 0.48, kp: 14, ki: 0.03, kd: 0.25, dAlpha: 0.7 

### start/stop button
Er is geen fysieke knop met een start/stop functie, dit wordt gedaan via de draadloze communicatie en een run on en run off commando. Ook zal de Linefollower stoppen als er geen duidelijke zwarte lijn aanwezig is.
