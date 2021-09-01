# xRmold Standard Operating Procedure

Document version: 1.0

App Version: 1.0.0 Build 67.

## 1. PURPOSE

This document describes the standard operating procedure of the xRmold platform. This document is kept in synchronization with the xRmold app.

xRmold comprises a motorized microscope that is wirelessly operated by an iPad, and a software to drive the microscope. It is dedicated to the measurement of mold spores in air samples, following the ASTM standard D7391. The microscope is operated bright field, the images are captured by the iPad and analyzed locally by an embedded artificial intelligence.

Although a training is provided when a unit is deployed in a laboratory, this document should also be read, understood and referred to when questions arise. This document is kept up to date with the app on its internet repository, and a permanent link is provided when installing and running the app the first time.

If an information is requested, particularly if relevant and not found in the document, the user is welcome to contact [support@xrapid-group.com] for any further question.

# 2. CONTEXT

-   These instructions are for the use of researchers, technicians and operators in general who are performing air samples mold diagnostics.
-   This SOP contains general guidelines for the analysis of samples and for sample preparation.
-   This SOP is not a substitute for the standards, the machine and software are used within the frame of standards and/or recommendations but do not replace them.

## 2.1. Main characteristics

xRapid Group has developed a fully automated microscope, patent pending, which consists in a phase contrast microscope (PCM) retrofitted with a set of motors to control the stage movement in three orthogonal directions (x, y and z) with various accuracies. For mold spores analysis, the microscope is operated in bright field mode (the phase contrast ring is removed from the phase condenser). This enables a full sample to be imaged within a few minutes. A series of images are taken by an iPad at increasing depths, from which an autofocus measure is calculated to image the next field. At the same time, a convolutional neural network (CNN) is used for our AI to characterize the objects in the field of view. All the analysis is performed locally on the device, none of the images are uploaded to a server, so that remote work in a poorly connected area is permitted. While we usually refer to AI as Deep Learning, one should notice that xRmold system is not self-learning: all the data has been extracted by humans, and validated by humans. The system shipped is not evolving between updates of the app, which enables to guarantee its performance and pass an eventual certification.

This is best exemplified by a demonstration video, as shown below.

![][image-1]

## 2.2. Equipment specifications

### 2.2.1. General

-   Phase contrast microscope, with phase condenser ring 40×, operated in bright field (phase condenser ring is *not* placed in the phase condenser): the phase contrast mode is used **only** for fiber analysis with our other IH product, xRfiber.
-   Objectives: 40× PCM and 10× bright field objective (4 or 5 spots on the turret).

### 2.2.2. Illumination

-   Kohler illumination
-   LED light source, 3W

### 2.2.3. Power

-   12V-3A power source for 100-240V 0.8A mains, EU-UK-USA-AUS adapters (CE)
-   USB-A plug charge only for iPhone/iPad Pro 10.5’’ (5V, 2A), USB-C plug charge for iPad Pro 11’’ or iPad Air 4 (5V, 3A and 9V, 2A)

### 2.2.4. Eyepiece

-   Two eyepieces, standard 30mm tube diameter.
-   One third eye with a 10× (23mm diameter) eyepiece mounted on collapsible tube, factory centered, on which a cradle support for iPad is attached.

### 2.2.5. Motorized stage

-   X&Y displacement by steps of 125µm and 220µm, respectively
-   Z displacement by steps of 0.5µm or 0.25µm in sequences
-   X course: 75mm
-   Y course: 30mm
-   X&Y error: ±5µm over 18mm (forward and backward displacement of 40 steps)
-   Speed: 15ms/step (X&Y), 9ms/step (Z)
-   Control of coarse and fine displacement by software
-   Stage piloted via Bluetooth or Ethernet through the control app

### 2.2.6. Motorized turret

- Compatible with both 4 and 5-objectives turrets
- Operated automatically to switch between the 40× and 10× objective and back irrespective of the number of objectives on the turret
- Presence and operability automatically detected

### 2.2.7. Control machine

-   iPad Pro 11”, iPad Air 4
-   Additional devices possible, requires additional mounts
-   Power adapter (Apple standard, fitted to region of purchase)
-   Must be connected to the internet at least once a month for authorization

### 2.2.8. Control app

-   Fully automated diagnostic with return to the original point of measure
-   Average diagnostic time per slide lower than 3 minutes (50 fields option) or 8 minutes (150 fields option)
-   Test log (journaling) and QC checks
-   Exports results to PDF and Excel spreadsheets (single or grouped)
-   Artificial intelligence based on convolutional neural networks trained by expert (machine learning), validated on 360’000 fields. This model is fixed in time, it requires a software update to evolve
-   Standards supported: ASTM D7391.

### 2.2.9. Operation details

-   Working capture resolution at 40× is ≈14 pixels per µm
-   Scale and gratings/grids displayed by software, factory calibrated to standard traceable micrometer calibration slides (Ted Pella slides 2280-11, 2280-13, 2280-15)

### 2.2.10. Accessories

-   Telescope for ring position adjustment
-   Leveling tool
-   Dust protection bag and silicon dust cap, lens cleaning paper
-   Set of Allen/Torx wrench
-   Template for slide preparation

## 2.3. Standards

xRmold supports the **ASTM D7391** standard. Do not hesitate to contact us should any other standard be required for operation.

## 2.4. SLIDE PREPARATION
The analysis process was designed for Air-O-Cell and Zefon type slides — spore traps. 

