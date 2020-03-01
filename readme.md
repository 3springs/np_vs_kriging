Quick test of Neural Processes vs Kriging (Gaussian Processes). 


The results look promising in terms of gridding fit. You can likely get a good result with a better scalability than Kriging (O(x) vs O($x^3$)). However, it does show some neural network like behviour: where it wildly extrapolates at the edges instead of returning to the mean.

# Results 

Results on test set:

![](docs/box_plot.png)

Kriging:

![](docs/kriging.png)


Neural Processes:

![](docs/np_grid.png)


Map with NP grid

![](docs/map.png)

# Data 
For data I used the lead soil samples from the [meuse dataset](http://spatial-analyst.net/book/meusegrids). 

> The meuse is a classical geostatistical data set used frequently by the creator of the gstat package to demonstrate various geostatistical analysis steps. The point data set consists of 155 samples of top soil heavy metal concentrations (ppm), along with a number of soil and landscape variables. The samples were collected in a flood plain of the river Meuse, near the village Stein. This zip files contains additional gridded maps (2-40 m resolution), which are used in the exercise 'First steps'.

