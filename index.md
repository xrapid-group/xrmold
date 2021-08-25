# xRmold Standard Operating Procedure

Document version: 1.0

App Version: 1.0 Build xxx

## 1. PURPOSE

This document describes the standard operating procedure of the xRmold platform.

xRmold comprises a motorized microscope that is wirelessly operated by an iPad, and a software to drive the microscope. It is dedicated to the measurement of mold spores in air samples, following the ASTM standard D7391. The microscope is operated bright field, the images are captured by the iPad and analyzed locally by an embedded artificial intelligence.

Although a training is provided when a unit is deployed in a laboratory, this document should also be read, understood and referred to when questions arise. This document is kept up to date with the app on its internet repository, and a permanent link is provided when installing and running the app the first time.

If an information is requested, particularly if relevant and not found in the document, the user is welcome to contact [support@xrapid-group.com] for any further question.

# 2. CONTEXT

-   These instructions are for the use of researchers, technicians and operators in general who are performing air samples mold diagnostics.
-   This SOP contains general guidelines for the analysis of samples and for sample preparation.
-   This SOP is not a substitute for the standards, the machine and software are used within the frame of standards and/or recommendations but do not replace them.

## 2.1. Main characteristics

xRapid Group has developed a fully automated microscope, patent pending, which consists in a phase contrast microscope (PCM) retrofitted with a set of motors to control the stage movement in three orthogonal directions (x, y and z) with various accuracies. For mold spores analysis, the microscope is operated in bright field mode (the phase contrast ring is removed from the phase condenser). This enables a full sample to be imaged within a few minutes. A series of images are taken by an iPad at increasing depths, from which an autofocus measure is calculated to image the next field. At the same time, a convolutional neural network (CNN) is used for our AI to characterize the objects in the field of view. All the analysis is performed locally on the device, none of the images are uploaded to a server, so that remote work in a poorly connected area is permitted. While we usually refer to AI as Deep Learning, one should notice that xRmold system is not self-learning: all the data has been extracted by humans, and validated by humans. The system shipped is not evolving between updates of the app, which enables to guarantee its performance and pass a certification.

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

## 2.3. Standards and paths

xRfiber supports a large number of standards, which come with specificities, whether they are about the objects counted (for example, some standards specifically request *not* to count objects that are touching debris, while others have different strategies), or about the path that one must apply to scan the sample.

The following standards are currently supported:

-   NIOSH 7400 (Type A & B)
-   OSHA id 160
-   NOSHC-3003
-   IRSST 243-1
-   HSG248
-   NF X43-269
-   NBN T 96-102

Four sample geometries and therefore paths are supported: quarter disk oriented right or up, and half disk oriented horizontally or vertically.

\*\*\*\*\*\*\*\*\*\*\*\*\*\* ## 2. REQUIREMENTS
- xRmicroscope: the xRmicroscope Mark I used for xRfiber, motorized on three axes (X, Y and Z), operated via Bluetooth or Ethernet.
	- Firmware version: 1.10.01, will be checked remotely by xRapid
- iPad: compatible models are iPad Pro 10.5”, iPad Pro 11” (2019), iPad Air 4
- iPad support/cradle compatible with your device
- Minimum iOS requirement: current version, i.e. iOS 14.3
---- 

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

This is the procedure that was used to mount cultures from Pétri dishes.

- On a clean microscopic glass slide, add a drop of 70% ethanol
- Add the fungal specimen to the drop of alcohol using a sterile mounter such as an inoculation loop (from solid medium), depending on the sample of use.
- Tease the fungal sample of the alcohol using a needle mounter, to ensure the sample mixes well with the alcohol.
- Using a dropper or pipette, add one or two drops of Lactophenol Cotton Blue Solution (prepared above) before the ethanol dries off.
- Carefully cover the stain with a clean sterile coverslip without making air bubbles to the stain.
- Examine the stain microscopically at 40×, to observe for fungal spores and other fungal structures.
- If the slide is acceptable, capture 150 fields using xRmold, less than 15 minutes after the slide has been mounted.