### 2.4.1. Staining
#### 2.4.1.1. Definition
**Lactophenol Cotton Blue (LPCB) Staining** method was used in this work, a standard method to aide the identification of the fungal cell walls:
- Fungi are eukaryotic organisms with both macroscopic and microscopic characteristics
- The fungal spore cell wall is made up of chitin of which the components of the Lactophenol Cotton Blue solution stains for identification.
- The lactophenol cotton blue solution acts as a mounting solution as well as a staining agent.
- The solution is clear and blue in color and it is made up of a combination of three main reagents:
	- Phenol: It acts as a disinfectant by killing any living organisms
	- Lactic acid: To preserve the fungal structures
	- Cotton blue: To stain or give color to the chitin on the fungal cell wall and other fungal structures
- The stain will give the fungi a blue-colored appearance of the fungal spores and structures, such as hyphae.

LPCB can be purchased (skip to the last subsection) or prepared from reagents. 

#### 2.4.1.2. Reagents of Lactophenol Cotton Blue (LPCB) Staining

A preparation of 50ml Lactophenol cotton Blue staining solution is made up of:
- Distilled water 50ml
- Cotton Blue (Aniline Blue) 0.125g
- Phenol Crystals (C6H5O4)  50g
- Glycerol 100ml
- Lactic acid (CH3CHOH COOH) 50ml
- 70% ethanol

Note: Lactophenol Cotton Blue solution is prepared at least 2 days before use.

#### 2.4.1.3. Preparation of Lactophenol Cotton Blue solution

Lactophenol Cotton Blue solution is prepared for over two days leaving the reagents undisturbed to allow dissolving and maturation.

Day 1: Dissolve the cotton blue in distilled water and leave to rest overnight. This eliminates insoluble dye.

Day2: Using protective gloves, add phenol crystals to lactic acid in a glass beaker and stir using a magnetic stirrer until the crystals dissolve. Add glycerol. Filter the Cotton blue and the distilled water into the phenol + glycerol +lactic acid solution and mix.

#### 2.4.1.4. Procedure of Lactophenol Cotton Blue (LPCB) Staining

This is the procedure that was used to mount cultures from Pétri dishes:
- On a clean microscopic glass slide, add a drop of 70% ethanol
- Add the fungal specimen to the drop of alcohol using a sterile mounter such as an inoculation loop (from solid medium), depending on the sample of use.
- Tease the fungal sample of the alcohol using a needle mounter, to ensure the sample mixes well with the alcohol.
- Using a dropper or pipette, add one or two drops of Lactophenol Cotton Blue Solution (prepared above) before the ethanol dries off.
- Carefully cover the stain with a clean sterile coverslip without making air bubbles to the stain.
- Examine the stain microscopically at 40×, to observe for fungal spores and other fungal structures.
- If the slide is acceptable, capture 150 fields using xRmold, less than 15 minutes after the slide has been mounted.

The procedure used to mount samples from air cassettes is as follows:
- Open the cassette with a scalpel
- Remove the slide sample with gel from the cassette — notice the trace in the middle appears matte on the shiny background of the gel
- Eventually mark the beginning of the trace with a second (sterile) scalpel
- Apply a small droplet of lactophenol cotton blue on the slide
- Hold the sample slides gel facing the microscope slide, from one side, and let it fall in place gently, taking care of not creating air bubbles
- Apply a light pressure on the slide to squeeze out completely the lactohenol cotton blue.
The spread of LPCB will vary depending on the quantity applied and quality of the adhesive.

A summary quick-sheet can be downloaded at this link.

#### 2.4.1.5. Limitations

- It can only be used as a presumptive identification method of fungi which should be followed up with other diagnostic tools such as biochemical and cultural examination.
- The components of the solution should be used before expiry, including the use of the solution before it expires.
- The solution may disrupt the original morphology of the fungi.
- The stain can only be used to identify mature fungi and its structures and not the young vegetative forms of fungi.
- The stain can not be stored for a long period of time.

**Important: we have noticed that the stain diffuses through the spores slowly, which confuses the AI after some time. To obtain the best results, the slides should be processed through xRmold no more than 15 minutes after being mounted in LPCB.**

#### 2.4.1.6. Where to get LPCB

- Lactophenol Cotton Blue, Fungal Stain, 15ml, by [Hardy Diagnostics][1]
- Lactophenol blue solution [Merck/Sigma Aldrich][2]

### 2.4.2. Mount

xRmold is set to analyze samples that have been laid out **horizontally** only. The microscope will scan 150 fields horizontally to capture a full trace of 10mmx1mm. The next Figure shows the correct geometry for the mount.

![][image-2]

**Note**: for the sake of simplicity, it is not envisaged to enable a vertical mount at the moment. Do not hesitate to contact us if this is standard practice in your laboratory. 

# 3. SAFETY NOTES

-   Always carry the microscope with two hands, wear protective clothing and shoes when moving equipment. It is advisable to place one hand under the base of the box for extra support.
-   When opening the box, make sure that the top is facing upwards.
-   If the microscope is stored in a box, always ensure the door is locked before picking up the box.
-   Never disassemble the microscope on your own without xRapid-Group instructions and guidance as doing so may damage it and null the warranty.
-   Turn off and unplug from the power supply before moving the microscope.
-   Secure the turret of the microscope before and when moving the microscope.
-   Never use coarse focus on your microscope — this knob is locked. Only the fine focus is available. The coarse focus knob is blocked, and using it will damage the z-movement of the microscope.
-   Make sure your workstation is set up ergonomically to use the microscope.
-   Make sure the microscope is not stored in direct sunlight, nor stored in rooms where large temperature variations are expected. Normal temperature usage is within 15 to 25 degrees Celsius.
-   Make sure the microscope is regularly electrically tested and tagged. Only use the provided electric cable and adapter. Choose a stable power source.
-   Wear protective clothing, gloves and goggles preferably when preparing the slides, and operating the microscope. It is better to prepare the samples in a laminar flow cabinet.
-   Never touch the lenses of the microscope with naked fingers: objectives, eyepieces and eyepiece on the trinocular.
-   Only use special lens paper to clean the optics.
-   Never touch an electric outlet with wet hands.
-   Do not open the back of the microscope without being grounded, as this may result in electric shocks/hazards.
-  Contact [support@xrapid-group.com][3] in case there is any doubt.

