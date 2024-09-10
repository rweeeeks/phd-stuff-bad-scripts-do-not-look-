This is just stuff I've needed to script during my time analyzing a particular type of dataset. 
They're not designed to be used by anybody and is mostly here as evidence of me being a person in 2024

matlab_tonehalf_nice.py -- this is an individual trace t1/2 calculator with a few tweaks that I use to account for the lower signal/higher noise datasets
                        -- half max is defined as (baseline + maximum)/2 like other calculators but
                            --baseline is defined as the average of the first 10 data points
                            --maximum is defined as the average of the top 5 (or you can modify easily) values, *outside of the baseline* 
                            --script excludes any data set with maximum<baseline
                            --Linear interpolation of time half max data point and previous data point for more precision
