# Beauty-Predictor
The Chicago Face dataset  has been used to create a Machine Learning model as well as a Deep Learning model with Convolutional Neural Network and transfer learning with the VGG dataset. The Chicago face dataset comprises images of around 597 males and females with facial proportions and an attractiveness score. So, I use this dataset to rate myself. The machine learning model created is purely regression-based, and it assesses faces based on the dimensions of parts of the face. The second model created utilized images of 597 people, and a dense convolution with the VGG face dataset for transfer learning. So, an image can be loaded on to this model, and it would return the score. This model basically rates us purely based on the image, while the one mentioned above has a mathematical approach.

## The database can be downloaded from: 
https://chicagofaces.org/default/
(In order, to access the data, a request form has to be submitted stating the purpose and the link will be sent as a mail.)
## The VGG face-model from: 
https://drive.google.com/file/d/1CPSeum3HpopfomUEK1gybeuIVoeJT_Eo/view?usp=sharing


## Dimensions required by the ML model:

Nose_Width 	Distance between outer edges of nostrils at widest point.

Nose_Length	Distance between Forehead Bridge at level of visible upper eye edge to nose tip. For the Nose Tip, imagine a spot where the nose protrudes from the face. Optional Tip: You can make a temporary line across the eyes to get a good visual reference of where the upper eye edge is on the bridge of the nose.	

Face_Length	Distance between hairline and base of chin. Note: For some people, there may be a double chin. You may have to guesstimate. 
			
Avg_Eye_Height	Average distance between upper and lower edge of visible eye within eyelids at center of pupil for right and left eye.			
			
Avg_Eye_Width	Average distance between inner and outer corner of eye for right and left eye.			

Face_Width_Cheeks	Distance between outer edges of cheeks at most prominent points.

Forehead	Distance from center of hairline to the center between the eyes. Tip: You can make a temporary box that goes between the eyes to get a good visual reference on where to start on the bridge of the nose.
		
Asymmetry_pupil_top	Absolute value difference between distance between pupil center to hairline for right and left.			
		
Pupil_Lip_L	Distance between pupil center to top edge of lips.			
Asymmetry_pupil_lip	Absolute value difference between distance between pupil center to top edge of lips for right and left.	

Midcheek_Chin_L	Distance between midcheek and bottom of chin.	

Cheeks_avg	Average distance between midcheek and bottom of chin for right and left.		
		
Midbrow_Hairline_L	Distance between midbrow to hairline. This should be above the pupil of each eye in the middle of the eye brown. 

Heartshapeness	Face width at cheeks divided by face width at mouth

Noseshape	Nose width divided by nose length		

LipFullness	Lip thickness divided by face length		

EyeShape	Eye height divided by eye width	

UpperHeadLength	Forehead divided by face length		

MidfaceLength	(Average pupil to lip for right and left) divided by face length	

ChinLength	Bottom of lip to chin divided by face length		

ForeheadHeight	(Average midbrow to hairline for right and left) divided by face length

CheekboneHeight	(Average midcheeck to chin for right and left) divided by face length		

CheekboneProminence	(Face width at cheek minus face width at mouth) divided by face length		

FaceRoundness	Face width at mouth divided by face length	

fWHR	Facial width to height ratio		

### Each measurement taken in cms must be converted to inches (divide by 2.54) and multiplied by a factor of 100.
