Wall Connector 3 Install Manual
Type 2 Handle

Important Safety Information...........................2 Calculating Group Power Management Requirements
for Existing Systems....................................................42
Product Specifications....................................5
Wall Connector LEDs.....................................43
Wall Connector Label.......................................7
Light Codes................................................................43
Power Supply Options.....................................8
Error Codes.................................................................44
Circuit Breaker Rating / Maximum Output......10 Electric Vehicle Service Equipment (EVSE)
Communication Codes................................................46
Using Wall Connector.....................................12
Charging Equipment Limited Warranty..........47
Features.........................................................13
Limits of Liability...........................................48
Connectivity................................................................13
Hosted Access Point....................................................13 Claiming Under the Charging Equipment
Local Network..............................................................13 Limited Warranty...........................................49
Residual Current Device (RCD)....................................14
Dispute Resolution.........................................51
Ground Monitor Interrupter.........................................14
Power Outages............................................................14
Firmware Updates........................................................15
Thermal Monitoring.....................................................15
Wall Connector External Components............16
Wall Connector Internal Components.............17
In the Box.......................................................18
Tools..............................................................19
Installation Considerations............................20
Installation Steps...........................................23
STEP 1: Sizing and Routing Conductor Wires..............23
STEPS 2, 3, 4: Preparing and Mounting the Wirebox...24
STEP 5: Stripping and Securing Wires in Wirebox
Terminals.....................................................................27
STEP 6: Securing Main Unit to Wirebox......................29
Commissioning Procedure............................30
Perform Device Setup..................................................31
Software Updates.......................................................31
Complete Registration................................................31
Address Alerts...........................................................36
System Details...........................................................37
Optional: Access Controls..........................................37
Optional: Dynamic Power Management.......................37
Optional: Group Power Management..........................38
Operating and Error States.........................................39
Group Power Management............................40
Group Power Management Overview..........................40
Breaker and Branch Circuit Setup................................41
Considerations for Group Power Management............42

IMPORTANT SAFETY INFORMATION
Read all instructions before using this product. Save these instructions. Wall Connector features built-in RCD Type A
+ DC 6mA.
This manual contains important instructions for the Tesla Gen 3 Wall Connector that should be followed during
installation, operation, and maintenance. Please review all warnings and cautions before installing and using the Wall
Connector.
WARNING: When using electric products, basic precautions should always be followed, including the
following.
INSTRUCTIONS RELATING TO RISK OF FIRE OR ELECTRIC SHOCK
WARNING: Do not install or use the Wall Connector near flammable, explosive, harsh, or combustible
materials, chemicals, or vapors.
WARNING: Turn off power at the circuit breaker before installing or cleaning the Wall Connector.
WARNINGS
WARNING: Eaton strongly recommends using only type BR breakers that end in H (for instance BR260H) for
continuous loads such as the Wall Connector.
WARNING: This product needs to be mounted on a flat, vertical surface without significant irregularities.
Installations that do not adhere to this requirement are at risk of thermal failure.
WARNING: This device should be supervised when used around children.
WARNING: The Wall Connector must be earthed through a permanent wiring system or an equipment-
earthing conductor.
WARNING: Use the Wall Connector only within the specified operating parameters.
WARNING: Never spray water or any other liquid directly at the wall mounted control box. Never spray any
liquid onto the charge handle or submerge the charge handle in liquid. Store the charge handle in the dock to
prevent unnecessary exposure to contamination or moisture.
WARNING: Do not use the Wall Connector if it is defective, appears cracked, frayed, broken, or otherwise
damaged, or fails to operate.
WARNING: Do not use the Wall Connector if the flexible power cord or cable is frayed, broken, or otherwise
damaged, or fails to operate.
WARNING: Do not attempt to disassemble, repair, tamper with, or modify the Wall Connector. The Wall
Connector is not user serviceable. Contact Tesla for any repairs or modification.
Wall Connector 3 Install Manual 2

IMPORTANT SAFETY INFORMATION
WARNING: When transporting the Wall Connector, handle with care. Do not subject it to strong force or
impact or pull, twist, tangle, drag, or step on the Wall Connector, to prevent damage to it or any components.
WARNING: Do not touch the Wall Connector’s end terminals with fingers or sharp metallic objects, such as
wire, tools, or needles.
WARNING: Do not insert fingers or foreign objects into any part of the Wall Connector.
WARNING: Do not forcefully fold or apply pressure to any part of the Wall Connector or damage it with sharp
objects.
WARNING: Use of the Wall Connector may affect or impair the operation of any medical or implantable
electronic devices, such as an implantable cardiac pacemaker or an implantable cardioverter defibrillator.
Check with your electronic device manufacturer concerning the effects that charging may have on such
electronic devices before using the Wall Connector.
Wall Connector 3 Install Manual 3

IMPORTANT SAFETY INFORMATION
CAUTIONS
CAUTION: Do not use private power generators as a power source for charging.
CAUTION: Incorrect installation and testing of the Wall Connector could potentially damage the vehicle's
battery, components, and/or the Wall Connector itself. Any resulting damage is excluded from the New
Vehicle Limited Warranty and the Charging Equipment Limited Warranty.
CAUTION: Do not operate the Wall Connector in temperatures outside its operating range -30˚C to 50˚C
(-22˚F to 122˚F).
CAUTION: Wall Connector should only be installed by personnel who are trained and qualified to work on
electrical systems.
CAUTION: No adapters or conversion adapters are allowed to be used.
CAUTION: Cord extension sets are not allowed to be used.
CAUTION: This equipment should be installed and operated with a minimum distance of 20 cm between the
radiator and your body.
Wall Connector 3 Install Manual 4

PRODUCT SPECIFICATIONS
This manual applies to Wall Connectors identified by part number 1529455-**-*.
Nominal Voltage and Wiring Single phase configuration Wye transformer configuration Delta configuration
(Service Type) 1-phase 230 V L-N 3-phase 400 V L-L 3-phase 230 V L-L
Nominal Current and Current 1-20(32) A (adjustable by installer)
Range
Imin – Inominal(Imax)
Terminal Blocks Stranded: 4-25 mm2, copper only
Solid: 1.5-20 mm2, copper only
Supported Earthing Scheme TN/TT/IT
Nominal Frequency 50/60 Hz
Cable Length 7.3 m (24 ft)
Wall Connector Dimensions Height: 345 mm (13.6 in)
Width: 155 mm (6.1 in)
Depth: 110 mm (4.3 in)
Wire Box Bracket Dimensions Height: 250 mm (9.8 in)
Width: 120 mm (4.7 in)
Depth: 50 mm (2.0 in)
Weight (including wirebox) 6.8 kg (15 lb)
Operating Temperature -30˚C to 50˚C (-22˚F to 122˚F)
Storage Temperature -40˚C to 85˚C (-40˚F to 185˚F)
Location Non-restricted access
Withstand Current Ratings ( Ipk, 10kA
Icw & Icc)
Enclosure Rating IP 55
Pollution degree 3
Wall Connector 3 Install Manual 5

