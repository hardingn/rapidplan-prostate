# rapidplan-prostate
A repository to hold RapidPlan model for CHHip based Prostate 60Gy in 20# model.
This repository was started as an example of performing version control for the UK RapidPlan Consortium (UKRC).
Future work will look to add in a proforma which describes the technical settings in the model as well as the structures that are requried in the model, how these are grown from the CTVs etc. A proforma is being developed by the UKRC for this purpose. At this time, this readme includes details for this models.
Also in future work, it would be good to develop an ESAPI script which would allow for the releavnt structures to be automatically created.

## Training Set Description
Version|Published
-------|---------
1.2 | 27/02/2020

Training Set Description | Values
-------------------------|-------
No of Plans | 58
VMAT Arcs | 1

Structures (non target) | Description
------------------------|-----------------------------------------------------
Bladder | Comfortably full
Rectum | Empty
Avoid 5mm | 1.5cm wall from PTV48. Cropped 0.2cm from PTV48,0.5cm from PTV57.6
Femoral Heads | Both heads mapped to one model structure
PTV48 DVH Opt | PTV48 DVH cropped 0.5cm from PTV57.6

Structures (targets) | Description
--|--
PTV60 | 0.5cm margin from CTV3 (but excluded from rectum)
PTV57. DVH | PTV57.6 minus PTV60
PTV48 DVH | PTV48 minus PTV57.6 
