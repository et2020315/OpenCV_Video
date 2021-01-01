# CSCE491-FaceER
For course csce 491

The best 2 models:

model 5.modified version of model 4: (might have higher false negative rate, but low false positive rate)
model5.json + weight5.h5

model 4. Built by Ezgi Akcora:
model4.json, model4.h5

Model that is no longer using:

model 3. modified version of model 4, (higher false positive rate)
model3.json, weight3.h5

model 2.Model that uses convolutional blocks and HOG
(h5 file and json file not put in the repo, avoid causing confusions)
They could be generated by running model2.ipynb

model 1. Model that only uses convolutional blocks without HOG, did not keep track of the record so I lost it.


Some of the helper function from viewModel(1).ipynb is from Ezgi Akcora's code.

Steps:

1. Use the models provided by OpenCV library and other library:
shape-predictor-68-face-landmarks.dat and haarcascade-frontalface-default.xml

2. In Video-useModelWriteVideo2.ipynb, change the path in line 12 in main() function to /content/drive/My Drive/(model-structure-you-pick).json, you can choose model3.json, model4.json and model5.json and change the path in line 17 in main() function to /content/drive/My Drive/(modelweights-you-pick).h5 (you can choose weight3.h5 or model4.h5 or weight5.h5. (I recommend choosing model4.json+model4.h5 or model5.json + weight5.h5)

3. In Video-useModelWriteVideo2.ipynb, replace the path in line 1 to the path to the text file with links you scraped in it. If you don't have a link, please use the notebook scrapeLinks.ipynb and follow the instruction "Collecting links from YouTube 8M Open data set" below to collect the links,

Collecting links from YouTube 8M Open data set:

Provide a text file that contains the links that you scraped. If you don't have any text file that contains the links, you can got to http://research.google.com/youtube8m/explore.html and collect the html and use scrapeLinks.ipynb to collect the links from html files.

4. Run Video-useModelWriteVideo2.ipynb
