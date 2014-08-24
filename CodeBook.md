
CodeBook

The tidy data set consists of the following cariables;
 
activity - This is a string containing the name of activity performed during session.
WALKING WALKING_UPSTAIRS WALKING_DOWNSTAIRS SITTING STANDING LAYING

subject - This is an integer value representing the identifier for the  test subject. Integer value valid range: 1-30

Columns 3:88 contain the feature measurements for 85 different measurements collected from the pedometersi, smart phone,
gyroscope,  and other accelerometers. 

Each measurement is ithe estimated value for:

n(): Mean value
std(): Standard deviation
mad(): Median absolute deviation 
max(): Largest value in array
min(): Smallest value in array
sma(): Signal magnitude area
energy(): Energy measure. Sum of the squares divided by the number of values. 
iqr(): Interquartile range 
entropy(): Signal entropy
arCoeff(): Autorregresion coefficients with Burg order equal to 4
correlation(): correlation coefficient between two signals
maxInds(): index of the frequency component with largest magnitude
meanFreq(): Weighted average of the frequency components to obtain a mean frequency
skewness(): skewness of the frequency domain signal 
kurtosis(): kurtosis of the frequency domain signal 
bandsEnergy(): Energy of a frequency interval within the 64 bins of the FFT of each window.
angle(): Angle between to vectors.

The 561 features are reduced to only the mean or standard deviation measurements for a particular axis represented 
as a floating point values:

tbodyaccmeanx tbodyaccmeany
tbodyaccmeanz tbodyaccstdx
tbodyaccstdy tbodyaccstdz
tgravityaccmeanx tgravityaccmeany
tgravityaccmeanz tgravityaccstdx
tgravityaccstdy tgravityaccstdz
tbodyaccjerkmeanx tbodyaccjerkmeany
tbodyaccjerkmeanz tbodyaccjerkstdx
tbodyaccjerkstdy tbodyaccjerkstdz
tbodygyromeanx tbodygyromeany
tbodygyromeanz tbodygyrostdx
tbodygyrostdy tbodygyrostdz
tbodygyrojerkmeanx tbodygyrojerkmeany
tbodygyrojerkmeanz tbodygyrojerkstdx
tbodygyrojerkstdy tbodygyrojerkstdz
tbodyaccmagmean tbodyaccmagstd
tgravityaccmagmean tgravityaccmagstd
tbodyaccjerkmagmean tbodyaccjerkmagstd
tbodygyromagmean tbodygyromagstd
tbodygyrojerkmagmean tbodygyrojerkmagstd
fbodyaccmeanx fbodyaccmeany
fbodyaccmeanz fbodyaccstdx
fbodyaccstdy fbodyaccstdz
fbodyaccmeanfreqx fbodyaccmeanfreqy
fbodyaccmeanfreqz fbodyaccjerkmeanx
fbodyaccjerkmeany fbodyaccjerkmeanz
fbodyaccjerkstdx fbodyaccjerkstdy
fbodyaccjerkstdz fbodyaccjerkmeanfreqx
fbodyaccjerkmeanfreqy fbodyaccjerkmeanfreqz
fbodygyromeanx fbodygyromeany
fbodygyromeanz fbodygyrostdx
fbodygyrostdy fbodygyrostdz
fbodygyromeanfreqx fbodygyromeanfreqy
fbodygyromeanfreqz fbodyaccmagmean
fbodyaccmagstd fbodyaccmagmeanfreq
fbodybodyaccjerkmagmean fbodybodyaccjerkmagstd
fbodybodyaccjerkmagmeanfreq fbodybodygyromagmean
fbodybodygyromagstd fbodybodygyromagmeanfreq
fbodybodygyrojerkmagmean fbodybodygyrojerkmagstd
fbodybodygyrojerkmagmeanfreq angletbodyaccmeangravity
angletbodyaccjerkmeangravitymean angletbodygyromeangravitymean
angletbodygyrojerkmeangravitymean anglexgravitymean
angleygravitymean anglezgravitymean

Data was extracted from original UCI HAR Dataset. Activity labels, subject id, and features were merged with the training data from the test and train data sets. Only measurements involving mean or standard deviation were used for this data set.

Finally, the train and test sets were merged and aggregated by activity and subject, aggregating on the mean for each category.

