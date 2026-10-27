# Flightory — Super Stingray build notes

A build reference for the Super Stingray flying wing and its VTOL conversion, with parts sources for builders in India.

## Aircraft illustrations

### Super Stingray — fixed wing

![Super Stingray fixed-wing line-art concept](docs/images/super-stingray-fixed-wing-line-art.png)

A swept flying wing with a modular nose and one rear pusher motor.

### Super Stingray — VTOL

![Super Stingray VTOL line-art concept](docs/images/super-stingray-vtol-line-art.png)

The VTOL conversion adds four lift motors on two booms. The rear pusher motor remains in place.

### Fixed wing — exploded view

![Super Stingray fixed-wing conceptual exploded view](docs/images/super-stingray-fixed-wing-exploded.png)

The illustration separates the main modules: wing panels, access hatches, removable nose, and rear motor with its propeller.

### VTOL — exploded view

![Super Stingray VTOL conceptual exploded view](docs/images/super-stingray-vtol-exploded.png)

The illustration separates the wing panels, nose, hatches, two lift-motor booms, four lift motors, and rear pusher motor. It shows how the VTOL modules relate to the base aircraft.

*These generated illustrations use Flightory's product images as visual references. Exploded views show the main modules only. Part shapes, joints, spacing, and alignment are illustrative. Use the supplied Flightory manual for assembly.*

## The aircraft