# 4. PREREQUISITES

The following items are required for the operation of xRMold platform.

-   A cleared and clean laboratory space, if possible with constant lighting and in a low vibration environment
-   A free power outlet
-   At least one dedicated technician
-   An internet connection, active during the installation and at least once a month on the first day of the month
-   An Apple mobile device: iPad Pro 11” (2019) and iPad Air 4 are all compatible with the hardware
-   An iCloud account and AppleID (free iCloud account is good enough)
-   Depending on the standard of the laboratory, some QC slides
-   Optionally a networked printer.

# 5. RESPONSIBILITIES

It is the responsibility of the user to ensure that:

-   The microscope unit is functioning properly, and report to [support@xrapid-group.com][4] in case there is any doubt that it does
-   The power supply is connected to a stable source of 110V or 220V, depending on the local environment
-   The microscope unit it set in a proper environment, that the optics are covered and dust protected when the unit is not in use (see section 6.1)
-   A field blank is used regularly to check that the count is adequate, i.e. it yields zero spores counted. Alternatively, check that there are no fixed elements in the field images, which would indicate dirty optics
-   An adequate number of slides are checked for quality control of the software (see section 6.5)
-   The user name on the main screen of the software, when operating the unit, is correct, for traceability purposes (see section 6.4)
-   A copy of the standard in use locally is located close to the equipment for reference.

Additionally, the best results are obtained when:

-   The slides are well prepared: see above.
-   The initial focus is on the surface of the filter.

# 6. PROCEDURE

## 6.1. Hardware

### 6.1.1. Components

The xRfiber/xRmold microscope components are shown in Figure 6.1.

1. Power Switch
2. Power Adapter Port
3. USB Charging Port
4. Fine Focus Adjustment Knob
5. LED Light Source with Field Iris Diaphragm
6. Condenser
7. Condenser Adjustment Knob
8. Phase Ring Holder
9. Condenser Iris Diaphragm
10. Microscope Stage
11. Stage Clip
12. X-Axis End Stops with Cover
13. 40x Plan PH2 Objective
14. Objective Turret
15. Oculars
16. Condenser Alignment Screws
17. Cradle Support Arm
18. Adjustable C-Mount Adapter
19. iPhone/iPad Cradle
20. Ocular Locking Screws

![][image-3]

Figure 6.1. xRfiber Microscope components

Additional components in the box are shown in Figure 6.2.

![][image-4]

Figure 6.2. Additional components in the box

---- 
21. Protection Bag
22. Lens Cleaning Tissue
23. Slide Preparation
24. Level
25. Plug Adapter
26. Power Supply
27. Telescopic Eyepiece
28. Eyepiece Cap
29. Eyepiece Screws
30. Eyepiece WF10X
31. Allen Wrench (Alignment)
32. Allen Wrench H2.5
33. Allen Wrench H1.5
34. Torx T10  

Finally, for xRmold, an optional motorized turret is present on the microscope (recommended), and a 10X microscope objective is provided.

### 6.1.2. Installation

1.  OPENING THE BOX

Upon opening your xRfiber unit, please use the checklist provided to confirm all items have been received: the checklist is on the top of the box when opening it. If something is missing, please contact [support@xrapid-group.com][5].

![][image-5]

Figure 6.3. box contents

2.  GETTING THE MICROSCOPE OUT OF THE BOX

When deciding where to place the xRfiber Platform, consider the following:

- The platform should be placed on a stable, level surface
- The platform should be placed conveniently as to minimize the need to move after initial setup
- The area/room the platform is placed in should have consistent, even lighting as to prevent errors due to fluctuations in ambient lighting
- Once a location has been selected, take the microscope out of the box and place it in the selected area
- Remove the plastic wrapping from the microscope.

Verify that the head of the microscope (A) is aligned with the body (B). If not, slide the head into alignment with the body by hand: apply a slight rotation of the head to align its edges with those of the body.

![][image-6]![][image-7]

Figure 6.4. Alignment of the microscope head

Verify that the adjustable C-Mount Adapter (n°18) is aligned with the head of the microscope. If not, use a Allen wrench H3 (not included) and adjust the adapter after loosening the screw.

Remove both Ocular Covers (n°35). Eventually use a air duster (not included) in the ocular openings to ensure that they are free of debris and dust.

![][image-8] ![][image-9]

Figure 6.5. Installation of the eyepieces

3.  INSTALLING THE OCULAR (N°15)

If the ocular is not clean, use an air duster (not included), and/or the Lens Cleaning Paper (n°22) to clean it before insertion (no circular motion — always have a linear motion so that the dirt stays on the edges of the lens and does not spread over the lens).

If you cannot insert it, loosen the ocular locking screw(s) (n°20) with the Allen Wrench H1.5 (n°33) and try again.

4.  SECURING THE OCULAR (N°15)

Slowly tighten the screw with the Allen Wrench H1.5 (n°33) to secure the eyepiece.

