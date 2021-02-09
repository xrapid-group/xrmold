# xRmold Quick Start Guide

Document version: 0.1 alpha

App Version: 0.32.0 Build 33

## 1. PURPOSE

Thank you for volunteering in testing xRmold in its alpha/beta stage. xRmold is a new product and needs to be put through its paces before, hopefully, being released to industrial hygiene specialists. This document is a “quick start guide”, meaning that it is _not_ a Standard Operating Procedure or Manual, which will come later.

## 2. REQUIREMENTS
- xRmicroscope: the xRmicroscope Mark I used for xRfiber, motorized on three axes (X, Y and Z), operated via Bluetooth or Ethernet.
	- Firmware version: 1.10.01, will be checked remotely by xRapid
- iPad: compatible models are iPad Pro 10.5”, iPad Pro 11” (2019), iPad Air 4
- iPad support/cradle compatible with your device
- Minimum iOS requirement: current version, i.e. iOS 14.3

## 3. SLIDE PREPARATION
The analysis process was designed for Air-O-Cell type slides — spore traps. 

### 3.1. Staining
#### 3.1.1. Definition
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

#### 3.1.2. Reagents of Lactophenol Cotton Blue (LPCB) Staining

A preparation of 50ml Lactophenol cotton Blue staining solution is made up of:
- Distilled water 50ml
- Cotton Blue (Aniline Blue) 0.125g
- Phenol Crystals (C6H5O4)  50g
- Glycerol 100ml
- Lactic acid (CH3CHOH COOH) 50ml
- 70% ethanol

Note: Lactophenol Cotton Blue solution is prepared at least 2 days before use.

#### 3.1.3. Preparation of Lactophenol Cotton Blue solution

Lactophenol Cotton Blue solution is prepared for over two days leaving the reagents undisturbed to allow dissolving and maturation.

Day 1: Dissolve the cotton blue in distilled water and leave to rest overnight. This eliminates insoluble dye.

Day2: Using protective gloves, add phenol crystals to lactic acid in a glass beaker and stir using a magnetic stirrer until the crystals dissolve. Add glycerol. Filter the Cotton blue and the distilled water into the phenol + glycerol +lactic acid solution and mix.

#### 3.1.4. Procedure of Lactophenol Cotton Blue (LPCB) Staining

This is the procedure that was used to mount cultures from Pétri dishes.

- On a clean microscopic glass slide, add a drop of 70% ethanol
- Add the fungal specimen to the drop of alcohol using a sterile mounter such as an inoculation loop (from solid medium), depending on the sample of use.
- Tease the fungal sample of the alcohol using a needle mounter, to ensure the sample mixes well with the alcohol.
- Using a dropper or pipette, add one or two drops of Lactophenol Cotton Blue Solution (prepared above) before the ethanol dries off.
- Carefully cover the stain with a clean sterile coverslip without making air bubbles to the stain.
- Examine the stain microscopically at 40X, to observe for fungal spores and other fungal structures.
- If the slide is acceptable, capture 150 fields using xRmold, less than 15 minutes after the slide has been mounted.

#### 3.1.5. Limitations

- It can only be used as a presumptive identification method of fungi which should be followed up with other diagnostic tools such as biochemical and cultural examination.
- The components of the solution should be used before expiry, including the use of the solution before it expires.
- The solution may disrupt the original morphology of the fungi.
- The stain can only be used to identify mature fungi and its structures and not the young vegetative forms of fungi.
- The stain can not be stored for a long period of time.

**Important: we have noticed that the stain diffuses through the spores slowly, which confuses the AI after some time. To obtain the best results, the slides should be processed through xRmold no more than 15 minutes after being mounted in LPCB.**

#### 3.1.6. Where to get LPCB

- Lactophenol Cotton Blue, Fungal Stain, 15ml, by [Hardy Diagnostics][1]
- Lactophenol blue solution [Merck/Sigma Aldrich][2]

### 3.2. Mount

xRmold is set to analyze samples that have been laid out **horizontally** only. The microscope will scan 150 fields horizontally to capture a full trace of 10mmx1mm. The next Figure shows the correct geometry for the mount.

![][image-1]

**Note**: for the sake of simplicity, it is not envisaged to enable a vertical mount at the moment. Do not hesitate to contact us if this is standard practice in your laboratory. 

**Note 2**: half measurement not available in first alpha version, undergoing testing in our laboratory for now.

## 4. OPERATION
### 4.1. Phase ring
xRmold operates in standard transmitted light microscopy (upright microscope), which is not the case of xRfiber. If you are using the xRmicroscope for both xRfiber and xRmold, you **must remove the phase ring from the condenser before operating xRmold**.

