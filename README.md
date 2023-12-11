# fast-dem-coregistration
FastDCore - Fast DEM CoRegistration

This method finds coherent areas that seem unchanged and uses them to find the ideal "tie points" between two rasters for coarse co-registration.

It then proceeds to find a swarm of other tie points for fine co-registration and finally considers gross differences are changed pixels. 

Algorithms used for corse and fine co-registration are an ensamble of fast point detectors, swarm particle optimization (fancy name for robust  regression), artificial intelligence and more standard ....

# Method 

We apply phase correlation over multiple subwindows that are determined by an 
initial salient features detection and extraction. 
Phase correlation uses the frequency-domain representation of the data and
then analysing the inverse transform of the cross-power spectrum. The XY shift
is determined by the position of the cell with the maximum value in
this last product.  



is an approach to estimate the relative translative offset between two similar