The procedure used to mount samples from air cassettes is as follows.

**TODO: add process for air cassettes**

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

![][image-1]

**TODO: this figure must be changed to reflect the 50 fields option**

**Note**: for the sake of simplicity, it is not envisaged to enable a vertical mount at the moment. Do not hesitate to contact us if this is standard practice in your laboratory. 

**Note 2**: half measurement not available in first alpha version, undergoing testing in our laboratory for now.

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

![][image-2]

Figure 6.1. xRfiber Microscope components

Additional components in the box are shown in Figure 6.2.

![][image-3]

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

![][image-4]

Figure 6.3. box contents

2.  GETTING THE MICROSCOPE OUT OF THE BOX

When deciding where to place the xRfiber Platform, consider the following:

- The platform should be placed on a stable, level surface
- The platform should be placed conveniently as to minimize the need to move after initial setup
- The area/room the platform is placed in should have consistent, even lighting as to prevent errors due to fluctuations in ambient lighting
- Once a location has been selected, take the microscope out of the box and place it in the selected area
- Remove the plastic wrapping from the microscope.

Verify that the head of the microscope (A) is aligned with the body (B). If not, slide the head into alignment with the body by hand: apply a slight rotation of the head to align its edges with those of the body.

![][image-5]![][image-6]

Figure 6.4. Alignment of the microscope head

Verify that the adjustable C-Mount Adapter (n°18) is aligned with the head of the microscope. If not, use a Allen wrench H3 (not included) and adjust the adapter after loosening the screw.

Remove both Ocular Covers (n°35). Eventually use a air duster (not included) in the ocular openings to ensure that they are free of debris and dust.

![][image-7] ![][image-8]

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

**Useful tip**: as we are working around some automated light source intensity setting, we have found it useful to use the phase ring to get the focus on the spores first, and then slide it out before starting the analysis.

### Koehler illumination
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

![][image-9] ![][image-10] ![][image-11] ![][image-12]

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

![][image-13]

Figure 6.7. unbalanced (left) and perfectly flat orientations of the iPhone in its cradle and on stage

## 6.2. Device (iPhone/iPad) setup

After going through Apple’s initialization guide, ensure the following:

-   The device is logged into an iCloud account (this is required for location services to be active which is required for device use records).
-   The device is connected to the internet (this is required to upload usage records for billing purposes).

Open the Apple App Store and select the Search tab in the bottom right of the screen. Search for “xRmold” and the application should appear in the results list. Press the Install option and confirm the installation with your password/thumbprint. Once the application is installed, turn on the microscope and then open the application once the LED light source has finished blinking three times (approx. 3-5 seconds from powering on).

**NOTE**: when the microscope is switched on, the light first blinks three times. It is an indicator that the Bluetooth has been initialized and the microscope is now ready to interact with the Software (the xRmold app).

The app is released via Diawi during the alpha/beta testing periods, it is made available on the App Store afterwards. The user gets notified by email that a new version is available, with the release notes of the update. The user also gets in his email and the iPad’s email the link to download the app.
Once the link is tapped on the iPad or entered manually into Safari (the iPad’s web browser), a window offering to install the app is accessed.

**Important when updating from Diawi**: in order to be able to install the app, one needs to tap the “aA” button in the Safari top bar, and pick “Request mobile website” from the pop-up box. Then one can hit the “Install this app” button in the middle of the page. A message box will come up asking for confirmation of installation.

**App Store update**: we recommend that the iPad is setup to auto-update the apps installed. This is performed nightly when the iPad is connected to the internet.

### 4.4. First step: logging in

In the xRmold app, from the main screen, open the “Settings” by tapping the upper right button, and get to the last thumb “Institution”. Normally you should not be logged in as an institution when first launching the app. XRapid creates an account for your institution and delivers by email a username and password. The easiest is to copy the username and then the password from the email you have received. Upon logging in, your institution details, logo, etc... will be populated.

This step is usually performed during installation and training.

**Important**: one needs to be connected to the internet for this process to work.

**Note**: one should only need to login once. Do not hesitate to contact us should some details be missing or incorrect.