xRmold uses the same Olympus x40 objective for mold diagnostic as xRfiber: this phase contrast objective is also perfect for transmitted light microscopy.

**Useful tip**: as we are working around some automated light source intensity setting, we have found it useful to use the phase ring to get the focus on the spores first, and then slide it out before starting the analysis.

### 4.2. Koehler illumination
While there is a certain leeway ni operating xRfiber with a quite-not-perfect illumination of the microscope (note: not for chysotile samples!), this is not the case for xRmold, where the condenser must be perfectly aligned and spaced vertically with the slide.

We recommend that the user familiarizes with Koehler illumination by using the excellent app “Koehler Tutor”, which can be downloaded from the App Store at this [link][3] if it is not installed on your iPad already.

### 4.3. App installation

The app is released via Diawi during the alpha/beta testing period, it will be available on the App Store afterwards. The user gets notified by email that a new version is available, with some release notes. The user also gets in his email and the iPad’s email the link to download the app.
Once the link is tapped on the iPad or entered manually into Safari (the iPad’s web browser), a window offering to install the app is accessed.

**Important**: in order to be able to install the app, one needs to tap the “aA” button in the Safari top bar, and pick “Request mobile website” from the pop-up box. Then one can hit the “Install this app” button in the middle of the page. A message box will come up asking for confirmation of installation.

### 4.4. First step: logging in

In the xRmold app, from the main screen, open the “Settings” by tapping the upper right button, and get to the last thumb “Institution”. Normally you should not be logged in as an institution when first launching the app. XRapid creates an account for your institution and delivers by email a username and password. The easiest is to copy the username and then the password from the email you have received. Upon logging in, your institution details, logo, etc... will be populated. 

**Important**: one needs to be connected to the internet for this process to work.

**Note**: one should only need to login once. Do not hesitate to contact us should some details be missing or incorrect.

### 4.5. Performing an analysis
The method is analogous to that used in xRfiber:
- position the microscope slide either manually or using the screen controls at the beginning of the trace: is is useful to rotate the turret out of position and adjust the position of the slide to the light spot of the condenser
- Adjust the focus manually
- Hit the start button.
The slide will then be scanned though 150 steps. As it is the case with xRfiber, the slide is scanned through the thickness, and one will see the objects/spores blur in and out. A step is considered out-of-focus when the objects/spores do not get though a position of focus during the through thickness scan.

**Note to alpha/beta testers**: please record any loss of focus and report it as soon as possible. We have done our best to ensure that the focus is kept all slide throughout, but some edge cases/mounts may still throw it off.

### 4.6. Results

Results are presented according to the **ASTM D7391**. You will find the raw counts, the spores per volume if the volume was indicated, as well as the total percentage in the table. We also indicate the percentage of coverage of the trace.

**Note**: in the current version, the results can only be exported as an image or a PDF, exporting to Excel is not yet available.

## 5. ARTIFICIAL INTELLIGENCE

### 5.1. Basics

The app xRmold uses a heavily customized version of an object detector, which has two functionalities:
- detect the position of the objects the AI has been trained to recognize
- Classify those objects, i.e. attribute them a label and a confidence.

### 5.2. Confidence

The confidence is an agnostic measurement of probability that the AI calculates, it goes from 0 to 100%. In essence, we chose to limit the mold spores found to certain thresholds of confidence, in order to limit the number of false positives and false negatives. To do so, we did accept a level of 20% of “Unidentified Spores”, which you will see in the report. Those represent the entities that the AI identified, perhaps rightly, that the classifier could not sort with an acceptable confidence.

In practice, we have experienced great difficulties between some classes, and they mostly come from spores that are somewhat damaged: a squished stachybotrys can ressemble a chaetomium, and a folded chaetomium can ressemble a stachybotrys, for example.

### 5.3. Reviewing the results

Tapping on the images icon from the main results view will bring up a collection view of all the fields captured. All functionalities are similar to xRfiber at this point, with one big exception: one can select the fields from the classes they include by long-pressing the classes selector at the bottom right. Selecting and de-selecting classes updates the underlying images. This is particularly useful to find some interesting fields.

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

**Note**: it would be useful to have an independent validation set from field slides, we will welcome images without annotations but description to this effect. 

[1]:	https://www.amazon.com/Lactophenol-Cotton-Fungal-Hardy-Diagnostics/dp/B0732CDHHT
[2]:	https://www.sigmaaldrich.com/catalog/product/sial/61335?lang=fr&region=FR
[3]:	https://apps.apple.com/fr/app/koehler-tutor/id1281328178?l=en

[image-1]:	https://xrapid-group.github.io/xrmold/Pictures/XRmold_Sample_Geometry.png