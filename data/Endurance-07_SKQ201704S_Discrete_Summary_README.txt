Endurance 07 (R/V Sikuliaq, 2017-04-09 to 2017-04-23) Discrete Sampling README

Revision History:

1.00 (2019-##-##) -- Assembled and published to Alfresco 2019-##-##. Still missing Discrete Salinity estimates.

General Notes:

Data sheets containing the discrete sampling estimates that we receive from the different laboratories that process the samples are provided "as is" for the user to review. 

We use the value -9999999 to represent missing values. The Discrete Data Flags (included in the spreadsheet and reproduced below) and the Summary Notes shown below can be used to determine why the missing value was set. 

If a discrete sample field contains DIC-###, CHL-###, OXY-###, PSU-###, or NUT-###, that is the sample bottle number and not analyzed data. When the analyzed data becomes available, these values will be replaced with the discrete sample data. 


Summary Notes:

Notes are reported per Cruise ID, Cast Number, Bottle Number and Discrete Data Flag. Where note(s) are applicable to all casts and all bottles, the Cast Number and Bottle Number entries are set to "All Casts" and "All Bottles", respectively. Otherwise, specific numbers are used.

SKQ201715S, Cast 001, Bottle 20, Discrete Oxygen Flag -- Not enough points were recorded to make a valid regression, and therefore a sample value could not be obtained.

SKQ201715S, Cast 022, Bottle 02, Discrete Oxygen Flag -- Possible pipette malfunction. Processed sample value looks OK, but marked as questionable sample.


SKQ201715S, All Casts, All Bottles, Discrete Nutrients Flag -- All samples processed by Dr. Burke Hale's laboratory group at Oregon State University with the following reported nominal lower concentration detection limits for each nutrient:

        Phosphate			0.01 uM
        Nitrate+Nitrite		0.06 uM
        Silicate	        0.19 uM
        Nitrite             0.014 uM
        Ammonium			0.05 uM 
		
Concentration values are reported below the detection limits to provide users with an idea of the lab's precision (Joe Jennings, personal communication). Nitrates are estimated and reported in the Discrete Summary spreadsheet by subtracting Nitrite from Nitrate+Nitrite.

SKQ201715S, All Casts, All Bottles, Discrete Salinity Flag -- Waiting for analysis results. Will update spreadsheet once we have the updated values.

SKQ201715S, All Casts, All Bottles, Discrete Alkalinity Flag -- This value is not measured directly by the analysis lab that processes our samples. Instead, see the calculated Alkalinity value, which is reported at in-situ temperatures.

SKQ201715S, All Casts, All Bottles, Discrete DIC Flag -- All values are reported at in-situ temperatures.

SKQ201715S, All Casts, All Bottles, Discrete pCO2 Flag -- All values are reported at in-situ temperatures.

SKQ201715S, All Casts, All Bottles, Discrete pH Flag -- This value is not measured directly by the analysis lab that processes our samples. All Calculated pH values are reported in total scale referenced to in-situ temperature.

Further Notes:

More Information provided by Dr. Burke Hales (we use his lab to process the DIC samples) regarding the DIC samples is copied from and email exchange here.

---------- Forwarded message ---------
From: Burke Hales <bhales@coas.oregonstate.edu>
Date: Thu, Jan 31, 2019 at 3:03 PM
Subject: Re: OOI Water Sampling Carbon Questions
To: <wruef@uw.edu>
Cc: Joe Jennings <jenningj@ceoas.oregonstate.edu>

Hi Wendi—

Joe’s out sick and he forwarded your message on to me.

1. Yes. pHt, not pHnbs or pHsws

2-3. All parameters are reported at in situ conditions. We essentially
use the lab-T TCO2 and pCO2 to calculate Alkalinity, and then use the
TCO2 and Alkalinity at in situ T and P (more on the fine points of
this, below) to calculate the in situ distributions. I do not report
values at reference temperatures.

4. I wrote my own calculation routine.  It uses the carbonic acid
dissociation constants of Millero, 2010, with the full-resolution
parameters provided by Frank himself (the values in his paper do not
report sufficient significant figures). These are the same as Lueker’s
constants at S>25.  I use Millero’s 1995 Kw, and Dickson’s 1990 Kb.  I
use Mucci’s 1980 Ksp for calcite and aragonite. I use Weiss’  1973 Kh.
My Alkalinity is modeled as:

HCO3- + 2CO3= + B(OH)4- + OH- - H+

5. See 2-3 above.  All my results are reported at in situ conditions.
Our analytical temperatures are typically 22C, and are recorded but
not controlled.

Fine point #1.  There is some ambiguity in reporting pCO2 at in situ
pressure.  We know almost nothing about the total-pressure dependence
of Kh, but what we do know suggests that gas solubility decreases as
total pressure increases.  That factor is not incorporated in any of
my calculations and the pCO2 I report at in situ pressure is probably
slightly lower than the true partial pressure if we were able to
measure it.  We do know about the pressure dependence of the other Ks,
though, and they suggest that CO2aq will decrease with increasing
pressure, which means that pCO2 will also decrease.  The marine
physiologists think organisms respond to the partial pressure of
dissolved gases, and not their dissolved concentrations, so I have
provided both CO2aq and pCO2 at in situ conditions, even if we are
uncertain about the magnitude of the Kh pressure effect.  If you want
to know the ‘potential pCO2’ or that which the water sample would have
if it were at the surface, you need to take the reported TCO2 and
Alkalinity, T< and S, and recalculate with P = 1 atmosphere.

#2.  The alkalinity I report is robust and independent of
contributions from non-carbonate acids/bases, and none of the other
calculated parameters are sensitive to the inclusion or exclusion of
non-carbonate alkalinity species.  Measured TA, however, will include
those components to varying degree, and calculations based on those
measurements without knowledge of the other contributing species will
contribute to the error propagation of calculated parameters.

Let me know if you have other questions.

Best —
Burke

Burke Hales
Professor
CEOAS
Oregon State University
(541)737-8121

On Jan 31, 2019, at 10:35 AM, Joe Jennings
<jenningj@ceoas.oregonstate.edu> wrote:

Burke,

I’m going to pass this to you.

Joe

----- Forwarded Message -----
From: Wendi Ruef <wruef@uw.edu>
To: Joe Jennings <jenningj@coas.oregonstate.edu>
Cc: Sheri N. White <swhite@whoi.edu>, Andrew <areed@whoi.edu>, Katie
Bigham <bighamkt@uw.edu>, Orest Kawka <kawkaoe@uw.edu>, Chris Wingard
<cwingard@ceoas.oregonstate.edu>
Sent: Wed, 30 Jan 2019 08:09:01 -0800 (PST)
Subject: OOI Water Sampling Carbon Questions

Hi Joe,

We are compiling a combined field-verification summary that will
include inorganic carbon sample analyses from multiple labs.  Since
these labs measure different parameters (labs that directly measure
TCO2 and pCO2 and provide the calculated TAlk and pH vs labs that
directly measure TCO2, TAlk, and pH and provide the calculated pCO2),
we want to make sure we are reporting values as consistently as
possible.  We will still be providing the original reports as received
from each lab, and will provide the combined summary in addition.  If
you have a chance, would you mind answering the following questions in
regards to how your lab outputs results?

Thank you in advance!

1. Is pH reported in “total scale"?

2. When a pH sample is analyzed at lab temperature, is it typical to
report analysis temperature and then the pH values in reference to
that analysis temperature, or is there a correction applied for in
situ temperature before pH values are reported? (i.e. is the reported
pH at the analysis temp or the in-situ temp?)

3. For calculated parameters (e.g. pH from TCO2 and pCO2), are they
calculated with respect to the analysis temperature or the in-situ
temperature?

4. If calculated values are provided, what is the software package and
version used?

5. If measured values were analyzed at different temperatures, does
each measured value need to be paired with the individual
corresponding analysis temperatures to aid in calculating other
inorganic carbon parameters and ensuring proper quality assurance?

Please Reply To All with your answers.


Sheri, Andrew, Wendi, Katie, Chris, Orest
The OOI Water Sampling Group


Discrete Data Flags:

* Cast Flags:		Bit 	Flags
					0		Notes/Other
					1		Delayed start to data collection
					2		Acceptable; normal cast according to SOP
					3		Non-standard winch speed
					4		Non-standard surface soak time
					5		Non-standard bottle soak time before Niskin trip
					6		Sensor issues but cast completed and data collected
					7		Cable issues but cast completed and data collected
					8		Winch issues but cast completed and data collected
					9		Premature cast end with data and/or data loss
					10		Significant ship heave
					11		Station position not adequately maintained during cast
					12		Tow-yo, Yo-yo cast
					13		ROV bottle sample
					14		Unassigned
					15		Unassigned

* File Flags:		Bit 	Flags
					0		Notes/Other
					1		Data cast only, no Niskins triggered
					2		Acceptable; file processed according to SOP
					3		File processed using modified parameters
					4		File processed using alternate XMLCON
					5		Missing scans as indicated by modulo error counts
					6		Missing metadata
					7		Unassigned
					8		Unassigned
					9		Unassigned
					10		Unassigned
					11		Unassigned
					12		Unassigned
					13		Unassigned
					14		Unassigned
					15		Unassigned

* Parameter Flags:	Bit 	Flags
					0		Notes/Other
					1		Not calibrated
					2		Acceptable measurement
					3		Questionable measurement
					4		Bad measurement
					5		Not reported
					6		Calibration coefficients > 1 year old
					7		Corresponding discrete sample
					8		Unassigned
					9		Unassigned
					10		Unassigned
					11		Unassigned
					12		Unassigned
					13		Unassigned
					14		Unassigned
					15		Unassigned

* Niskin Flags:		Bit 	Flags
					0		Notes/Other
					1		Bottle information unavailable
					2		No problems noted
					3		Leaking
					4		Ran out of water during sampling
					5		Vent open
					6		Misfire at wrong depth
					7		Unknown problem
					8		Unassigned
					9		Unassigned
					10		Unassigned
					11		Unassigned
					12		Unassigned
					13		Unassigned
					14		Unassigned
					15		Unassigned

* Sample Flags:		Bit 	Flags
					0		Notes/Other
					1		Sample for this measurement was drawn from water bottle but analysis not received.
					2		Acceptable; sample processed according to SOP
					3		Questionable measurement
					4		Bad measurement
					5		Not reported
					6		Sample collected out of order
					7		Sample processed using alternative method; see notes
					8		Unassigned
					9		Sample not drawn for this measurement from this bottle
					10		Unassigned
					11		Unassigned
					12		Unassigned
					13		Unassigned
					14		Unassigned
					15		Unassigned

* Duplicate Flags:	Bit 	Flags
					0		Notes/Other
					1		Duplicate analysis on same sample
					2		Single sample
					3		Duplicate analysis from same Niskin
					4		Triplicate analysis from same Niskin
					5		Unassigned
					6		Unassigned
					7		Unassigned
					8		Unassigned
					9		Unassigned
					10		Unassigned
					11		Unassigned
					12		Unassigned
					13		Unassigned
					14		Unassigned
					15		Unassigned
