
## Meredith VanAcker - Project Proposal 
## Parameterize a resistance surface for white-tailed deer dispersal in the northeastern United States.

I am interested in parameterizing landscape resistance values for white-tailed deer (*Odocoileus virginianus*) movement in the northeastern United States. This would inform my understanding of how tick vectors may be moved across heterogeneous space by their final host, white-tailed deer. The dispersal of adult ticks via deer is important because it is one of the main contributors to the spread and establishment of new tick populations. I can use simulations to understand how many deer colonizers are required to get a constant probability of colonization and what landscape features serve as barriers to deer movement.

### **The data:** 
I will web scrape sites such as GBIF, BISON and Movebank to establish a large collection of deer occurrence data within the states of New Jersey, New York and Connecticut. I have radiotracking data from 20 male deer individuals on Staten Island and deer telemetry data from Movebank that I will use to validate my resistance surface cost values. The spatial data will be simulated and derived from the National Land Cover Database 2011 and the NYC Open Data Landcover Raster 2010. 

### **The tools:**
**1.)** I will use **Circuitscape** to produce current density maps that represent the probability of deer movement on Staten Island. 

**2.)** I will validate the resulting current density map of Staten Island from Circuitscape using deer occurrence data from across Staten Island. To do this, I will use **Statsmodels** to run a t-test to compare mean current density values at deer occurrence locations versus random locations. If the resistance surface accurately represents functional connectivity for deer then the current densities at deer locations will be higher than at random locations. 

**3.)** I will use the **Requests** http library for Python to web scrape for white-tailed deer occurrence data on the aforementioned websites. 

**4.)** I will use the landscape generator software, **NLMpy**, to simulate landscapes with classed resistance values that reflect the validated map from Staten Island and which include movement barriers of interest (roads, urban centers, riverways). 

**5.)** I will simulate arrays of data that reflect the distribution of deer occurrences using a deterministic process of dispersal to run on the artificial landscape to understand how the landscape affects colonization probability and movement patterns. 

### **The novelty:**
There are few papers documenting resistance values for white-tailed deer and none that I have seen that validate these values with telemetry or occurernce data. 

### **Short-Term Goals:** 
* Parameterize a resistance surface of Staten Island using deer occurrence and telemetry data.
* Assess the reliability of extrapolating the resistance surface values from Staten Island more broadly to landscapes in surrounding northeast states. 

### **Long-Term Goals:** 
* Simulate deer dispersal across artificial landscapes.
* Determine deer colonization probability and barriers to movement.
* Display simulations of deer dispersal using the dash visualization tool on my computer. 
* Allow for simulations to run on our lab website. 

