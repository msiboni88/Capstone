# Capstone

Create image recognition model that can answer the age old question, is this a Chihuahua or a Blueberry Muffin: 
![](https://github.com/msiboni88/Capstone/blob/master/images/1*bt-E2YcPafjiPbZFDMMmNQ.jpeg)


### Status Update

I currently have overt 1600 images of chihuahuas and over 1600 images of muffins scraped form google images, processed in to a numpy array of greyscale values for all pixels (see files tab, c_array.npy and m_array.npy). 

I ran in to issues finding enough photos of blueberry muffins. To address this, I translated "blueberry muffin" in to every language that uses the latin alphabet and searched for all of the translations I got. This enabled me to find images that were not labeled in English and nearly doubled my data set. 

I also ran in to issues saviong numpy array files (and used all the disk space on my computer attempting to save these files). Eventually I learned the issue was because I was attempting to use my computer while processing these images as 1500X1500 pixel files. When I reduced the file size to 300X300 pixels, I was able to process all my images without issue. 

While processing the images, I found that ~1% of the images I downloaded that could be opened by my computer were unable to be opened by my program. I am not sure why these files behaved in this manner, but it was a small enough proportion of my data set that I simply removed these images. 

