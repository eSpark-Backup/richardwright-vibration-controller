# RichardWright-Vibration_Controller
 
## Project Requirements
### Description
The project is for a vibrating device that is intended to produce different vibrations controlled by firmware. The product will be a battery powered device with with the capability to charge it via means of USB C interface.

### Required Features
1. The product is to be powered using LiPo or coin cell (whichever one is better in the given use case)
2. The product will feature the following major components:
  * MCU (needs to be selected, one that can drive the motor as well as be very cost and power effective)
  * [Vibration Motor](https://www.vybronics.com/coin-vibration-motors/lra/v-g1040003d) link is specified. This was finalized by client and the client believes that 3 of these motors will be enough. However we will need to study       properly and guide the client with the best solution. It is also observed that these motors come with their own driving circuit that needs to be studied as well.
  * If we go with the option of LiPo / Li-Ion, then an appropriate charging circuit is also required. The link to [LiPo](https://tinycircuits.com/collections/batteries/products/lithium-ion-polymer-battery-3-7v-500mah) is also specified. If we go with coin cell (which I don't think can be feasible), then replaceablity is fine.
  * There will also be battery supervisor circuit to minimize the current draw as much as possible.
  * The input to battery charging will be 5V provided via USB-C connector
  * The whole design has to be managed in 40mm(L) x 20mm(W) x 15mm(h) margins so component selection should be done accordingly. If needed, PCB designers can also be engaged at an early stage of component for their opinion on component size.
  * The product will also have a user Push Button. This same button can be used to power ON/OFF the product and to cycle through different vibration modes. The power ON/OFF will require long press and the modes cycling will be done via short presses. The duration calculation will be done via the MCU but the hardware design should account for power ON/OFF feature via single button.
 