5.  INSERTING THE TELESCOPIC EYEPIECE (N°28) FOR PHASE RING ALIGNMENT

If you cannot insert the telescopic eyepiece, loosen the eyepiece locking screw (n°20) with the Allen Wrench H1.5 (n°33) and try again.

Insert the Telescopic Eyepiece (n°27).

Slowly tighten the screw with the Allen Wrench H1.5 (n°33) to secure the Telescopic Eyepiece (n°27).

6.  INSTALLING THE OBJECTIVE (N°13)

Rotate the turret so the available opening is askew from the optic train.

Carefully align and slowly tighten the 40X Plan PH2 Objective (n°13) in the available turret orifice.

**WARNING**: The objective is very fragile, please take care when handling

Turn the turret to align the objective (n°13) with optic train.

**WARNING**: Take care that the stage (n°10) is low enough in order to avoid collision with the 40X objective (n°13). If it is not the case, get the stage down using the Fine Focus Adjustment Knob (n°4).

7.  INITIAL CALIBRATION

#### Centering the condenser

-   With no sample on the stage, slowly close the field iris by turning the dial around it clockwise.
-   As the edges of the iris come into the field of view, adjust the center of the condenser using the Condenser Alignment Screws (n°16) located on the front left and front right sides of the condenser.
-   When complete, the hexagon of the field iris should appear in the center of your field of view.
-   Begin turning the dial on the field iris counter- clockwise until the edges of hexagon are just outside the field of view.

#### Phase ring
xRmold operates in standard transmitted light microscopy (upright microscope), which is not the case of xRfiber. If you are using the xRmicroscope for both xRfiber and xRmold, you **must remove the phase ring from the condenser before operating xRmold**.

xRmold uses the same Olympus x40 objective for mold diagnostic as xRfiber: this phase contrast objective is also perfect for transmitted light microscopy.

#### Koehler illumination

While there is a certain leeway ni operating xRfiber with a quite-not-perfect illumination of the microscope (note: not for chysotile samples!), this is not the case for xRmold, where the condenser must be perfectly aligned and spaced vertically with the slide.

We recommend that the user familiarizes with Koehler illumination by using the excellent app “Koehler Tutor”, which can be downloaded from the App Store at this [link][6] if it is not installed on your iPad already.


6.  INSTALLING THE CRADLE (N°19)

Use the T10 screwdriver (n°34) to remove the 3 screws (n°29) from the eyepiece tube of the cradle.

Insert the Eyepiece WF10X (n°30) into the Cradle (n°19).

-   If the eyepiece is not clean, use an air duster (not included), and the Lens Cleaning Tissue (n°22) to clean it before insertion (no circular motion).

Replace the screws you had previously removed, making sure they do not run into the sides of the eyepiece.

-   Insert the screw approx. 1mm past the inner wall so that they keep the eyepiece in place but can also still be adjusted after attaching to the adapter.

Remove the two screws (n°37) located on the top of the back of the microscope.

Remove the C-Mount Adapter Cap and align the Cradle with the tube of the adapter sliding them together. (Note: the screw holes on the bottom of the Cradle Support Arm should line up with the holes you just opened in the previous step)

Attach the Cradle to the microscope using the two screws (n°36) you removed.

![][image-10] ![][image-11] ![][image-12] ![][image-13]

Figure 6.7. Installation of the iPhone cradle

7.  ALIGNING THE CRADLE (N°19)

-   Unlock your device (iPhone/iPad) and open the “Measure” application (this comes installed on all iOS devices normally, if it is not installed search for it in the Apple App Store)
-   Place the device across the stage of the microscope, taking care that it lays flat on the stage
-   If the stage is not perfectly level, you can try moving the microscope or rotating it on the table to find the most level position in the selected area
-   If you cannot get a zero (0) value after adjustments, take note of the level of the stage (degree and direction)
-   Remove the device and place it in the cradle
-   Loosen the locking knob on the adjustable C-mount adapter
-   Slide the C-Mount Adapter up into the eyepiece tube of the cradle
-   Make sure the adapter tube is fully inserted into the eyepiece tube completely past the screws in the eyepiece tube
-   While holding the tube and cradle together, adjust the height of the adapter until you get an optimal level in that y-axis direction
-   Tighten the locking knob on the adapter securely
-   Once the adapter is locked, start tightening the screws on the cradle tube to secure it to the adapter
-   Once secure, small adjustments can be made to the alignment through tightening/loosening these screws
-   If your stage was not perfectly level, adjust the cradle positioning so that the cradle orientation best matches the direction and twist/yoke angles of the stage level measured in the first place.

The ideal situation is shown below: the device both on stage and in cradle should show the same orientation, leveled at zero degrees in all directions.

![][image-14]

Figure 6.7. unbalanced (left) and perfectly flat orientations of the iPhone in its cradle and on stage

## 6.2. Device (iPhone/iPad) setup

### 6.2.1. Generic setup

After going through Apple’s initialization guide, ensure the following:

-   The device is logged into an iCloud account (this is required for location services to be active which is required for device use records).
-   The device is connected to the internet (this is required to upload usage records for billing purposes).

Open the Apple App Store and select the Search tab in the bottom right of the screen. Search for “xRmold” and the application should appear in the results list. Press the Install option and confirm the installation with your password/thumbprint. Once the application is installed, turn on the microscope and then open the application once the LED light source has finished blinking three times (approx. 3-5 seconds from powering on).

**NOTE**: when the microscope is switched on, the light first blinks three times. It is an indicator that the Bluetooth has been initialized and the microscope is now ready to interact with the Software (the xRmold app).

