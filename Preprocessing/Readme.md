## Preprocessing timeline:
- **February 3, 2024** : Initail preprocessing using direct methods like pixel differencing.
- **February 9, 2024** : Exploration of other preprocessing methods like feature extraction using CNN and image transformation methods to overcome alignment issues.
- **February 10, 2024** : Exploring more on Convolution feature extraction methods. Tried out new Kernel iteration technique.
- **February 11, 2024** : Exploring image registration and alignment based methods.
- **February 11, 2024** : Finalized Preprocessing method.

## Chosen Methodology:
- Absolute differencing between the template and test image has been performed and pixels with difference have been converted into red pixels (0,0,255) - BGR format.
- This same is passed to the model for training.
- We can notice that this preprocessing technique is prone to alignment issues but yet it is very effective in addressing defects than other tested techniques.
- The next favourable preprocessing is edge detection, image subtraction and addition of edge to the difference pixels. We were able to reach maximum accuracy of 87 % with the same configuration we apllied on the considered absolute difference method.
- Next we preferred image alignment based technique to rectify the redundant pixels. We found that image alignment algorithms works with a concept of key point identification. This contradicted with many cases in PCB dataset where it is not able to map the key point vector from two images, often leading to irrelevant causing more redundancy than absolute difference.
- CNN based methods seemed to be computationaly intensive for preprocessing. Utilizing normal CNN resulted in poor performance as it works more like a feature predictor and using that feature predictions we are not able to map the differences.  
