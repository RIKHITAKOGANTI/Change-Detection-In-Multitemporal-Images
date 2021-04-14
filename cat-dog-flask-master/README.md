Change detection (CD) is essential for accurate understanding of land surface changes with multi-temporal Earth observation data. The main idea is to detect the regions of change in multiple images of the same scene taken at different times is of widespread interest due to a large number of applications in diverse disciplines, including remote sensing, surveillance, medical diagnosis and treatment, and civil infrastructure. The objective is extended to examine the effectiveness of each change detection technique regarding not only the ability to differentiate changed from unchanged areas, but also the ability to classify the changed areas according to the “from-to” identifiers. The results indicated that the post classification change detection technique provided the highest accuracy 
 principle component analysis is used  in feature detection and dimensionality reduction and k means clustering is used for clustering.
**Implementation Plan
We have gathered our dataset from Bhuvan website using LISS-III satellite. It comprises of four multispectral images of 3 bands each(R-G-B).

 We have set the latitude and longitude of a particular location for which all the images of consecutive years are displayed among which we have selected two images for our analysis.

 Initially we got four images for each year selected from which  it is  converted into single image following the raster process using the QGIS3 tool.

 Now we read our images and resize them into required size using cv2 module.

Then the difference of two images is calculated using abs function.

 Now we find principal components or the features using the functions find fvs, and find vector set.
 To the principal components obtained we apply the K-Means algorithm to generate the change map.
From the change map obtained  we calculate the percentage of change occured