The app is released via Diawi during the alpha/beta testing periods, it is made available on the App Store afterwards. The user gets notified by email that a new version is available, with the release notes of the update. The user also gets in his email and the iPad’s email the link to download the app.
Once the link is tapped on the iPad or entered manually into Safari (the iPad’s web browser), a window offering to install the app is accessed.

**Important when updating from Diawi**: in order to be able to install the app, one needs to tap the “aA” button in the Safari top bar, and pick “Request mobile website” from the pop-up box. Then one can hit the “Install this app” button in the middle of the page. A message box will come up asking for confirmation of installation.

**App Store update**: we recommend that the iPad is setup to auto-update the apps installed. This is performed nightly when the iPad is connected to the internet.

### 6.2.2. Setting up the Ethernet connection
When the microscope is to be operated through a wired connection, one follows the connection scheme described in 6.1.3. Irrespective of the connector that was provided in the package (availability of this connectors vary), the procedure will be the same:
- in the iPad Settings, spot the “Ethernet” option when the USB-C adapter connects to the iPad
- A blue “cable connection” icon will appear in the top bar and stay for about 5 seconds, then disappear
- In the “Ethernet” thumb, under “Interfaces” the connector will appear
- Getting into this connector settings will reveal options for “IPV4 ADDRESS”, “DNS” and “HTTP PROXY”
- The correct settings are:
	- IPV4 ADDRESS
		- Configure IP: Manual
		- IP address: 169.254.65.10
		- Subnet mask: 255.255.0.0
		- Router: 169.254.65.6
	- DNS
		- Configure DNS: Manual
	- HTTP PROXY
		- Configure Proxy: Off
From that point onwards, when the Ethernet cable is connected to the iPad, the microscope will establish a network connection first.

![][image-15]

Video 6.1. setting up the Ethernet connection in iPad’s settings

## 6.3. Operating the software

The xRmold app has many features to facilitate not only the diagnostic, but also the review of results. We will now examine the various screens and functionalities of the app.

### 6.3.1. Main screen

#### 6.3.1.1. Establishing a connection

When starting the app, the central button START MEASURE (5) is grayed out. After a few seconds, the app completes the connection to the microscope and is now ready to measure:

-   the Bluetooth logo or its alternative Ethernet logo (1) is circled
-   the large hexagonal START MEASURE (5) button turns white and animates to a pulsation.

Notice that the Bluetooth logo (1) is more than just an icon: it is also a button that can be tapped again should the Bluetooth connection drop. It generally takes about 2-3 seconds to establish this connection.

**NOTE**: the Bluetooth standard comes with a few drawbacks. One of those is the failure to resume a connection when a service has been lost for a duration of 30 seconds.

Once a device is connected, the button (1) being circled, tapping the Bluetooth button again will show a pop up with the name of the device selected. In laboratory settings where more than one microscope can be connected via Bluetooth, this is used to change the iPhone/iPad assignment to another microscope.

**NOTE**: the Bluetooth functionality lets us discover the device based on the strength of the signal. If two devices are more than one meter apart, the iPhone/iPad will find the correct microscope, i.e. the microscope it is sitting on. If devices are closer, some mixing or confusion of signals may occur, and the device will have to be checked and connected manually using the pop up menu.

![][image-16]

Figure 6.9. Main screen in the disconnected state (left), Bluetooth connected state (middle) and Ethernet connected state (right) 

#### 6.3.1.2. Elements

##### Operator

It is good practice, and **requested by most standards**, to have the operator (3) identified during testing. xRmold offers the capability to have more than one operator registered on a device. When multiple operators are registered, the right and left arrows (2) are visible and circled, indicating that they can be tapped to select the next or previous operator in the list. When only a single operator is listed, the arrows do not appear. Alternatively, one can swipe left and right on the name of the operator and this will present the previous/next operator in the list.

Entering or changing an operator is done through the Settings option of the app.

##### Settings button

The Settings button (4) is always active, it leads to the parameters and options of the app. Will be used to set the standard, the operator(s) and optionally a printer.

##### Statistics line

The number of tests run this month (6) and today (7) are displayed on this line. These numbers are dynamic, they reset at the end of the day and the beginning of the month.

The last three tests are displayed in boxes (9) under the statistics, and can be used to navigate quickly to the detailed results of the test.

##### Tests log

The Tests Log button (8) props up the log of all the tests ever carried out on the device. Because the microscope does not keep in memory the record of the tests performed, but rather just the global count, the tests log may be different if two devices are used to drive the same microscope.

##### Light button

The light button (10) is used to switch on/off the microscope light source. When the microscope is connected the state of the microscope is highlighted under the button.

### 6.3.2. Settings screen

#### 6.3.2.1. Overview

The settings/options have 4 main categories, reached by tapping on the segmented control: Practitioner (1), Print (2), Parameters (3), Institution (4). Parameters are related to the motorized turret, and only accessible when the microscope is connected to the iPad via an Ethernet cable.

![][image-17]

Figure 6.10. Settings screens with the Practitioner (left), Print (center left),  Parameters (center right) and Institution (right) settings.

Notice at the bottom (8) the version and Build number between parentheses — communicate those to xRapid when requesting support.

All changes need to be validated, by hitting the Save button at the bottom right of the screen. Cancelling restores the last saved options.

#### 6.3.2.2. Practitioner

All the users informations are private, and not exchanged with xRapid-Group: they are mainly used for app-generated reports, and QC/QA purposes. The printed, PDF or CSV reports will have all the information the user has entered in this section.

