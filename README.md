Electric Motor Temperature

Business Objective:
Predict Motor Speed based on other attributes available and predict pm and stator_yoke on other aviable attributes

The dataset comprises several sensor data collected from a permanent magnet synchronous motor (PMSM) deployed on a test bench. The PMSM represents a german OEM's prototype model. Test bench measurements were collected by the LEA department at Paderborn University. This dataset is mildly anonymized.
All recordings are sampled at 2 Hz. The dataset consists of multiple measurement sessions, which can be distinguished from each other by column "profile_id". A measurement session can be between one and six hours long.
The motor is excited by hand-designed driving cycles denoting a reference motor speed and a reference torque. Currents in d/q-coordinates (columns "i_d" and i_q") and voltages in d/q-coordinates (columns "u_d" and "u_q") are a result of a standard control strategy trying to follow the reference speed and torque. Columns "motor_speed" and "torque" are the resulting quantities achieved by that strategy, derived from set currents and voltages.
Most driving cycles denote random walks in the speed-torque-plane in order to imitate real world driving cycles to a more accurate degree than constant excitations and ramp-ups and -downs would.


Feature set:

ambient:
Ambient temperature as measured by a thermal sensor located closely to the stator.

coolant:
Coolant temperature. The motor is water cooled. Measurement is taken at outflow.

u_d:
Voltage d-component

u_q:
Voltage q-component

motor_speed:
Motor speed

torque:
Torque induced by current.

i_d:
Current d-component

i_q:
Current q-component

pm:
Permanent Magnet surface temperature representing the rotor temperature. This was measured with an infrared thermography unit.

stator_yoke:
Stator yoke temperature measured with a thermal sensor.

stator_tooth:
Stator tooth temperature measured with a thermal sensor.

stator_winding:
Stator winding temperature measured with a thermal sensor.

profile_id:
Each measurement session has a unique ID. Make sure not to try to estimate from one session onto the other as they are strongly independent.