The [Super Stingray](https://flightory.com/product/superstingray/) is a swept flying wing with a rear pusher motor, removable wings, and a modular nose. The [VTOL pack](https://flightory.com/product/super-stingray-vtol/) adds four lift motors on two booms. It is an add-on to the base aircraft, not a separate complete aircraft kit.

| Item | Fixed wing | VTOL conversion |
| --- | --- | --- |
| Wingspan | 1,130 mm | 1,130 mm |
| Length | 700 mm | 700 mm |
| Flightory listed all-up mass | 1,000–2,500 g | 1,500–2,800 g |
| Motors | One rear pusher | Four lift motors + one rear pusher |
| Print materials | LW-PLA and PETG | LW-PLA and PETG |
| Minimum print bed | 220 × 220 mm | 220 × 220 mm |
| Paid design files | Base package | Base package + VTOL pack |

*Dimensions and mass ranges come from the linked Flightory product pages. They are design references, not measured results from this repository.*

## Design files and credit

Aircraft design: **Flightory, Szymon Wójcik**. Purchase the [base files](https://flightory.com/product/superstingray/) and the [VTOL conversion](https://flightory.com/product/super-stingray-vtol/) from the designer. Flightory lists these products for personal use under its [licence agreement](https://flightory.com/license/). This guide does not grant rights to the paid files.

Use the official product pages and the manual supplied with your purchase for print settings, assembly, centre of gravity, and wiring. These build notes and supplier options do not replace that manual.

## Can the README show a 3D model?

Yes. GitHub supports interactive models in a fenced `stl` block that contains ASCII STL data. It also provides a separate viewer for an individual STL file, with a documented 10 MB limit. It cannot open an STL inside a ZIP as an inline model.

The inspected archives contain **42 binary STL parts** for the base aircraft and **14 binary STL parts** for the VTOL conversion. These are separate print parts. A useful full-aircraft preview needs an assembled model with the correct part positions. A small preview mesh can then be converted to ASCII STL for the README. Do not treat a collection of print parts as an assembled aircraft.

For now, this guide uses static illustrations. No paid mesh is added to this preview.

Sources: [GitHub Markdown STL support](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams#creating-stl-3d-models), [GitHub STL file viewer and limits](https://docs.github.com/en/repositories/working-with-files/using-files/working-with-non-code-files#3d-file-viewer).

## Parts sources in India

Research date: **27 October 2026**. Prices are in INR. These are seller listings, not quotes or reserved stock. Some evidence comes from search-index copies; stock and prices can change. Shipping is extra unless the seller states otherwise. Confirm the final amount, GST, variant, and delivery to your PIN code before purchase.

“Sold in India” does not mean “made in India.” Most options below are imported products sold by Indian suppliers. No alternative below has been flight-tested for this build.

### Shared electronics

| Part / quantity | Flightory reference | Indian source / listed price | Availability evidence | Fit and substitution notes |
| --- | --- | --- | --- | --- |
| Flight controller ×1 | SpeedyBee / Matek F405 Wing | [SpeedyBee F405 WING APP — Xbotics](https://xbotics.in/product/speedybee-f405-wing-app-flight-controller/): **₹5,556.92 incl. GST** | Indexed listing says 7 in stock; live page extraction did not confirm stock | Same named controller family. Confirm board revision, included power board, firmware target, and output allocation. |
| Controller alternative ×1 | Wing controller | [SpeedyBee F405 WING MINI — UAVGarage](https://uavgarage.com/shop/speedybee-f405-wing-mini-fixed-wing-flight-controller/): **₹5,072.82 incl. GST** | Pre-order | Different board and connector layout. Confirm the required outputs and power distribution, especially for VTOL. |
| GPS + compass ×1 | Matek M10Q or similar | [Foxeer M10Q 120 + QMC5883 — Robu](https://robu.in/product/foxeer-m10q-120-gps-5883-compass/): **₹2,429 incl. GST** | Listing says in stock | Alternative brand. Check UART, I²C, connector pinout, supply voltage, and compass support. |
| Elevon servos ×2 | EMAX ES08MA II metal gear | [EMAX ES08MA II — IBOTS](https://ibots.in/product/emax-es08ma-ii-servo/): **₹860 each; ₹1,720 for two** | Backorder; seller says backorder price may vary | Same named servo. Confirm GST and lead time. Check horn fit, travel, and supply voltage. |
| Receiver ×1 | Matek R24-D ELRS or similar | [RadioMaster RP1 V2 — Zbotic](https://zbotic.in/product/radiomaster-rp1-expresslrs-2-4ghz-nano-receiver/): **₹2,476.82 incl. GST** | Listing says in stock | ELRS/CRSF alternative. Confirm radio band, firmware compatibility, failsafe, and antenna placement. |
| Pusher ESC ×1 | BLHeli 30–40 A | [EMAX BLHeli 30 A Oneshot — Robu](https://robu.in/product/emax-blheli-series-30a-esc-oneshot-original/): **₹2,009 incl. GST** | Listing says in stock | 30 A continuous, not 40 A continuous. Validate current with the chosen motor, propeller, and 4S battery. |
| ESC alternative ×1 | 30–40 A ESC | [SimpliFly 30 A 2S–6S — Robocraze](https://robocraze.com/products/simplifly-esc-30a-2s-6s-for-bldc-motors-with-d-shot-oneshot125): **₹862 incl. GST** | Add-to-cart shown; stock count not stated | Lower-cost candidate. [Robu lists India as country of origin](https://robu.in/product/simplifly-esc-30a/). Confirm the exact revision and continuous-current rating. |

### VTOL additions

| Part / quantity | Flightory reference | Indian source / listed price | Availability evidence | Fit and substitution notes |
| --- | --- | --- | --- | --- |
| Lift motors ×4 | EMAX ECO II 2306 1700KV / T-Motor F60 1750KV | [EMAX ECO II 2306 1700KV — Zbotic](https://zbotic.in/product/ecoii-2306-1700kv-brushless-motor/): **₹1,827.82 each; ₹7,311.28 for four, incl. GST** | Add-to-cart shown; stock count not stated | Same named EMAX model. Seller text mentions 5–5.5-inch props, while Flightory specifies 7-inch lift props. Resolve this with motor data and a current/thrust test. |
| Lift-motor alternative ×4 | 2306 class, about 1700KV | [iFlight XING-E Pro 2306, 1700KV — Fioparts](https://fioparts.com/products/iflight-xing-e-pro-2306-motor): **₹1,899 each; ₹7,596 for four, incl. GST** | Dispatch stated as 3–4 business days; exact variant stock needs confirmation | Candidate only. Matching KV and stator size does not prove equivalent thrust, mounting, or 7-inch propeller suitability. |
| Lift propellers, 2 CW + 2 CCW | 7×4 / 7×5 / 7×6 | [DalProp Cyclone 7040 bi-blade, four-prop set — The Engineer Store](https://www.theengineerstore.in/products/foxeer-dalprop-cyclone-bi-blade-7040-propeller-2-pair-cw-ccw-crystal-black): **₹232.14 per set** | Add-to-cart shown; seller states 3–5 working days dispatch | Nominal 7×4 size. Confirm GST, hub, shaft fit, rotation, and the motor test data. |
| Four lift ESC channels | Four 30–40 A singles or a suitable 4-in-1 | [T-Motor Velox V2 V45A 4-in-1 — Fioparts](https://fioparts.com/products/t-motor-velox-v2-v45a-3-6s-blheli32-4-in-1-esc): **₹7,999 incl. GST** | Seller states 3–4 business days dispatch; stock count not stated | Candidate only. The rear pusher still needs its own ESC. Confirm power input, signal harness, mounting, and cooling. |

### Radio, battery, and FPV options

| Item | Indian option / listed price | Availability evidence | What to check |
| --- | --- | --- | --- |
| RC transmitter | [RadioMaster Pocket ELRS — RC Mumbai](https://rcmumbai.com/products/radiomaster-pocket?variant=50865323180313): **₹8,179.99 incl. tax** | Listing says in stock | Select ELRS, not CC2500. Seller says two 18650 cells are not included. |
| 4S LiPo candidate | [SHANGYI 5200 mAh 4S 60C — Vimaana Technologies](https://www.vimaanatech.com/product-page/5200-mah-4s-14-8v-lipo-battery): **₹4,364** | Listed; stock and tax treatment need confirmation | Seller lists 148×50×31 mm, 550 g, Deans plug. Check bay fit, centre of gravity, connector, and measured current. This is not the designer's endurance pack. |
| Battery comparison | [Orange 5200 mAh 4S — Havoc Hobby](https://havochobby.in/products/orange-5200mah-4s-40c-80c-14-8v-lithium-polymer-battery-pack): **₹7,870 incl. tax** | Sold out | 488 g, 137×44×40 mm, XT60. Included as a price/fit comparison, not an available purchase. |
| Balance charger | [ISDT 608AC — Xbotics](https://xbotics.in/product/isdt-608ac-200w-50w-smart-charger/): **₹9,789.40 incl. GST** | Indexed listing says 10 in stock | 50 W AC / 200 W DC. Confirm included mains supply and charge lead. [Manufacturer reference](https://isdtshop.com/en-in/products/isdt-608ac). |
| Analog FPV camera | [RunCam Phoenix 2 — Kapdronix](https://kapdronix.com/products/c08-002): **₹4,675.04 incl. GST** | Listing says in stock | Listed 19×19 mm camera size matches the base design's nominal camera format. Check actual mounting and lens clearance. Needs a separate analog VTX, antenna, and matching goggles. |

## Items still to source or validate

This is a sourcing guide, not a complete shopping cart. No full-build total is given because the propulsion selection and several required items remain open.

- **Pusher motor:** Flightory specifies 23XX, 1000–1400KV, with a 10×5 or 10×6 propeller. An exact Indian-stock match with sufficient technical evidence was not confirmed. Do not substitute a common 2300KV racing motor based on price alone.
- **Pusher propeller:** [Robu lists an HQProp 10×5](https://robu.in/product/hqprop-thin-electric-prop-10x5-2ccw-propeller/), but price and stock could not be confirmed. Confirm correct rotation and shaft fit.
- **Power distribution:** confirm a suitable PDB, current sensor, BEC, wire sizes, connectors, and total current capacity for the complete VTOL power system.
- **Video link:** choose a complete analog or digital system. Camera, VTX, antennas, and goggles must work together. No complete Indian-stock video bundle was validated here.
- **Airframe hardware:** use the manual's carbon-tube sizes, inserts, screws, hinges, pushrods, horns, servo extensions, glue, straps, LW-PLA, and PETG. The VTOL conversion also needs two 16×500 mm carbon booms.
- **Test equipment:** include a current meter and a suitable thrust-test setup in the build budget.

## Before the first flight

Use the manufacturer's manual for assembly and limits. Confirm mass, centre of gravity, control direction, motor order, failsafe, and power-system capacity. Test control and electrical functions with propellers removed. Perform propulsion tests in a suitable secured test setup. A matching product name or KV value does not establish a safe motor/propeller/battery combination.

No flight test, endurance result, or complete parts compatibility is claimed by this repository.
