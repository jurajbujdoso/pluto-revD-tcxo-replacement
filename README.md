# pluto-revD-tcxo-replacement

Original source:

https://s-taka.org/plutosdr-revision-c/


https://blog-goo-ne-jp.translate.goog/osqzss/e/02041fe5dc9f4e204f7243fc0cda03ed?_x_tr_sl=auto&_x_tr_tl=sk&_x_tr_hl=sk&_x_tr_pto=wapp

# List of required HW

Desoldering tape:
https://www.aliexpress.com/item/1005003252802464.html?spm=a2g0o.order_list.order_list_main.5.3bfa1802rCCLSM

Heat resistant polyimide tape:
https://www.aliexpress.com/item/1005001382622258.html?spm=a2g0o.order_list.order_list_main.10.3bfa1802rCCLSM

Precision tweezers -pinzete
https://www.aliexpress.com/item/1005004223074659.html?spm=a2g0o.order_list.order_list_main.31.3bfa1802rCCLSM

Soldering station with heater (400-500"C)
https://www.aliexpress.com/af/soldering-station-smd.html?d=y&origin=n&SearchText=soldering+station+smd&catId=0&spm=a2g0o.detail.1000002.0&initiative_id=SB_20221222215521

soldering paste, I prefer one wit Au
https://www.aliexpress.com/item/1005004654324980.html?spm=a2g0o.order_list.order_list_main.5.22fe1802wc04Tj

Oscillator  TG2520SMN 40.0000M-ECGNNM3 (EPSON)


# Procedure

Oscillator is located on back side of pluto device. The pcb contains white dot which is important for oscillator position. The same dot is also on oscillator part.
![BEFORE](1671775967325.jpg)

Use the heat resistant tape and create a mesh next to the oscilator.  Then use desoldering station. I was not successfull with heater bellow 200"C and the success come with about 480"C. With tweezers I have removed old oscilator.
![mask](pred.jpg)

After removing of old oscillator use desoldering tape with soldering tips and remove old tin from pcb. I did not done it in first try and parts where not align and I have to desolder new osicillator :(. Add add some small amount of thin soldering paste on pcb afterwards. Place the smd oscillator on soldering paste and pcb. 
![removed](odobrane.jpg)

Use the heat station to distribute heat on soldering paste. I used 350"C and air flow in range of 10%. I recommend to keep heat resistant tape on pcb during soldering. It prevents from demage of other parts and does not allow soldering paste to move to unwanted direction.
![soldered](po-vymene.jpg)

It is huge help to have electronic microsope or magnify glasses during procedure. I just use black pen marker to create more visible dot on smd oscillator for better aligment.

# Result
In the first test device seems to work, but it require some experience to provide feedback. Precision is now 100x better.
With 20ppm and 1Ghz the freq. difference could be aroung 20Khz.

Base on japan article former osicillator was reponsible for switch to provide external clock signal. With the replacement the external clock is no available any longer => No Leo Bodnar or similar solution.