PRODUCT SPECIFICATIONS
| EMC Classification         | Environment A & B               |                 |
| -------------------------- | ------------------------------- | --------------- |
| Mechanical Protection      | IK08                            |                 |
| Ventilation                | Not required                    |                 |
| Means of Disconnect        | External branch circuit breaker |                 |
| Residual Current Detection | Integrated (Type A + DC 6 mA)   |                 |
| Wi-Fi                      | 2.4 GHz, 802.11b/g/n            |                 |
| Maximum RF power           |                                 |                 |
| RFID                       | 13.56 MHz                       | ERP: 0.0166 mW  |
| UHF                        | 433.92 MHz                      | ERP: 0.00353 mW |
| 2.4GHz Wi-Fi               | 2412-2472 MHz                   | EIRP: 95.5 mW   |
| BLE                        | 2402-2480 MHz                   | EIRP: 1.84 mW   |
| Certifications             | CE, IEC 61851-1 CB              |                 |
Wall Connector 3 Install Manual  6

WALL CONNECTOR LABEL
Each Wall Connector has a label on the exterior side with information that is unique to the product, including the
public key:
• TPN: Tesla Part Number
• TSN: Tesla Serial Number
• Input: Max input power
• Output: Max output power
• MAC: Unique MAC address assigned to the Wall Connector
• SSID: Unique Wi-Fi access point assigned to the Wall Connector
Wall Connector 3 Install Manual 7

POWER SUPPLY OPTIONS
For basic operation, Wall Connector requires an electrical connection to Line 1, Neutral, and Protective Earth (PE)
terminals. Connection to Line 2 and Line 3 terminals is supported for some grid types.
CAUTION: Wall Connector supports 230 V L-N (+/- 10%). Mis-wiring the neutral terminal with >264V to PE
can damage Wall connector
Wall Connector can operate on a three-phase power supply or a single-phase power supply.
Table 1. Most Common Installation Option
Wiring Configuration Option for Five Wires: Line 1, Line 2, Line 3, Neutral, PE
Grid type options:
• 400 V 3-phase Wye
CAUTION: Double check N connection is
230 V L to N at terminals of wirebox
before energizing.
NOTE: Blue is used as the IEC standard for neutral. Some markets may use other colors to symbolize neutral
and line conductors.
Wall Connector 3 Install Manual 8

POWER SUPPLY OPTIONS
Table 2. 2nd Most Common Installation Option
Wiring Configuration Option for Three Wires: Line 1, Neutral, PE
Grid type options:
• 230 V Line to Neutral
CAUTION: Double check N connection is
230 V L to N at terminals of wirebox
before energizing.
Wall Connector 3 Install Manual 9

CIRCUIT BREAKER RATING / MAXIMUM OUTPUT
Power Output
For the best charge rate, install a circuit breaker to match the grid type and desired current output. Wall Connector
features built-in RCD Type A + DC 6 mA.
Maximum current output (amps) can be programmed by the installer as part of the commissioning process. Any
amperage between 6 A and 32 A can be selected. See the estimate power output for various grid connections below:
NOTE: To ensure that the desired current output of Wall Connector can be delivered continuously for multiple
hours, a circuit breaker has to be selected that adheres to local regulations and design best practices. The
table below provides a guideline for circuit breaker derating to avoid nuisance tripping. Regardless of the
breaker size, cables smaller than 4 mm2 stranded should not be used to connect the Wall Connector to the
breaker. Refer to the next page for additional information regarding cable size.
NOTE: Some Tesla vehicles may draw less current than the max output of Wall Connector. Actual charging rate
depends on Wall Connector output and onboard charger in the vehicle. See Tesla website for vehicle
specifications.
NOTE: Refer to local regulations regarding any disconnect requirements.
NOTE: See Commissioning Procedure on page 30 for details on how to set maximum amperage.
Wall Connector 3 Install Manual 10

CIRCUIT BREAKER RATING / MAXIMUM OUTPUT
Branch Circuit Conductors and Earth Wire
NOTE: Eaton strongly recommends using only type BR breakers that end in H (for instance BR260H) for
continuous loads such as Universal Wall Connector.
• Refer to local electrical code to select correct conductors and earth wire size that are suitable for the chosen
circuit breaker.
• Wall Connector wirebox terminals can accept stranded wire sized between 4 mm2 to 25 mm2, or solid wire 1.5
mm2 to 25 mm2. Installer is responsible for selecting a wire size that will be compliant with local code, possibly
taking into account amperage, distance and other site conditions.
NOTE: If using stranded wiring smaller than 4 mm2, use a correctly sized ferrule so it can be securely
terminated.
• For sites with multiple Wall Connectors, each Wall Connector must have its own branch circuit and dedicated
circuit breaker.
• For outdoor installations, use watertight fittings when securing feeder wires to the wirebox.
• For this installation guide, IEC standard colors are used for L1, L2, L3, Neutral, and PE. Some regions may use
other standardized colors.
Earth Connections
Wall Connector must have an earth path back to the main equipment earthing point on site. Without a proper earth
connection, the Wall Connector will not charge a vehicle during an earth assurance test. Equipment-earth conductor
must be run with the circuit conductors and connected to the equipment-earth terminal in the wirebox. Install an
earth wire sized according to local electrical code.
NOTE: To support TT and IT grids, earth assurance can be disabled as part of the commissioning process.
Earth assurance must always be enabled for TN grids.
Wall Connector 3 Install Manual 11

USING WALL CONNECTOR
1 . Open the vehicle charge port by the following methods:
a. Press the button on the charge handle.
b. Press on the charge port door.
c. Open the vehicle charge port by using the mobile app, using the vehicle touchscreen, or by pressing and
holding the trunk button on the keyfob.
2 . Insert the charge handle into the vehicle charge port.
3 . Check the vehicle controls to verify charging.
4 . To remove the charge handle from the vehicle, press and hold the button on the handle to unlock the charge
port.
NOTE: The vehicle must be unlocked to remove the charge handle.
5 . Remove the charge handle from the vehicle charge port.
6 . Wrap the charge cable counter-clockwise around the Wall Connector and insert the charge handle into the
holster.
Wall Connector 3 Install Manual 12

FEATURES
Connectivity
Wall Connector is equipped with Wi-Fi to communicate with local site routers, vehicles, mobile devices, other Wall
Connectors, and other Tesla products.
Hosted Access Point
Wall Connector hosts a WPA2 password-secured, 2.4 GHz, 802.11 Wi-Fi access point network to facilitate
commissioning and connecting to other devices.
A unique SSID Wi-Fi network name and WPA2 password for connecting to the Wall Connector are printed on a label
at the rear of the main unit, as well as on the front cover of the Quickstart Guide included in the box.
Local Network
Connecting Wall Connector to a local Wi-Fi network enables it to receive over-the-air firmware updates, remote
diagnostics access, and usage data tracking capability. A Wi-Fi connection is required for sites that utilize
authentication, billing, and other property management features.
NOTE: New features and fucntions will be added over time.
Wall Connector only supports WPA2 secured, 2.4 GHz, 802.11 infrastructure mode networks.
Wall Connector 3 Install Manual 13

