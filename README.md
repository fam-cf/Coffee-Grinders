# Coffee-Grinders

## Intro
When you first visit an espresso forum asking for advice, the first thing you will often run into is people asking not what machine you're going to get, but the grinder. This is because the particle distribution that your grinder produces influences both the way water flows through the coffee puck and the exposed surface area of grinds available for extraction. Both of these factors will strongly affect how the end product tastes, and exactly what both of these factors have on extraction can be understood roughly through simplification, but the exact effects of these two factors in tandem with each other are actually not well understood at all. Collected in this repository are grind distributions from various grinders collected via Jonathan Gagne's coffee grind size application. The purpose of looking at these distributions is not to make direct comparisons between grinders, extropolate to taste, or to declare a winner, but rather to raise questions that can be analyzed with more detail and rigor in the future. 

## Methodology
The way in which so many grind distributions were collected was through crowd-sourcing. In order to potentially get some insight on roast effects on grind, seasoning, and coffee varietals, meta-data was collected on estimated seasoning weight, coffee roaster, varietal, and approxiate roast level. Not all the grinders present the meta-data, but data was collected anyways to increase the number of samples.

Samples were prepared as such:
1. grind setting at "medium fine filter" (aiming for ~700-800um peak mode)    
2. shadows minimized through lighting the sample below the camera or w/ a ringlight
3. clumps minimized through physical agitation, and software erasure

Caveats of measurement:
1. sample preparation: Grinds clumped depending on the grinder and the humidity, camera resolutions and photo taking quality were hugely varying, and no one used the same coffee. In addition, inconsistencies are added in post-image processing, because physical clumps are individually taken out at data points via the judgement of the person doing the processing
2. Microfines. Because of the resolution and photo preparation, the size and shape of the microfines cannot be fully accounted for in the picture. This can be addressed (but not fully solved) via color manipulation, lens correction and using higher resolution, but I felt that would close the door to the number of samples I was able to receive so ultimately, I decided against implementing stricter data collection parameters.
3. Espresso grind. A big caveat, this type of analysis is unable to use espresso grind (at least with these testing parameters). The issue with evaluating espresso grind has to do with again, the resolution and sample preparation of the photo. Because espresso grind is so small, it is much more prone to clumping due to static and is thus much harder to separate. We can measure the same grinder and coffee at various grind sizes, observe the behavior, and try to roughly exrapolate roughly what the distribution at espresso sizes looks like. However, without improved equipment and procedure, we will never be completely sure of a grinders behavior at espresso grind sizes, especially when many grinders are grinding to near turkish grind sizes for espresso.

## Observations

I compiled a few comparisons and observations in a Jupyter notebook and used Seaborn to visualize them. This is still rough around the edges and a work in progress, so feel free to discuss further with me! Click either link to render the notebook to a web browser.

[GitHub View](https://github.com/fam-cf/Coffee-Grinders/blob/main/Notes%20and%20Observations.ipynb)    
[nbviewer](https://nbviewer.jupyter.org/github/fam-cf/Coffee-Grinders/blob/main/Notes%20and%20Observations.ipynb)    

## Weibull Fitting    
This notebook is squarely a work in progress, and I would love suggestions for improvements and changes.   

[GitHub View](https://github.com/fam-cf/Coffee-Grinders/blob/main/The%20Weibull%20Distribution.ipynb)