**NOTE**: For QC purposes it is impossible to change the name of the operator of a test once the test has started.

One must have at least one operator per device. Fill in contact details accordingly, and hit the Save button at the bottom right.

Tap the button (5) Add New Practitioner to have multiple operators on a single device: it will clear out the name field, and you will be free to Save this additional operator. There is no limit to the number of operators that one device can hold. On the other hand, there is a limit on the number of addresses (only one) an institution can have.

One can switch the user from the Main screen, or using the small arrows on the left and right of the name.

**NOTE**: it is good practice to change the operator of the software whenever the physical operator of the xRfiber microscope changes. At the same time, all the QC checks should be passed before a new run of slides is carried out.

#### 6.3.2.3. Print

The easiest way to generate reports is to print them directly from the app. xRfiber has the capability to print to any wireless networked printer in a variety of formats. Tapping the printer or Add printer button will take you to the iOS print menu — this is a system feature.

xRfiber can print reports in color or monochrome, on A4 and US Letter paper. Should your printer handle double-sided prints, xRfiber will comply.

While most users want to export their results to a CSV (Comma Separated Values) file compatible with Excel or Numbers, it is useful for quality purposes to keep a daily log of the machine, and print it out at the end of the day. xRfiber facilitates this operation by letting the user select all the records of the day in the Tests Log to export or print them out.

#### 6.3.2.3. Parameters

Parameters are only related to the microscope. They enable the reading of the firmware version — the current firmware running on the microscope card. 

The second parameters, named the `Steps Focus Difference` is provided to you or initialized when purchasing a microscope. Because not all microscope turrets and/or objectives are created equal, there is generally a difference between the focus positions of the 40x and 10x objectives. When performing a trace finding, xRmold automatically adjusts between the focus positions of 40× and 10×, to find the best focus on the trace. 

The third parameter is presented as a visual. Microscope turrets ship with 4 or 5 holes for objectives. The number of holes is determined automatically. In the rare case the wrong number is detected, usually due to an error in mounting the objectives, tapping this button enables to change the number of holes.

The next parameter is a switch that enables to have either a combined trace and focus finding, either have them separate. These two modes are detailed in section 6.3.3.

The final parameter is also a switch, to use Contextual analysis. The purpose of the contextual analysis is to reduce the number of unknown spores. When the AI is certain beyond a threshold established experimentally that certain species are present, it uses this information in contextual analysis to lower the acceptance threshold of similar spores. The contextual analysis is on by default, raw data can always be recovered in any case.

#### 6.3.2.5. Institution

This last setting is where the institution logs in and eventually changes its coordinates. Those are used to produce customized reports with the name, address and logo of the institution. The username and password are fixed, and provided to the user by xRapid during installation. To login or logout, one needs to swipe down to access the button.

**Important**: one needs to be connected to the internet for this process to work.

**Note**: one should only need to login once. Do not hesitate to contact us should some details be missing or incorrect.

### 6.3.3. Measurement screen

Once the device is properly setup, one can proceed to performing diagnostics. The Measurement screen is obtained when the hexagonal Start Measurement button is tapped on the Main screen.

When entering the Measurement screen, the microscope light source will turn on automatically. If it does not, the microscope is not properly connected to the iPad via Bluetooth or Ethernet, and the connection should be re-established. Notice that failure to establish connection with the microscope stops the user from entering in the Measurement screen.

#### 6.3.3.1. Test identifier

A default identifier (1) is automatically generated. It is grayed-out, and can be changed. Tapping this identifier will show the iOS keyboard (2), tapping the small X icon at the right of the field will dismiss all changes and the keyboard. Any identifier longer than one character can be entered. 

The case presented in Figure 6.11. enables the use of sequences: any string followed by a dash - and a number will be automatically followed by the the same string with the number incremented by one when the next test is launched. This is particularly useful when a file contains several samples with a resulting large number of slides. Notice that the next time the analysis is launched, the test identification will now default to the next increment, if a dash was present in the first test diagnostic. It is possible to start a sequence at any number following the dash: this can be useful when a job is split in more than one series.

![][image-18]

Figure 6.11. Starting a diagnostic with changing the default test identification

#### 6.3.3.2. Stage movement control

The usual sequence is shown Figure 6.12: tap the Start Diagnostic hexagonal button (1), after which the diagnostic sequence executes automatically.

One can adjust the position of the slide by tapping the Controls icon (2), which will bring up the in-plane control (3) and focus control (4). One can return to the start button by hitting the cross (5).

![][image-19]

Figure 6.12. Illustration of entering a Diagnostic screen (right), start position being set up (middle), and diagnostic running (right)

#### 6.3.3.3. Trace and focus finding

Because finding the trace can be challenging, xRmold has been designed to find the trace automatically, provided there is one: this procedure will likely fail on some clearance samples. The microscope features a second objective (10× Olympus objective) and a motorized turret that rotates between 40× and 10× objectives. Two options are available in the `Settings` of xRmold, under `Parameters`: if `Combine Trace and Focus` is switched on, a single button will appear: `Do Trace`. Otherwise two buttons will be available, `Find Trace` and `Focus`. With a single button configuration, the microscope will:
- rotate to the 10× objective
- proceed in finding the trace
- position the slide at the beginning of the trace
- rotate back to 40× objective
- focus.
The preferred operation, however, is to use two buttons. One can then find the trace and adjust the start position using the 10× objective and the fine movement controls as a first step. When the position is correct, one hits the `Find Focus` button which rotates the turret back to the 40× objective.

#### 6.3.3.4. Measurement path

