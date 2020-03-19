# Updates by the session

## Update at 17th March 2020

It's been a very long time since I updated this log. The functions are working and the manuscript is drafted. Release and preprint are almost ready


## up to the 12th June
* 


## up to the 8th June
lots of specific things here
* updated functions, we now can plot.sca.overlap() to compare e.g. Stroop data from session 1 and 2 in the same order of specifications - this gives a picture of how the same specification can also result in slightly different estimates.
* the function can also take a correlation output - also there is a cor.sca() correlation function now to check the correlation between two measures, at a range of specifications. 


## up to the 27th May 2019
* updated output-much prettier now
* functions massively updated to be simpler to use
  + run.sca()
  + plot.sca()
  + threshold()


## 22 May 2019 evening:
* converted code into functions:
  + all.specifications(specifications)
  + specs_data <- process.specifications(data = DPT_data,
                       specs = specs)
  + sca <- run.sca(specs_data = specs_data,
        specs = specs)
  + plot.sca(sca = sca,
         specs = specs)
  + removals <- check.removals(data = DPT_data,
               specs_data = specs_data,
               specs = specs)
  + threshold(sca = sca, 
          threshold = 0,
          use = "lower")
These functions run the generation of the specifications list, the data reduction for each specification, splithalf for each specification, plot the sca, check the number and porportion of participants and trials removed and return remaining trials per participant, and a threshold check to see the number of estimates above a certain threshold.


## 22 May 2019:
* removed printing of specification number, and have a progress bar instead. 
*made the SCA curve plot a little prettier. 
* started a paper papaja markdown document. but might first work in word for ease

