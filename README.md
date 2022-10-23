# COMP90086 Final Project: Stereo Disparity

The project is to solve Stereo Disparity based on dataset provided by COMP90086 Computer Vision, 2022 Semester 2, The University of Melbourne.

## Authors

- Xinhao Yan - 1200713 - xinhao1@student.unimelb.edu.au
- Chenyang Dong - 1074314 - doncd@student.unimelb.edu.au

## Packages required

- cv2
- numpy
- scipy
- tqdm


## Dataset

We expect that you can have a folder called **Dataset** with all required images in it. The folder should be put under the same directory aligning with our [Project.ipynb](Project.ipynb).


## To re-create our work
The notebook has been divided into different sections. 

### Prepare your dataset
In this section, you can check whether your dataset is correct by running this section. If yes, you will see an example for the data with their name and corresponding images.

### Other functions
In this section, it has most of functions used later in the experiment, including:
- 'read_image()' -  transforming the input images
- 'evaluate()' - computing the performance of the algorithm
- 'plot_record()' - plotting the performance under different window size.
- ...
    
### Start Matching 
In this section, you can start the trial experiment using the 'Match()' function. The comments in the section will guide you what and how to adjust the input varibales including the input images, window size, whether to use smooth function, whether to print the output (time taken and performance). For the result, you can get the plotting of the disparity map with the suggested matching function; and if you allow printing, you will get the performance of the algorithm including the runtime for such image, the rms (root mean squared) error between the values in your disparity map
and those in the ground truth, and the fractions of pixels with errors less than 4, 2, 1, 0.5 and 0.25 pixels.

### Are all pixels in the matching window equally important?
In this section, a gaussian filter is applied on the matching to check whether all pixels in the matching window are equally important.

### Tuning Window Size & Performance Check
In this section, by setting the input images and a range of window size you want to experiment, then by running each subsection of different matching function, it will output with the trend of the performance on the window sizes. For the last one which is ZNCC as we used for analyse, the comparision between RMSE with different window size between non-smoothed and smoothed ZNCC is also plotted.

### Smoothing Effect on RMSE
In this section, the smoothing effect is presented by using the RMSE result from previous section.

### Sub-Pixel Technique (Attempted)
In this section, sub-pixel techniques are attempted to improve our algorithm, however the result is not satisfied.

### Average Performance of Final Algorithms
In this section, all images set in the dataset is tested with our final algorithms. The performance of the algorithm including RMSE and fraction of pixels in small-error ranges are output.


