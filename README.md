# headphone-usb
This is my documented process of fixing my logitech g733 headphone lightspeed 2.4GHz dongle <br/>
 ☆ 3D Printer: Bambu Lab P2S<br/>
 ☆ CAD Program: Solidworks<br/>
 ☆ Sketch Program: Procreate<br/>
 ☆ Solder Iron: FNIRSI HS-02  Soldering Iron<br/>

## The initial issue:<br/>
This lightspeed dongle's USB port broke and bent. I assume it was during a move to different houses. The dongle no longer worked unless it was in this specific angle and it was impractical. So, I have decided to fix it and redesign the shell so I won't have to buy a new headset. <br/>
<img width="3024" height="4032" alt="problem 1" src="https://github.com/user-attachments/assets/bc36d6d1-6f03-4b77-8001-ce3e57e4cdcb" /> <img width="3024" height="4032" alt="problem 5" src="https://github.com/user-attachments/assets/bf3af461-e6a7-4ccd-a276-084aaeb67549" /><img width="3024" height="4032" alt="problem 3" src="https://github.com/user-attachments/assets/151664d5-f50b-4ab3-a3da-e35486f32c89" /><img width="3024" height="4032" alt="problem 2" src="https://github.com/user-attachments/assets/90210594-8d41-4416-ab37-90cbb3ac6c1c" /> <br/>

# The finished product:<br/>
<img width="1320" height="1670" alt="E8BB7BCA-DA52-46C4-9C92-998D79B75FAA (1)" src="https://github.com/user-attachments/assets/a23d34ce-1f11-4a8d-8b65-3507fbd83aa5" /><br/>

# Soldering and fixing the PCB <br/>
Soldering the new connector was quite a challenge but I am glad I got it to work in the end. One of the bridge pads broke during disassembly. However, without having the schematic (because Logitech has not publicly published it), I was able to figure out what pad to bridge it to and make a working connection. It was rewarding to go through this challenge and get it to work in the end. <br/>
## Finished solder job:<br/>
<img width="4032" height="3024" alt="IMG_4978" src="https://github.com/user-attachments/assets/b8f069df-f702-433d-962b-94020e9632a2" /><br/>
<img width="4032" height="3024" alt="IMG_4980" src="https://github.com/user-attachments/assets/da6d6c8a-48c0-48ba-bb49-87027a8a14b9" /> <br/>
<img width="3024" height="4032" alt="IMG_4981" src="https://github.com/user-attachments/assets/d2385103-e533-4b27-8301-a22d784aa00a" /> <br/>
## The broken pad: <br/>
One of the bridge pads lifted during disassembly and took its trace with it. Logitech doesn’t publish a schematic, so I used a multimeter in continuity mode to trace where the pad had connected. It ran to the end terminal of the nearby black SMD component. I bridged the gap with the USB port leg that I have shaped before soldering, so it wouldn’t pull on the joint. Before powering it , I checked for shorts between the new connection.<br/>
<img width="3024" height="4032" alt="IMG_4738" src="https://github.com/user-attachments/assets/d9f41b92-a474-4a42-ab46-057378b665bb" /><br/>
<br/>

I also lost a small capacitor during the repair and couldn’t determine its value without a schematic. Since the dongle worked without it, I left it off. It is most likely a decoupling cap. If I see audio dropouts or range problems, the first thing I’d add is a 1–10µF ceramic cap. <br/>



# Redesigning the shell:<br/>
The rough sketch ideas:<br/>
<img width="1320" height="2346" alt="rough sketch " src="https://github.com/user-attachments/assets/aeca9296-88c1-4773-a559-7234bcbbb25d" /><br/>

### The drawing of the part (Designed in SOLIDWORKS):<br/>
<img width="2767" height="1484" alt="usb case" src="https://github.com/user-attachments/assets/d328b849-55b0-4e88-adc1-c23b5441f628" /><br/>

### Printing Prototype 1:<br/>
<img width="5712" height="4284" alt="bambu lab studio" src="https://github.com/user-attachments/assets/2f15b1b2-b751-4406-997a-aaf50828adae" /><br/>
<img width="3024" height="4032" alt="print 3" src="https://github.com/user-attachments/assets/92445c77-c9fb-4c29-a708-3e6aaaba5717" /><br/>
<img width="3024" height="4032" alt="print 2" src="https://github.com/user-attachments/assets/bd524bbd-ddb8-4f4a-9ab2-4c0a9951f3a7" /><br/>
<img width="3024" height="4032" alt="Prototype 1" src="https://github.com/user-attachments/assets/bc0769a1-890b-40f4-91f0-f516cb164776" /><br/>
I have ran into a problem and have excluded the light hole and the offset for the board to sit in. But the hole for the USB A connector to stick out is a perfect fit. I have redesigned and added both missing features. (refer to SOLIDWORKS drawing above)<br/>
<img width="4284" height="5712" alt="prototype process 2" src="https://github.com/user-attachments/assets/b4da2c55-3efc-461a-b71d-db7e410e3d6a" /><br/>

