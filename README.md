# VW-e-UP-OBD-CAN-logs

the .asc files behind these links contain logs of all messages on the Comfort CAN while periodically issuing requests for certain known parameters at the OBD2-port.

**KCAN+obd_Testfahrt3.asc: short trip with motor data from ECU 01 (7E0/7E8):**

**https://github.com/sharkcow/VW-e-UP-OBD-CAN-logs/blob/master/KCAN%2Bobd_Testfahrt3.asc**

==================== ================= ===============
logged OBD2-codes    value             comments 
==================== ================= ===============
22 F4 5B             state of charge   net?
22 14 7D             motor current
22 14 84             motor voltage
22 14 7E             motor power
22 14 7F             motor torque
22 14 9A             motor rpm
22 F4 49             acc. pedal
22 F4 0D             speed
22 14 85             battery power
22 16 17             HV-system current
==================== ================= ===============

**KCAN+obd_charge90-100.asc: charging from about 90% to 100%:**

**https://github.com/sharkcow/VW-e-UP-OBD-CAN-logs/blob/master/KCAN%2Bobd_charge90-100.asc**

car is charged from about 90% until it stops chargging, two different SoC codes are logged:

==================== =========================== ===============
logged OBD2-codes    value                       comments 
==================== =========================== ===============
7E0 03 22 F4 5B      state of charge from ECU 01
7E5 03 22 02 8C      state of charge from ECU 8C
==================== =========================== ===============

**KCAN+obd_Klima_remote.asc: remote heating test via OBD from ECU 75 (767/7D1):**

**https://github.com/sharkcow/VW-e-UP-OBD-CAN-logs/blob/master/KCAN%2Bobd_Klima_remote.asc**

remote heating started via OBD at 200s, stopped at 230s, started again 250-280s

**KCAN_Klima_remote_app_2x.asc: remote heating test via online app (no OBD):**

**https://github.com/sharkcow/VW-e-UP-OBD-CAN-logs/blob/master/KCAN_Klima_remote_app_2x.asc**

car was fully asleep (no messages on KCAN), remote heating turned on via app, then turned off again until car was fully asleep, then repeated the process

**KCAN_remote_Klima_app_22_20C.asc (no OBD):**

**https://github.com/sharkcow/VW-e-UP-OBD-CAN-logs/blob/master/KCAN_remote_Klima_app_22_20C.asc**

remote heating activated for two different temperatures (22°C and 20°C, previous logs were all at 21°C)

**KCAN+obd_Testfahrt_Akku1.asc: short trip with battery data from ECU 8C (7E5/7ED):**

**https://github.com/sharkcow/VW-e-UP-OBD-CAN-logs/blob/master/KCAN%2Bobd_Testfahrt_Akku1.asc**

==================== ============================ ===============
logged OBD2-codes    value                        comments 
==================== ============================ ===============
22 1E 34             minimum cell voltage & index
22 1E 33             maximum cell voltage & index
22 1E 0F             minimum temperature & sensor
22 1E 0E             maximum temperature & sensor
22 1E 3B             battery voltage
22 1E 3D             battery current
22 18 8D             battery power loss
22 02 8C             state of charge              gross?
==================== ============================ ===============

**KCAN+obd_rundown_6-0km.asc: complete rundown to vehicle turn off with battery data from ECU 01 & 8C (7E0/7E8 & 7E5/7ED):**

**https://github.com/sharkcow/VW-e-UP-OBD-CAN-logs/blob/master/KCAN%2Bobd_rundown_6-0km.asc**

==================== ============================ ===============
logged OBD2-codes    value                        comments 
==================== ============================ ===============
22 1E 34             minimum cell voltage & index
22 1E 33             maximum cell voltage & index
22 1E 0F             minimum temperature & sensor
22 1E 0E             maximum temperature & sensor
22 1E 3B             battery voltage
22 1E 3D             battery current
22 F4 5B             state of charge   		  net?
22 02 8C             state of charge              gross?
==================== ============================ ===============