xRmold enables two measurement paths, which are either linear (50 steps in linear sequence) or not (150 steps in a serpentine path). From experience, well-prepared Air-O-Cell slides are performing well with 50 steps, while Zefon slides require 150 steps: this is due to the dimensions and characteristics of the impacter.

The diagnostic will stop when the complete number of steps (50 or 150) has been reached. The analysis can be stopped at any time by means of the `Stop` button (8). Confirmation is required when the `Stop` button is tapped.


#### 6.3.3.5. Performing an analysis

The method is analogous to that used by a human analyst:
- position the microscope slide either manually or using the screen controls at the beginning of the trace: is is useful to rotate the turret out of position and adjust the position of the slide to the light spot of the condenser
- Adjust the focus manually
- Hit the start button.
The slide will then be scanned though 150 steps or 50 steps, depending on the option chosen. The slide is scanned through the thickness, and one will see the objects/spores blur in and out. A step is considered out-of-focus when the objects/spores do not get though a position of focus during the through thickness scan. The slide scanning process includes an auto-focus adjustment from step to step.

#### 6.3.3.6. Results

Results are presented according to the **ASTM D7391**. You will find the raw counts, the spores per volume if the volume was indicated, as well as the total percentage in the table. We also indicate the percentage of coverage of the trace.

The results can be exported as an image or a PDF, or to Excel as a comma separated value file (CSV option).

### 6.3.4. Results screen

The results screen presents all the spores identified by count, counts per volume if the volume was entered, and percentage. The table can be scrolled. Button `1` opens a Photos screen, while button `2`  enables to print and/or share the results. Tapping the button `2` opens a dialog `6` while tapping the button again `5` or anywhere on screen not in the dialing enables to close it again. `Sharing as a PDF` is illustrated here. `Sharing as a CSV file` opens a similar dialog to save the file in location, or open it in your spreadsheet editor of choice.

Text fields `3` and `4` are not editable.

This view can be dismissed to go back to the Tests Log by tapping button `8`.

![][image-20]

Figure 6.13. Results screen

**Note**: the spreadsheet editors on iPadOS are **Numbers** (Apple Inc., free) and **Excel** (Microsoft, free viewer and subscription required to edit).

### 6.3.5. Photos screens

Tapping button `1` on the previous Results screen opens the Photos screen, as shown below. The control at the bottom right lets one quickly review the results, by selecting only the positive or the negative fields. An additional picked is obtained by long pressing on the Positives index again after selecting it (a long press is about 2 seconds). A pop up with the species detected on this sample will show, one can tick/un-tick the species and the photos will update accordingly. Finally, tapping on an image brings up said image, where boxes delimit the spores identified in this field. Moving to next or previous field is achieved by swapping on the image right or left, respectively.

![][image-21]

Figure 6.14. Photos screens

Photos can be multiple selected for printing, exporting and the like: tap the select button at the bottom left of the screen, select the images by ticking/un-ticking them and hit the share button. Notice there is a limit due to iPadOS of about 50 images when exporting.

![][image-22]

Figure 6.15. Selecting photos for sharing/export

### 6.3.4. Tests log screen

The tests log screen is accessed from the main screen — the large button at the bottom. It keeps a log of all the tests performed on this iPad in reverse chronological order. Tapping any line brings up the Results of this test. Diagnostics are presented with the number of spores detected in italics, together with the number of fields.

Exporting or printing multiple test results at once is straightforward: tap the select button and tick/un-tick the desired tests. One easy way to eg print all tests from the same day is to tick the day, as shown in the Figure below.

![][image-23]

Figure 6.16. Test log, selecting and printing or archiving results by date

### 6.3.5. Image formats and Device space

Images are kept uncompressed depending on the space on the device. When the device space becomes low, images will begin to be compressed. This should not be apparent to the user. Images preferably uncompressed should be used when communicating with xRapid, as they can be re-run on our models. Compressing images takes them from about 3Mb to 300kb per image.

Should the iPad run low on space, do not hesitate to contact xRapid support.

## 6.4. ARTIFICIAL INTELLIGENCE

### 6.4.1. Basics

The app xRmold uses a heavily customized version of an object detector, which has two functionalities:
- detect the position of the objects the AI has been trained to recognize
- Classify those objects, i.e. attribute them a label and a confidence.

### 6.4.2. Confidence

The confidence is an agnostic measurement of probability that the AI calculates, it goes from 0 to 100%. In essence, we chose to limit the mold spores found to certain thresholds of confidence, in order to limit the number of false positives and false negatives. To do so, we did accept a certain level of “Unidentified Spores”, which you will see in the report. Those represent the entities that the AI identified, perhaps rightly, that the classifier could not sort with an acceptable confidence.

In practice, we have experienced great difficulties between some classes, and they mostly come from spores that are somewhat damaged: a squished stachybotrys can ressemble a chaetomium, and a folded chaetomium can ressemble a stachybotrys, for example.

### 6.4.3. Reviewing the results

Tapping on the images icon from the main results view will bring up a collection view of all the fields captured. One can select the fields from the classes they include by long-pressing the classes selector at the bottom right. Selecting and de-selecting classes updates the underlying images. This is particularly useful to find some interesting fields.

The images show classes and their confidence when this option is selected.

### 6.4.4. Species and legend