### 4.5. Performing an analysis
The method is analogous to that used by a human analyst:
- position the microscope slide either manually or using the screen controls at the beginning of the trace: is is useful to rotate the turret out of position and adjust the position of the slide to the light spot of the condenser
- Adjust the focus manually
- Hit the start button.
The slide will then be scanned though 150 steps or 50 steps, depending on the option chosen. The slide is scanned through the thickness, and one will see the objects/spores blur in and out. A step is considered out-of-focus when the objects/spores do not get though a position of focus during the through thickness scan. The slide scanning process includes an auto-focus adjustment from step to step.

### 4.6. Results

Results are presented according to the **ASTM D7391**. You will find the raw counts, the spores per volume if the volume was indicated, as well as the total percentage in the table. We also indicate the percentage of coverage of the trace.

The results can be exported as an image or a PDF, or to Excel as a comma separated value file (CSV option).

## 5. ARTIFICIAL INTELLIGENCE

### 5.1. Basics

The app xRmold uses a heavily customized version of an object detector, which has two functionalities:
- detect the position of the objects the AI has been trained to recognize
- Classify those objects, i.e. attribute them a label and a confidence.

### 5.2. Confidence

The confidence is an agnostic measurement of probability that the AI calculates, it goes from 0 to 100%. In essence, we chose to limit the mold spores found to certain thresholds of confidence, in order to limit the number of false positives and false negatives. To do so, we did accept a certain level of “Unidentified Spores”, which you will see in the report. Those represent the entities that the AI identified, perhaps rightly, that the classifier could not sort with an acceptable confidence.

In practice, we have experienced great difficulties between some classes, and they mostly come from spores that are somewhat damaged: a squished stachybotrys can ressemble a chaetomium, and a folded chaetomium can ressemble a stachybotrys, for example.

### 5.3. Reviewing the results

Tapping on the images icon from the main results view will bring up a collection view of all the fields captured. One can select the fields from the classes they include by long-pressing the classes selector at the bottom right. Selecting and de-selecting classes updates the underlying images. This is particularly useful to find some interesting fields.

The images show classes and their confidence when this option is selected.

### 5.4. Species and legend

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

### 5.5. How the AI is trained

Each specie is cultured and sampled at 3-5, 7-10 and 15 days on at least 3 slides. At least 150 fields are captured on each slide. Each field containing spores is manually annotated, where each spore is identified by position and class. The AI is trained on all the fields and the selected classes at once — about 30’000 samples. A full training takes about 3 days. Transfer learning, when adding for example 1-2 classes to the dataset, takes about half a day if all goes well.

The AI is tested and validated on independent sets from training, created using different slides from the same cultures.

**Note**: it is always useful to have an independent validation set from field slides, we will welcome images without annotations but description to this effect.

**Note**: it will be shown in the app utilization section how to change the labels of a spore. When this is performed, the image is sent back to our servers, and may be used in our training set after the change has been confirmed by our analysts.

# 6. XRMold app

[1]:	https://www.amazon.com/Lactophenol-Cotton-Fungal-Hardy-Diagnostics/dp/B0732CDHHT
[2]:	https://www.sigmaaldrich.com/catalog/product/sial/61335?lang=fr&region=FR
[3]:	mailto:%20support@xrapid-group.com
[4]:	mailto:%20support@xrapid-group.com
[5]:	mailto:support@xrapid-group.com
[6]:	https://apps.apple.com/fr/app/koehler-tutor/id1281328178?l=en

[image-1]:	https://xrapid-group.github.io/xrmold/Pictures/XRmold_Sample_Geometry.png
[image-2]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_1.png
[image-3]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_2.png
[image-4]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_3.png
[image-5]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_4_a.png
[image-6]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_4_b.png
[image-7]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_5_a.png
[image-8]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_5_b.png
[image-9]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_7_a.png
[image-10]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_7_b.png
[image-11]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_7_c.png
[image-12]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_7_d.png
[image-13]:	https://xrapid-group.github.io/xrfiber/Pictures/Figure_6_8.png