FEATURES
NOTE: Networks that are not password protected are not supported. The Wall Connector will not display non-
password protected networks in the options list.
Residual Current Device (RCD)
The Wall Connector features an RCD Type A function with DC 6mA detection and disconnection capabilities. Local
wiring regulations always take precedence.
AC earth fault interruption automatically detects an AC current mismatch between power delivery conductors that
would indicate that current is flowing through the earth conductor. AC fault protection will trip at 20 mA.
DC earth fault interruption automatically detects DC leakage through earth. DC fault protection will trip at 6 mA.
User interaction such as pressing the cable button or unplugging from vehicle is required to clear this fault. If the fault
continues, consult with an electrician to review the power supply.
Ground Monitor Interrupter
The ground monitor interrupter allows the installer to select different early monitor options. Wall Connector
continuously checks for the presence of a safe earth connection and automatically recovers from faults. Earth
assurance operates by injecting a small amount of current into the earth conductor in order to measure the
impedance between line and earth. If high impedance is detected, the Wall Connector will lock out charging and
display an error code of two (2) red blinks. See Error Codes on page 44 for a full list of error codes.
For earth assurance to operate on TN grids, one leg of the distribution transformer must be earth-bonded (Neutral).
Earth bond should only occur at one location in a site's electrical system.
Wall Connector earth assurance may be adjusted in countries with TT or IT grid configurations and can be disabled in
the commissioning procedure.
The Earth Monitor Interrupter feature monitors the Wall Connector earth connection. Select the correct option based
on the installation's earthing system and earth impedance.
Depending on country, three options are available:
• Enable: Earth connection will be monitored and a high detected earth resistance will disable the Wall
Connector. This is the preferred setting to provide protection and should be selected where earth connection
is expected to be strong (as in the case on TN networks and most TT networks), and where required by
regulation.
• Disabled: Earth connection will not be monitored. This should be selected where the earth connection is not
made (as is the case for IT networks), or where the current induced by this check would be problematic (as is
the case on some TT networks with sensitive residual-current devices).
Temporary problems such as earth faults or utility power surges are resolved automatically.
Power Outages
If there is a power outage while Wall Connector is charging a vehicle, charging will automatically resume within 1 to 3
minutes after power restoration. The Wall Connector will display a solid blue light on the faceplate to indicate that it is
communicating with the vehicle and waiting to resume charging. Alternatively, pressing the button on the charge
handle after power restoration will cause Wall Connector to resume charging immediately.
NOTE: Wall Connectors in a power management group maintain their group power management settings after
a power loss event.
Wall Connector 3 Install Manual 14

FEATURES
Firmware Updates
Firmware updates will be automatically applied to the Wall Connector to improve the user experience and introduce
new features. Connect Wall Connector to Wi-Fi for access to the most recent firmware update. See Commissioning
Procedure on page 30.
Thermal Monitoring
Wall Connector actively monitors temperatures in multiple locations while charging to ensure stability of the charge
session. Temperature sensors are located at the relays, microcontroller, and charge handle to monitor the
temperature of the terminals in the wirebox.
In warmer conditions, Wall Connector may reduce current and charge speed to protect itself. When this happens, the
light bar on the faceplate will continue to display the “streaming green” and a blink code of three red flashes to
indicate that charging has been reduced due to high temperatures. If heat continues to rise, Wall Connector will stop
charging and display a blink code of three red flashes.
NOTE: See Error Codes on page 44 for full list of error codes.
For optimal performance, install Wall Connectors in areas where ambient temperature will remain below 50˚C
(122˚F). In rare circumstances, Wall Connector may begin reducing amperage at 35˚C (95˚F) ambient temperatures.
Adjustments to amperage are automatic and do not require user input; Wall Connector will return to starting current
when temperatures are reduced.
Wall Connector 3 Install Manual 15

WALL CONNECTOR EXTERNAL COMPONENTS
"Wall Connector" refers to the product as a whole.
1 . Faceplate
2 . Light bar (vertical)
3 . Main unit
4 . Charge handle button
5 . Charge handle
Wall Connector 3 Install Manual 16

WALL CONNECTOR INTERNAL COMPONENTS
1 . Contact blades
2 . Temperature sensor
3 . Conductor terminals
4 . Zip tie anchor
5 . Sliding contacts
6 . Wirebox drainage opening (enables protection)
7 . Neutral
8 . Line 1
9 . Line 2
1 0. Line 3
1 1. Earth
Wall Connector 3 Install Manual 17

