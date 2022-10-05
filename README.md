# HannoHoffman-Smart-Alarm-controlling-lights-outside-with-arduino
An Arduino (ESP 32) was used to look at the status of the alarm buzzer to determine if the lights must go on outside. 

- The status of the alarm output determines wheter the outdoor lights must go on for 2 seconds (for when the alarm is armed or disarmed)
- Or when the alarm goes off, then the lights must flash 5 times and stay on for 2 minutes. 

**Required Components:**

- Male DC Plug
- Female DC Plug
- 10k Ohm Resistors x2 
- Breadboard 
- ESP 32 or Arduino Uno 
- 1ch Relay 
- Lights (ensure a compatent electrician works on the wiring of any voltage higher than 12V) 
- Smart alarm system
- Power supply for ESP32 of Arduino (5V cable) 

**Wiring:**
- Cut the output of cable of the aux cable in halve and attach to the DC jacks. 

![20220909_180842_resized](https://user-images.githubusercontent.com/115072716/194035603-b19bbd0c-49d7-4499-adcb-b73e7f06dd39.jpg)

- Then connect the two wires in parallel to the output of the alrm side (siren side) and this wires must be connected to the breadboard. 
- Now connect the ground of the alarm to the ground bus (choose one on the breadboard) 
- Also connect the ground of the ESP32 to the ground bus.
- Then connect the two resistors in series with one end attached to the ground bus.
- The other side of the two resistors (total of20kOhm) must be connected to the positive wire from the alarm (signal wire that was connected) 
- From the centre of the two resistors a wire must be connected to the input pin to the ESP32. 

![20220909_202829_resized](https://user-images.githubusercontent.com/115072716/194035858-b37792f7-cce4-4d48-ad3e-9a6d35dad2f3.jpg)