The following spores are identifiable in the current version:
- ULOBO: Ulocladium botrytis
- CLA: cladosporium cladosporoides and cladosporium sphaerospermum
- STACH: stachybotrys chartarum
- CHAGL: chaetomium globosum 
- EPICO: epicoccum
- ALT: alternaria alternata and alternaria solani
- ASP: aspergillus versicolor, aspergillus ochraceus, aspergillus Niger, aspergillus candidus, aspergillus tamarii , aspergillus fumigatus 
- PEN: penicillium brevicompactum, penicillium chrysogenum, penicillium sp1
- SCOBR: scopurialopsis brevicompactum
- FUSSO: fusarium solani

### 6.4.5. How the AI is trained

Each specie is cultured and sampled at 3-5, 7-10 and 15 days on at least 3 slides. At least 150 fields are captured on each slide. Each field containing spores is manually annotated, where each spore is identified by position and class. The AI is trained on all the fields and the selected classes at once — about 30’000 samples. A full training takes about 3 days. Transfer learning, when adding for example 1-2 classes to the dataset, takes about half a day if all goes well.

The AI is tested and validated on independent sets from training, created using different slides from the same cultures.

**Note**: it is always useful to have an independent validation set from field slides, we will welcome images without annotations but description to this effect.

**Note**: it is be shown in the app utilization section (6.3) how to change the labels of a spore. When this is performed, the image is sent back to our servers, and may be used in our training set after the change has been confirmed by our analysts.

## 6.5. Standard care and cleaning of the unit

### 6.5.1. Standard care

For optimal results, xRmold must be used in a microscopy environment, that means:

-   Air regulated area to avoid dust.
-   No vibration. The xRfiber platform must be installed in a stable and robust stage, uncoupled from floor vibrations.

Additionally, the microscope must be covered by its plastic pouch when not in use, to avoid the deposition of dust. Furthermore, the silicon tip must be inserted in the hole of the eyepiece of the trinocular tube when the iPhone/iPad is not on its cradle.

### 6.5.2. Cleaning the microscope

**WARNING**: Do not use detergents or aggressive liquids to clean the xRmold microscope or its optics. A compressed air spray (not included) and the lens cleaning paper (included) are sufficient to perfectly clean the xRfiber platform.

Process for cleaning the xRfiber platform

1.  Remove the cradle
	1.  Begin by the socket head screws that they maintain the cradle support in the microscope head.
	2.  Remove the cradle with the eyepiece.
	3.  Loosen the three screws which maintain the eyepiece on the cradle cylinder and remove the eyepiece.
	4.  Clean the eyepiece using a dust air spray, clean it on its top and on its bottom.
	5.  If some impurities remain on the lens, use a lens cleaning paper (always with linear motion), and use the compressed air spray when finished.
2.  Remove the trinocular tube by loosening manually the two screws maintaining it
3.  Use the compressed air spray to clean the glass on the top of the head.
4.  Remove the head of the microscope using a 2.5mm Allen wrench
	1.  Remove the Olympus objective from the turret.
	2.  Turn the turret to place the opened orifice in line with the optic train. From the top of the microscope, use the compressed air spray to clean the microscope and the turret.
5.  Reassemble the head of the microscope.
6.  Reassemble the trinocular tube.
7.  Place the eyepiece in the cradle cylinder and slowly fasten the 3 screws to maintain it.
8.  Reassemble the complete cradle and maintain it fastening both screws on the microscope head.
9.  Use the compressed air spray to clean the objective and reassemble it on the turret.
10. Use the compressed air to remove dust on:
	1. The lenses on the top of the condenser.
	2. The glass on the top of the light diaphragm.

If both the front oculars are in use, to clean them:
-   Remove both oculars using a 1.5mm Allen wrench.
-   Use the compressed air spray to clean inside the microscope head oculars orifices.
-   Use the compressed air spray to clean both oculars on their top and on their bottom. If some impurities are still existing, use the lens cleaning paper to remove them (every time with linear motion), and use the air compressed spray to finalize the oculars cleaning.

The xRmold microscope is now normally clean to proceed with the analysis. Do not forget to clean your Apple device camera lens using the lens cleaning paper.


[1]:	https://www.amazon.com/Lactophenol-Cotton-Fungal-Hardy-Diagnostics/dp/B0732CDHHT
[2]:	https://www.sigmaaldrich.com/catalog/product/sial/61335?lang=fr&region=FR
[3]:	mailto:%20support@xrapid-group.com
[4]:	mailto:%20support@xrapid-group.com
[5]:	mailto:support@xrapid-group.com
[6]:	https://apps.apple.com/fr/app/koehler-tutor/id1281328178?l=en

[image-1]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_DEMO_FINAL.m4v
[image-2]:	https://xrapid-group.github.io/xrmold/Pictures/XRmold_Sample_Geometry.png
[image-3]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_1.png
[image-4]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_2.png
[image-5]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_3.png
[image-6]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_4_a.png
[image-7]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_4_b.png
[image-8]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_5_a.png
[image-9]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_5_b.png
[image-10]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_7_a.png
[image-11]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_7_b.png
[image-12]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_7_c.png
[image-13]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_7_d.png
[image-14]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_8.png
[image-15]:	https://xrapid-group.github.io/xrfiber/Pictures/Ethernet_connection.mp4
[image-16]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_SOP_6_9.png
[image-17]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_SOP_6_10.png
[image-18]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_SOP_6_11.png
[image-19]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_SOP_6_12.png
[image-20]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_SOP_6_13.png
[image-21]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_SOP_6_14.png
[image-22]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_SOP_6_15.png
[image-23]:	https://xrapid-group.github.io/xrmold//Pictures/xRmold_SOP_6_16.png
[image-24]:	https://xrapid-group.github.io/xrmold//Pictures/QUICK_GUIDE_L-US-3.pdf