### Process:<br/>
The body was printed in PLA Pure filament in the color milky pink by Bambu Lab. The stars were printed in PLA Matte filament in the color sakura pink by Bambu Lab. I have also changed the orientation of the print in the 3D printer to eliminate the print bed texture. Giving the print that smooth texture from the PLA Pure filament. <br/>


### new drawing in SOLIDWORKS:<br/>
<img width="2782" height="1465" alt="look" src="https://github.com/user-attachments/assets/9f27eaca-43ad-4fd4-b0e6-be8c84cbc634" /><br/>
### New Studio Print:<br/>
<img width="4032" height="3024" alt="print 4" src="https://github.com/user-attachments/assets/356d1d14-fa98-4b44-b65a-ec9649218e6d" /><br/>
# Original 1, Prototype 1, Revision 2:<br/>
<img width="4032" height="3024" alt="file forms" src="https://github.com/user-attachments/assets/1241ca9d-c7ab-4c69-b95a-e21aa52eebc4" /><br/>
This print orientation did not go as expected. There were a few impurities on the opening for the connector. So dimension wise, the board fits, but not in this shell. I will sand it down when the time comes.<br/>
<br/>
<br/>
This is the side comparison. I liked the first print (left) compared to the second print (right). It is more flush and that is what I am looking for.<br/>
<img width="3722" height="2627" alt="Side view" src="https://github.com/user-attachments/assets/34c30668-80ca-4088-a29e-b1d2bcce86be" /><br/>

With the stars:<br/>
<img width="3024" height="2753" alt="stars 1" src="https://github.com/user-attachments/assets/6e9b20de-bc4b-4f08-81dc-bee3af14d2e5" /><br/>
The stars assembled: <br/>
<img width="3024" height="4032" alt="IMG_4734" src="https://github.com/user-attachments/assets/526532b1-97d9-419c-b879-93bb6b6c39b6" /><br/>

### Printing and testing prototype #2:<br/>
The assembly:<br/>
<img width="2782" height="1510" alt="the assem" src="https://github.com/user-attachments/assets/83e495ba-a23d-46a7-8fb6-fbd4f86578a9" /><br/>

### The final dongle case assembled:<br/>
<img width="3024" height="4032" alt="IMG_5021" src="https://github.com/user-attachments/assets/42bb61cc-ed34-4023-ae5b-b2b0be72bdb7" /><br/><img width="3024" height="4032" alt="IMG_5022" src="https://github.com/user-attachments/assets/f676ba21-d7db-49c3-8c57-97b170850429" /><br/><img width="3024" height="4032" alt="IMG_5023" src="https://github.com/user-attachments/assets/71c3269f-695e-4da7-9908-48b20a84510e" /><br/>
<img width="3024" height="4032" alt="IMG_5029" src="https://github.com/user-attachments/assets/36019137-eb51-4064-babf-473c15ea05e1" /><br/> 
<img width="3024" height="4032" alt="IMG_5030" src="https://github.com/user-attachments/assets/6ee210a2-a40c-4b40-b251-7304929d719f" /><br/>

### the stars!<br/>
<img width="3024" height="4032" alt="IMG_5033" src="https://github.com/user-attachments/assets/07f021de-5ff0-401b-8834-ca1acf9f6018" /><br/>


# The final product:
<img width="1320" height="1670" alt="E8BB7BCA-DA52-46C4-9C92-998D79B75FAA (1)" src="https://github.com/user-attachments/assets/a23d34ce-1f11-4a8d-8b65-3507fbd83aa5" /><br/>

This project was interesting and fun to make. I learned how to solder new ports and how to replace them when they are broken. I also learned more about 3D printing. It was important to design with the 3D printer in mind. I enjoyed designing and creating the different layers of the dongle so it had 3D stars. I also had practice troubleshooting and testing the dongle circuit board with a multimeter. And practice in CAD/SolidWorks is always a good move. It was nice creating the assemblies and drawings in SolidWorks. <br/>

## Sources:<br/>
[FCC ID filing for JNZA00179](https://fccid.io/JNZA00179)