IN THE BOX
Hex Bit (4 mm)
Main Unit Wirebox Mounting Template
Wirebox
Wirebox-to-Wall Fastener (x2)
Wall Connector-to- 4.0 x 50 mm (PZ2)
Wirebox Fastener (x4)
Zip tie (x1)
(#8 x 2 in)
Quickstart Guide (contains
sticker with SSID network
name and unique password)
NOTE: The hex bit, zip tie, and fasteners are located in a plastic bag inside the wirebox, which comes attached
to the main unit of the Wall Connector.
NOTE: Wall plugs are not included. If installing in concrete or other like materials, use 6 mm wall plugs.
Wall Connector 3 Install Manual 18

TOOLS
Required Tools
NOTE: Drill bit sizes assume wood mounting surfaces. If installing on concrete or other masonry, consult with
an electrician for optimal pilot hole sizes.
Stud Finder
Torque Driver (5.6 Nm, 50 lbf . in) (If installing on wood walls)
Multimeter Tape Measure
Drill Bit, 5 mm (3/16 in) Drill Bit, 2.5 mm (3/32 in) Bit Driver
Wire Stripper
(If installing on wood walls) (If installing on wood walls)
Level
Smartphone (with Wi-Fi) Power Drill
Optional Tools
Step Bit, 29 mm (1-1/8 in) Step Bit, 35 mm (1-3/8 in)
Computer (with Wi-Fi)
Wall Connector 3 Install Manual 19

INSTALLATION CONSIDERATIONS
Wall Connector may be installed on any flat, vertical surface capable of supporting its weight (e.g. wall, pedestal,
etc.). Wall Connector (wirebox, faceplate, and long cable) weighs 6.8 kg (15 lb).
Choosing Location
Install Wall Connector in a location that allows the charge cable to reach the vehicle charge port without putting strain
on the cable. Recommended installation area for Wall Connectors with 24 ft (7.3 m) cable:
Install Wall Connector in a location with ample clearance on all sides to allow the charge cable to loop around the unit
and the charge handle to comfortably land in the side dock.
NOTE: If constrained by space, a cable organizer can be installed near the Wall Connector.
Wall Connector 3 Install Manual 20

INSTALLATION CONSIDERATIONS
Choosing Height
• Maximum height (indoor and outdoor): 1.52 m (60 in)
• Recommended height: ~1.15 m (~45 in)
• Minimum outdoor height: 0.6 m (24 in)
• Minimum indoor height: 0.45 m (18 in)
Maximizing Wi-Fi Signal Reception
Wall Connectors should be connected to a local Wi-Fi network for optimal functionality. For maximum signal
reception, avoid installing Wall Connector on opposite sides of concrete, masonry, metal studs, and other physical
obstructions that could impede Wi-Fi signal reception.
NOTE: If a mobile device is able to connect to local Wi-Fi at a given location, it is a good indication that Wall
Connector will also be able to connect.
Wall Connector 3 Install Manual 21

INSTALLATION CONSIDERATIONS
Wire Entry Options
Wall Connector's wirebox has multiple wire entry options. Choose one entry path and follow installation instructions
based on chosen entry path.
1 . Top entry location
2 . Rear entry locations (left or right)
3 . Bottom entry location
Wall Connector 3 Install Manual 22

INSTALLATION STEPS
STEP 1: Sizing and Routing Conductor Wires
Pull excess wire first, then cut to length. Use a wire stripper to cut each conductor wire appropriately based on entry
point and position. Attach the conduit/fittings and route each conductor wire into the wirebox so it lands in the
correct terminal.
NOTE: Insulation wire colors may vary based on market.
For Top Wire Entry
Wire lengths/proportions shown are not to scale.
For Bottom (1), Rear Left (2), or Rear Right (3) Wire Entry
Wall Connector 3 Install Manual 23

INSTALLATION STEPS
Wire lengths/proportions shown are not to scale.
STEPS 2, 3, 4: Preparing and Mounting the Wirebox
This procedure has 4 different variations depending on the chosen wire entry option, but the general order of steps
will be the same for all wire entry options:
1 . Drill 5 mm holes into the wirebox*. If wiring for rear entry, use step bit.
2 . Use cardboard template to plan or drill pilot holes into mounting surface*. A 2.5 mm pilot hole is recommended
for most surfaces.
NOTE: Drill larger pilot holes that can accommodate 6 mm wall plugs if installing on concrete, masonry,
or similar materials.
NOTE: Installer can adjust pilot hole size based on mounting surface
NOTE: Use a level to ensure that the template is completely level.
3 . Attach wirebox to mounting surface using included fasteners, which include an integrated sealing washer. The
fastener head is compatible with both #2 Phillips or #2 square head bit. Attach conduit/fittings and bring in
conductor wires*.
NOTE: It is the responsibility of the installer to select appropriate conduit/fitting materials for the
installation.
*Exact locations depend on the wire entry option
Wall Connector 3 Install Manual 24

INSTALLATION STEPS
Table 3. For Top Wire Entry
| For Top Entry | 1   | 2   | 3   |
| ------------- | --- | --- | --- |
Table 4. For Bottom Wire Entry
| For Bottom Entry | 1   | 2   | 3   |
| ---------------- | --- | --- | --- |
Table 5. For Rear Left Wire Entry
| For Rear Left Entry | 1   | 2   | 3   |
| ------------------- | --- | --- | --- |
Wall Connector 3 Install Manual  25

INSTALLATION STEPS
Table 6. For Rear Right Wire Entry
For Rear Right Entry 1 2 3
CAUTION: Wall Connector is IP 55 rated and does not need caulking. Refrain from using any bonding, sealant,
or adhesives as part of the Wall Connector installation. The provided screws have sealant washers which
provide adequate sealing.
Installer is responsible for providing appropriate glands, fittings, and conduit to secure incoming power
supply to Wall Connector wirebox. Top and bottom entry are 28 mm in diameter when sealing plug is removed.
If needed, bottom entry can be expanded using a step bit. Do not expand top entry.
Wall Connector 3 Install Manual 26

INSTALLATION STEPS
STEP 5: Stripping and Securing Wires in Wirebox Terminals
1 . Use a wire stripper to strip the ends of each wire to ~12 mm.
2 . Insert each stripped wire into the correct terminal.
NOTE: If using stranded wiring smaller than 4 mm2, use a correctly sized ferrule so it can be securely
terminated.
3 . Use the included bit to torque each terminal to 5.6 Nm (50 lbf.in). Use zip ties to secure wires to service loop
on the left side of the wirebox.
Wall Connector 3 Install Manual 27

INSTALLATION STEPS
4 . Use scissors to cut excess plastic off zip tie after securing in place. Ensure no wiring or other obstruction
crosses over the terminal block screws before proceeding to the next step.
Wall Connector 3 Install Manual 28

INSTALLATION STEPS
STEP 6: Securing Main Unit to Wirebox
1 . Attach the main unit to the wirebox.
2 . Secure the main unit to the wirebox with the 4 included fasteners using the included bit. Use a bit driver to
hand-tighten the fasteners.
Wall Connector 3 Install Manual 29

COMMISSIONING PROCEDURE
The commissioning process for Wall Connector enables easy configuration of circuit breaker size, Wi-Fi connectivity,
and group power management options.
The Quick Start Guide is included with the Wall Connector and contains a QR code that is used to connect to Wall
Connector to perform device setup.
NOTE: Ensure the Quick Start Guide is not discarded as the QR code may be required in the future!
CAUTION: Start the process only when the Wall Connector is powered on. Do not connect to any load when
the face plate is separated from the main unit.
1 . Using the smartphone camera, scan the QR label on the Quick Start Guide.
◦ If the Tesla One app has not yet been installed, follow the prompts to install the app.
◦ If the Tesla One app is already installed, ensure it has been updated to version 10.8 or greater (select
More, then select Settings, then the app version to see if an update is available).
NOTE: Tesla One gets new features every week, so update frequently! The app should
automatically update but it is best practice to check for new updates, and manually update when
one is available.
2 . Log in to Tesla One using your Tesla Partner Portal account, or select Create Account to create a new account.
NOTE: Apple users may be prompted to allow Tesla One to find and connect to devices on the local
network. Select Allow or OK, as this is required to connect to the Wall Connector Wi-Fi network. If the
prompt does not automatically appear, permission can be granted by selecting Settings > Apps > Tesla
One > Local Network.
NOTE: Android users may be prompted to allow Location Consent. Allow all the time or Allow only while
using the app, as this is required to allow Tesla One to find and connect to devices. If the prompt does
not automatically appear, permission can be granted by selecting Settings > Apps > Tesla One>
Location.
3 . Select Tesla Device Setup, then select Begin.
Wall Connector 3 Install Manual 30

COMMISSIONING PROCEDURE
4 . Select Scan QR Code, then use the smartphone camera to scan the QR code on the Quick Start Guide again.
5 . On the charge handle, press and hold the handle button for 5 seconds. Wait for the LED to pulse green, then
select Join.
Perform Device Setup
1 . Select Installation Settings.
2 . Select the appropriate Country. Then select Breaker Size (A).
3 . Select Wi-Fi to connect Wall Connector to the homeowner’s network. The Wall Connector can be connected to
a network manually or by selecting from the available networks.
When connection is complete, Wall Connector will display Wi-Fi as connected.
NOTE: Wall Connector is only compatible with 2.4 GHz networks.
Software Updates
1 . Select Software Update to ensure the latest software is installed.
2 . Select Update if a software update is available.
Complete Registration
Installer Registration
Installer registration is an important step for tracking install quality, and it allows the installer (and partner(s) if
applicable) to view the site in Powerhub.
NOTE: The site is only created in Powerhub after customer registration is completed. Installer registration
allows the installing company to view the site in Powerhub, but customer registration must be completed for
the site to exist in Powerhub.
Wall Connector 3 Install Manual 31

COMMISSIONING PROCEDURE
NOTE: Once installer registration has been completed, it cannot be changed in Tesla One and instead must be
updated by Install Support.
To complete installer registration:
1 . Select Registration > Installer Info and enter your contact information.
a. In the Company Name field, verify that the name of the company performing the installation has
automatically been filled in. If the company name is not present or is not correct, search for your
company to select it.
NOTE:
▪ The Company Name is the field that links a partner to a site, meaning this is the field that
allows a company to view the site in Powerhub.
▪ If you are not a Tesla Certified Installer, please select Unknown for the company name
field, and then manually type your company name, if applicable.
b. In the Email field, leave the email address of the installer completing the installation. This email address
is used to track Tesla Academy training completion and the Pro Score inside Tesla One.
2 . To add a partner installer company:
a. Select Add Partner and search for the partner name to select it.
b. Repeat this step if needed (up to two partner companies can be added).
Wall Connector 3 Install Manual 32

COMMISSIONING PROCEDURE
NOTE: This feature enables another company or entity to access the site in Powerhub. For instance, if
another company is performing the installation, sold the system, owns the system, or distributes the
hardware in region, they can be given Powerhub access to the site this way.
NOTE: If the site is not shared with partner companies during device setup, it can be shared using
Powerhub. See Site Sharing in the Residential Powerhub User Manual for instructions to share the site
with partners.
3 . Select Continue to proceed to the customer registration.
Site Visibility in Powerhub
Tesla products appear in the Powerhub Fleet Monitoring Portal after Customer Registration is completed, and if the
Company Name was present during commissioning per the above steps.
If a site is not visible in Powerhub:
1 . Make sure the site was registered, meaning the customer can see it in their Tesla App.
2 . Contact the company that installed the system (or a partner company with site sharing capability) and ask them
to share the site in Powerhub. See Site Sharing in the Residential Powerhub User Manual for more information.
Wall Connector 3 Install Manual 33

COMMISSIONING PROCEDURE
Customer Registration
Customer registration allows the customer to view their system in the Tesla app, and the customer’s product warranty
is activated upon registration.
Tesla has two paths for customer registration:
• Option 1 (Installer-Led Registration, preferred):
1 . Select Enter Customer Info.
2 . Enter the customer's email address, then select the Next button.
3 . Complete the registration form.
NOTE: The customer email address entered during registration is the link between the product
and the customer's Tesla account. Please ensure that the email address is entered correctly and is
the one used by the customer for their Tesla account.
• Option 2 (Customer-Led Registration): If the customer is available, select Show a code or Text the customer to
allow the customer to enter their information. Both of these methods open the Tesla app to the Add Products
page; the customer can also navigate to Add Products manually.
NOTE: If customer registration is not completed, the customer will not have access to the system in the mobile
app. Ensure customer registration is completed!
Multi-Product Customer Registration
Each Wall Connector is separate, meaning each must be commissioned and registered individually. Failure to fully
register all products will result in loss of Powerhub visibility, loss of customer app visibility, and unactivated
warranties.
If a customer has multiple Tesla devices (Wall Connector(s) and/or Powerwall), all devices can be registered to the
same site for simplified viewing in Powerhub (for the installer) and the Tesla app (for the customer).
NOTE:
• This feature can be used in the following installation scenarios:
◦ Adding multiple Wall Connectors to a single site
◦ Adding Wall Connector to a Powerwall site (or vice versa)
• For complex edge cases, Tesla Support remains available to correct registration issues after the
registration process is completed
Options for registering multiple devices to a single site:
• Option 1 (Installer registers devices, preferred):
1 . Register one of the devices.
2 . For each subsequent device:
a. Connect to the device in Tesla One and, during the registration step, enter the customer's email
address.
Wall Connector 3 Install Manual 34

COMMISSIONING PROCEDURE
b. If the first device was registered within the last 24 hours by the same installer (using the same
mobile device), the Add to Recent Site option will appear with the customer's registration
information. Select this option.
c. If the Add to Recent Site option is not available, select the Next button.
d. Select the existing site.
NOTE: Existing sites belonging to the same customer email address and the installer's
Powerhub instance will be displayed.
Wall Connector 3 Install Manual 35

COMMISSIONING PROCEDURE
e. Select Register.
• Option 2 (Customer registers devices): Customers can register additional devices to their existing account
using the Add Product page in the Tesla app.
If either of these options fails for any reason, email to have them manually register the additional devices. Provide the
following information:
1 . Customer Name
2 . Customer Address
3 . Customer Email (associated with their Tesla Account, matching what was entered by the installer)
4 . Already registered equipment DIN (Device Identification Number: Part Number & Serial Number
5 . Additional DINs that need to be registered and added to the existing Site
Address Alerts
The Alerts tray is displayed at the bottom of the page if any alerts are present, and is a shortcut for the installer to
address important issues. The Alerts tray displays critical errors that the installer must take action on.
Alert Types
Some alerts are used to help explain what the system is doing:
• Software Update
Some alerts are used to indicate an issue the installer needs to address:
• Installation settings not configured
Wall Connector 3 Install Manual 36

COMMISSIONING PROCEDURE
Alert Icons
Icon Name Description
Process The system is carrying out a process; wait for it to complete
Success This task has been completed successfully
Warning There may be an issue; the installer should review
Error There is an issue that will prevent the system from functioning; action is required by the installer
System Details
1 . Select System Details to access more information about the Wall Connector System.
Optional: Access Controls
1 . Select Access Controls to configure which specific vehicles can access Wall Connector.
2 . From the Access Control menu, select the level of access control as determined by the customer:
◦ All Vehicles: default option, any vehicle can charge from this Wall Connector.
◦ Only Teslas: any Tesla can charge from this Wall Connector.
◦ Authorized Teslas Only: only Teslas configured in device setup or Tesla app can charge from this Wall
Connector.
◦ Compatibility Mode: This option allows Wall Connector to be compatible with older generation vehicles.
Use it only if you experience faults with your Wall Connector and your electric vehicle. Note that you will
lose some software functionality in utilizing this mode.
3 . If configuring Authorized Teslas Only, select Add to enable access for new vehicles. Enter the VIN(s) of the
vehicle(s) the customer would like to authorize. The customer can also add vehicles in the Tesla app.
Optional: Dynamic Power Management
Dynamic Power Management enables Wall Connector to dynamically adjust EV charging power based on live readings
of the overall load in the panel. An energy meter is installed to MONITOR live current in the panel; when panel loads
are reduced, Wall Connector is able to increase charging current up to a limit set by the installer.
NOTE: As described in the , Wall Connector should be installed with a 40A circuit breaker for maximum power
output; if there is not enough room for the recommended breaker size in the electrical panel, a smaller breaker
can be installed with a lower amperage configuration (see the application note for more information).
1 . Once connected, the Remote Energy Meter will automatically be detected. Select Meter to configure CTs and
set the Max Conductor Limit.
Wall Connector 3 Install Manual 37

COMMISSIONING PROCEDURE
NOTE: The Remote Energy Meter has four CT ports, with the following voltage references:
◦ CT1: L1
◦ CT2: L2
◦ CT3: L3
◦ CT4: L1
2 . Select the Neurio meter to configure the CTs.
3 . For each of the connected CTs, select the CT and set the Location to Conductor.
4 . On the Meter screen, set the Max Conductor Limit. This value should be 80% of the electrical panel’s rated
limit.
See the for instructions to test the system and troubleshoot as needed.
Optional: Group Power Management
Power sharing can only be done in a group of six wall connectors (one leader + five followers). Finish commissioning
the followers before commissioning the leader. Additionally, make sure that all the followers have a good line of sight
to the leader. For more information, see Group Power Management on page 40.
1 . Select Power Sharing to connect additional Wall Connectors.
2 . Toggle off Power Sharing to make settings adjustments.
3 . To add a new Wall Connector, select Scan QR Code then scan the Wi-Fi QR code on the new Wall Connector's
Quick Start Guide.
4 . Select Add Follower to add the new Wall Connector.
5 . Select Done once the leader is reconnected and the follower has successfully been added.
6 . Enable the power sharing network.
Program Network Limit
1 . Select Power Sharing Settings to program a network limit.
2 . Enter the appropriate network limit:
NOTE: This is the maximum total current a power sharing network is allowed to consume in amps. This
represents the continuous current which the network will not exceed. An electrician will need to
determine the correct amount of amperage and confirm that the load center has appropriate
overcurrent protection.
Expected Behaviors
• SSID access point of all Leader Wall Connectors in a power sharing network will continue to broadcast.
• Removing a Wall Connector from a network will temporarily set that device’s max output to 6 amps. Cycle
circuit breaker to reset Wall Connector to original configuration setting.
• Leader Wall Connector will share site Wi-Fi with follower Wall Connectors.
Wall Connector 3 Install Manual 38

COMMISSIONING PROCEDURE
Operating and Error States
Operating States
Ready: Wall Connector is ready to charge.
Charging: Connected to the internet and charging the car.
Unplugged: Connected to internet but not connected to car.
Waiting for vehicle: Charger is plugged in, and a charge session needs to be initiated in the vehicle or through the app.
Error States
Critical fault: Needs to be monitored. If it lasts for over 3 days, call Tesla Service.
Non-critical fault: Charging blocked due to authentication error, call Tesla Service.
Offline: Wall Connector does not have good connectivity and cannot connect to Tesla Servers. Contact your Tesla
Certified Installer.
Error Codes
Error Solution
Device is already registered on the same site and shows a Refresh the device list.
warning.
Device is already registered to a different site. Remove from Warp and try to register again/Flag to
Tesla team members.
Firmware is not up to date to minimum 22.33.1 Update firmware. (Side load).
Request ID cannot be found in error logs. Send a ticket to the Engineering team.
Wall Connector 3 Install Manual 39

GROUP POWER MANAGEMENT
Group Power Management Overview
The firmware-based group power management feature enables up to 6 Wall Connectors installed at the same site to
intelligently share the site's total available power via unit-to-unit Wi-Fi. This minimizes the need for many residential
and commercial applications to have specific electrical upgrades for concurrent multi-vehicle charging.
During the commissioning process,
• Wall Connectors are allocated to individual branch circuits (each up to 40A)
• Total power is allocated to the group of linked Wall Connectors
NOTE: For instructions to commission Wall Connectors in a group power management network, see the
Commissioning Procedure on page 30.
Total current output of Wall Connectors that share power will never exceed the site's total allocated power.
1 . AC feed (service panel)
2 . Group power management via Wi-Fi communication
Wall Connector 3 Install Manual 40

GROUP POWER MANAGEMENT
Breaker and Branch Circuit Setup
Group Power Management circuits may be installed in an electrical panel that supports other loads. If space is limited
or the main power supply is far from the Wall Connectors, installing a dedicated load center or single branch circuit
may be prudent.
See below for examples of Wall Connector group power management diagrams (one with sub-panel and one without).
Each individual Wall Connector in below examples is capable of providing 32A amps when it is the only one in use. As
more Wall Connectors begin plugging into vehicles, the system will automatically distribute power based on the total
power allocated to the site.
Group Power Management Setup with Sub-Panel
1 . Wall Connector
2 . Branch circuit
3 . Sub-panel / feeder breaker
Group Power Management Setup Without Sub-Panel
1 . Wall Connector
2 . Branch circuit
Wall Connector 3 Install Manual 41

GROUP POWER MANAGEMENT
Considerations for Group Power Management
Wall Connector group power management is achieved wirelessly.
For optimal performance, Wall Connectors within a group power management network should be installed within view
of each other whenever possible.
NOTE: Line of sight is recommended but not required. Wireless communication is capable of reaching around
concrete corners but network range may degrade as a result.
Avoid placing Wall Connectors on opposite sides of concrete, masonry, metal studs, and other physical obstructions
that would impede Wi-Fi signal strength.
Calculating Group Power Management Requirements for Existing Systems
To calculate power supply requirements per number of Wall Connectors for existing electrical systems, use the
following equation:
Available continuous amperage: Number of Wall Connectors: Max amperage output per Wall Connector when
100% utilized:
_____________________ ÷ ________________________ = ________________________
NOTE: Maximum number of Wall Connectors for group power management is 6.
NOTE: When calculating maximum amperage per Wall Connector, 100% utilization must be greater than 6
amps for group power management operation. If maximum amperage is greater than 32A amps, group power
management is not necessary.
For large scale sites, consider expected parking time in relation to a 100% utilization rate.
Expected Park Time (hours) Examples Recommended Amperage per Wall
Connector at 100% Utilization
6+ (long term) Long term parking, overnight 12+ amps
parking
3-5 (medium term) Workplace, hospitality 24+ amps
1-2 (short term) Shopping and dining 32+ amps
NOTE: 100% utilization represents the worst case scenario for charging speeds, where the least amount of
power would be available for each individual vehicle. In most situations, not all Wall Connectors would be
actively charging a vehicle, which enables faster charging for the remaining vehicles.
Wall Connector 3 Install Manual 42

WALL CONNECTOR LEDS
Light Codes
Startup
Once energized at the circuit breaker, every LED (seven total) on the faceplate will illuminate for up to five seconds.
Other
After startup,  Waiting to charge,
| Standby, waiting to  | Charging in  | SSID broadcasting,  |     |
| -------------------- | ------------ | ------------------- | --- |
waiting for  communicating with
| plug in | progress | ready to commission |     |
| ------- | -------- | ------------------- | --- |
commissioning vehicle
Solid yellow (green +  Every green
| Top green solid |     | Green pulsing | Blue solid |
| --------------- | --- | ------------- | ---------- |
red) streaming
NOTE: If a red dot is displayed, connect to Wall Connector Commissioning or see next table for all error codes.
Wall Connector 3 Install Manual  43

WALL CONNECTOR LEDS
Error Codes
All red blink codes pause for one second, and then repeat.
Light Bar What It Means Details
No Lights Power supply issue, Verify that the power supply is turned on. If the issue persists, have an
charging disabled electrician remove the Wall Connector from the wirebox and confirm that
voltage is present at the terminal block using a multimeter. Record
measurements at terminals of wirebox.
Solid yellow Wall Connector is ready See Commissioning on page 30 to commission the Wall Connector.
to be commissioned
Solid red Internal error, charging Turn the circuit breaker off, wait 5 seconds, and turn it back on. If solid
disabled red light remains, document part number and serial number, then contact
Tesla Energy.
Earth fault circuit Inspect the handle, cable, Wall Connector, and vehicle charge port for
One (1) red interruption due to damage or signs of water ingress. Contact Tesla Energy if power supply
blink unsafe current path, has been checked and confirmed as okay by an electrician.
charging disabled
Earth assurance fault, Verify that the Wall Connector is properly connected to earth. The earth
Two (2) red high earth resistance connection must be bonded in the upstream power supply for proper
blinks detected, charging operation. Check all physical connections, including the wirebox
disabled terminals, electrical panel(s), and junction boxes. If connected to a
transformer, contact the transformer's manufacturer for direction on how
to bond the earth connection. If charging on a IT or TT grid, check ground
monitor settings.
High temperature Verify that Wall Connector is connected to Wi-Fi and updated with the
Three (3) red detected; charging latest available firmware for optimal temperature sensing functionality.
blinks limited or disabled Check the faceplate and cable handle for excessive warmth. Have an
electrician remove the Wall Connector from the wirebox and verify that
the conductors used are sized correctly and that the terminal block is
torqued to specification. Connect Wall Connector to Wi-Fi so that
firmware can update to most recent version. If firmware does not
automatically update, use the Commissioning on page 30 procedure to
sign into the commissioning wizard and manually update the firmware. If
it does not solve the problem, contact our Customer Support team.
Internet connection lost, Check for objects that could interfere with the area's Wi-Fi signal
Four (4) red online features disabled strength. Confirm that the local Wi-Fi router is operational. If the Wi-Fi
blinks password was changed recently, follow the commissioning process on
your mobile device to update the Wi-Fi settings.
Group power Check for objects that could interfere with the area's Wi-Fi signal
Five (5) red management strength. Follow the commissioning process on your mobile device to re-
blinks communication issue, link the Wall Connectors for group power management.
charging reduced
Six (6) red Overvoltage or poor grid Connect to Wall Connector with commissioning process to view live
blinks quality detected, voltage info. If the issue persists, have an electrician remove the Wall
charging disabled Connector from the wirebox and confirm that voltage readings are as
expected at the terminal block using a multimeter. Record voltage
readings at terminals.
Wall Connector 3 Install Manual 44

WALL CONNECTOR LEDS
All red blink codes pause for one second, and then repeat.
Light Bar What It Means Details
Seven (7) Vehicle overcurrent Reduce the vehicle's charge current setting. If the issue persists and the
red blinks detected attached vehicle is manufactured by Tesla, record the vehicle's VIN and
approximate time of the fault and contact Tesla. If the vehicle is not
manufactured by Tesla, contact the vehicle's manufacturer.
Wall Connector 3 Install Manual 45

WALL CONNECTOR LEDS
Electric Vehicle Service Equipment (EVSE) Communication Codes
Light Bar Meaning Details
Connected to Vehicle, Electric Vehicle Verify vehicle is ready to charge and not blocked
Solid blue Service Equipment ready but vehicle not by settings like scheduled charging
requesting charge
Establishing communications with vehicle
Blue "breathing"
Connected to Vehicle, Electric Vehicle Verify device configuration to ensure settings
Two (2) blue blinks Service Equipment not ready to charge like scheduled charging, Open Charge Point
Protocol, or access control are not preventing
charging
Wall Connector 3 Install Manual 46

CHARGING EQUIPMENT LIMITED WARRANTY
Subject to the exclusions and limitations described below, this Charging Equipment Limited Warranty covers the
refund, repair or replacement necessary to remedy any manufacturing defects in a Tesla manufactured and supplied
Wall Connector that occur under normal personal use for a period of 48 months, or a period of 12 months for normal
commercial use*, and a Tesla manufactured and supplied Mobile Connector or charging adapter that occur under
normal use for a period of 12 months, starting from the date of invoice to the customer for any charging equipment.
Any Tesla manufactured and supplied connector or adapter included in the initial purchase and delivery of a Tesla
vehicle by Tesla is covered under the Basic Vehicle Limited Warranty section of the New Vehicle Limited Warranty for
4 years or 50,000 miles (80,000 km), whichever comes first, subject to the terms and conditions of the New Vehicle
Limited Warranty.
*For warranty claims specific to Wall Connectors, “commercial use” means Wall Connectors used for purposes other
than charging at a residential single family home for daily personal use, which includes, but is not limited to, charging
at hotels, offices, parking lots and complexes (including apartment, condominiums and other multi-family or unit
dwellings), and retail and other locations that allow (including by being listed online or publicly) for pay-for-use
charging, or are located where users other than the owner could reasonably obtain access to the Wall Connector.
This Charging Equipment Limited Warranty does not cover any damage or malfunction directly or indirectly caused
by, due to, or resulting from, normal wear or deterioration, abuse, misuse, negligence, accident, lack of or improper
installation, use, maintenance, storage or transport, including, but not limited to, any of the following:
Failure to follow the instructions, operation, maintenance and warnings published in the documentation supplied with
your Tesla connector or adapter;
External factors, including but not limited to, objects striking the Tesla connector or adapter, faulty or damaged
electrical wiring or connections, external electrical faults, junction boxes, circuit breakers, receptacles or power
outlets, the environment or an act of God, including, but not limited to, fire, earthquake, water, lightning and other
environmental conditions;
General appearance or damage to paint, including chips, scratches, dents and cracks;
Failure to contact Tesla upon discovery of a defect covered by this Charging Equipment Limited Warranty;
Any repair, alteration or modification to the Tesla connector or adapter or any part, or the installation or use of any
parts or accessories, made by a person or facility not authorized or certified to do so; and
Lack of or improper installation, repair or maintenance, including use of non-genuine Tesla accessories or parts.
Although Tesla does not require you to perform all maintenance, service or repairs at a Tesla Service Center or Tesla
authorized repair facility, this Charging Equipment Limited Warranty may be voided, or coverage may be excluded,
due to lack of or improper maintenance, service or repairs. Tesla Service Centers and Tesla authorized repair facilities
have special training, expertise, tools and supplies with respect to Tesla connectors and adapters and, in certain
cases, may employ the only persons, or be the only facilities authorized or certified to work on Tesla connectors and
adapters. Tesla strongly recommends that you have all maintenance, service and repairs done at a Tesla Service
Center or Tesla authorized repair facility in order to avoid voiding, or having coverage excluded under, this Charging
Equipment Limited Warranty.
Wall Connector 3 Install Manual 47

LIMITS OF LIABILITY
Subject to any non-excludable statutory guarantees as set out in the Country Specific Disclosures Appendix below
and to the maximum extent permitted by law, this Charging Equipment Limited Warranty is the only express warranty
made in connection with your Tesla connector or adapter. Implied and express warranties and conditions arising
under applicable local laws, federal statute or otherwise, in law or in equity, if any, including, but not limited to,
implied warranties and conditions of merchantability or merchantable quality, fitness for a particular purpose,
durability, or those arising by a course of dealing or usage of trade, or any warranties against latent or hidden defects,
are disclaimed to the fullest extent allowable by your local law, or limited in duration to the term of this Charging
Equipment Limited Warranty. To the fullest extent allowable by your local law, the performance of necessary repairs
and/or replacement of new, reconditioned, or remanufactured parts by Tesla for the covered defects is the exclusive
remedy under this Charging Equipment Limited Warranty or any implied warranties. To the maximum extent
permissible under your local law, liability is limited to the reasonable price for repair or replacement of the applicable
Tesla connector or adapter, not to exceed the manufacturer’s suggested retail price. Replacement may be made with
parts of like kind and quality, including non-original manufacturer’s parts, or reconditioned or remanufactured parts,
as necessary. This Charging Equipment Limited Warranty covers only parts and factory labor necessary to repair but
does not include any on-site labor costs related to un-installing, reinstalling or removing the repaired or replacement
charging equipment. Parts repaired or replaced, including replacement of a Tesla connector or adapter, under this
Charging Equipment Limited Warranty are covered only until the applicable warranty period of this Charging
Equipment Limited Warranty ends. Under no circumstances will the original warranty period be extended as a result of
your Tesla connector or adapter being repaired or replaced.
Tesla shall not be liable for any defects under this Charging Equipment Limited Warranty that exceed the fair market
value of the applicable Tesla connector or adapter at the time immediately preceding the discovery of the defect. In
addition, the sum of all benefits payable under this Charging Equipment Limited Warranty shall not exceed the price
you paid for the applicable Tesla connector or adapter.
Tesla does not authorize any person or entity to create for it any other obligations or liability in connection with this
Charging Equipment Limited Warranty. Subject to local laws and regulations, the decision of whether to repair or
replace a part or to use a new, reconditioned or remanufactured part will be made by Tesla, in its sole discretion. Tesla
may occasionally offer to pay some or all of the cost of certain repairs that are not covered by this Charging
Equipment Limited Warranty, either for specific models or on an ad hoc, case-by-case basis. Tesla reserves the right
to do the above at any time without incurring any obligation to make a similar payment to other Tesla charging
equipment owners.
To the maximum extent permissible under local law, Tesla hereby disclaims any and all indirect, incidental, special and
consequential damages arising out of, or relating to, the Tesla connector or adapter, including, but not limited to,
transportation to and from a Tesla Authorized Service Center, loss of the Tesla connector or adapter, loss of vehicle
value, loss of time, loss of income, loss of use, loss of personal or commercial property, inconvenience or aggravation,
emotional distress or harm, commercial loss (including but not limited to lost profits or earnings), towing charges, bus
fares, vehicle rental, service call charges, gasoline expenses, lodging expenses, damage to tow vehicle, and
incidental charges such as telephone calls, facsimile transmissions, and mailing expenses.
The above limitations and exclusions shall apply whether your claim is in contract, tort (including negligence and
gross negligence), breach of warranty or condition, misrepresentation (whether negligent or otherwise), or otherwise
at law or in equity, even if Tesla is advised of the possibility of such damages or such damages are reasonably
foreseeable.
Nothing in this Charging Equipment Limited Warranty shall exclude, or in any way limit, Tesla’s liability for death or
personal injury solely and directly caused by Tesla’s negligence, or that of its employees, agents or sub-contractors
(as applicable), fraud or fraudulent misrepresentation, or any other liability to the extent the same is proven in a court
of competent jurisdiction in a final nonappealable judgment and may not be excluded or limited as a matter of local
law.
Wall Connector 3 Install Manual 48

CLAIMING UNDER THE CHARGING EQUIPMENT LIMITED
WARRANTY
Australia
In Australia, the Charging Equipment Limited Warranty is given by Tesla Motors Australia, Pty Ltd.
New Zealand
In New Zealand, the Charging Equipment Limited Warranty is given by Tesla New Zealand ULC.
Claim Procedure
To make a claim under the Charging Equipment Limited Warranty you will need to:
1 . Contact Tesla at the address, email address or telephone numbers listed below for the country in which the
Wall Connector was purchased.
2 . Provide the following information when contacting the Tesla certified installer who sold you your Wall
Connector or Tesla:
a. your name and contact information;
b. proof of the original purchase of your Wall Connector and any subsequent transfer of ownership;
c. a description of the alleged defect(s) or LED error codes listed in the Error Codes chapter of this manual
and any attempts made to resolve the concerns, including any attempted repairs or services not
performed by or on behalf of Tesla.
If you make a claim in accordance with the above claim procedure and a fault with your Wall Connector is covered by
the terms of the Charging Equipment Limited Warranty, Tesla will bear the cost of repairs to or replacement of your
Wall Connector as well as transport and re-installation costs of the Wall Connector and the costs of any at-home or
on-site inspection of the Wall Connector that was required to diagnose the fault. All other expenses of claiming under
the Charging Equipment Limited Warranty will be borne by you. For the avoidance of doubt, the costs of any at-home
or on-site inspection, repairs to and replacement of the Wall Connector will be borne by you if any reported concern
with your Wall Connector is not covered by the Charging Equipment Limited Warranty or if a warrantable fault is
found but you elect to have the fault rectified by a third party that is not approved by Tesla, unless you are entitled to
those costs under applicable laws, including without limitation the Australian Consumer Law and the Consumer
Guarantees Act 1993 (NZ).
If your Wall Connector is replaced under the Charging Equipment Limited Warranty, the remainder of the original
warranty period under that warranty will apply to the replacement product, subject to any non-excludable rights and
remedies you have under local laws in your country or region in respect of the repaired or replacement product.
Contact Details
Tesla Motors Australia, Pty Ltd
Level 14, 15 Blue Street
North Sydney NSW 2060
Phone: 1800 646 952 (Toll Free)
Tesla New Zealand ULC
Wall Connector 3 Install Manual 49

CLAIMING UNDER THE CHARGING EQUIPMENT LIMITED
WARRANTY
501 Karangahape Road
Auckland, 1010
New Zealand
Phone: 0800 005 431 (Toll free)
Wall Connector 3 Install Manual 50

DISPUTE RESOLUTION
Tesla requires that you first provide written notification of any manufacturing defect within a reasonable time, and
within the applicable coverage period specified in this Charging Equipment Limited Warranty, and allow Tesla an
opportunity to make any needed repairs before submitting a dispute to our dispute settlement program (described
below). Please send written notification on dispute resolution to the following address:
Vehicles registered in Austrialia:
Tesla Motors Australia, Pty Ltd
ACN 142 889 816
Level 14, 15 Blue Street
North Sydney NSW 2060, Australia
Phone: 1800 646 952
Please include the following information:
• Tesla Part Number and Serial Number
• Your name and contact information
• Name and location of the Tesla Store and/or Tesla Service Center nearest to you
• Description of the defect
• History of the attempts you have made with Tesla to resolve the concern, or of any repairs or services that were
not performed by Tesla
• In the event any disputes, differences, or controversies arise between you and Tesla related to this Charging
Equipment Limited Warranty, Tesla will explore all possibilities for an amicable settlement
Wall Connector 3 Install Manual 51
