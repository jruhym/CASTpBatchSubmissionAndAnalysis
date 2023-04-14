# CASTpBatchSubmissionAndAnalysis
Batch submission of models to and reaping of resulting data from [CASTp](http://sts.bioe.uic.edu/castp/index.html) web server.

Requires [SeleniumIDE](https://www.selenium.dev/selenium-ide/)

CASTp, which allows you to calculate the binding-pocket volume of a protein from a structure file, does not have a batch submission option, downloadable code or an executable, or an API. I was interested in seeing how the volume of a pocket changes in time during a simulation. The first script allows me to submit many models to CASTp and save their submission Ids, which I use in the second script to download the results en masse. 

Note that this script is quite basic and will not prepare your data for you for submission. It has a basic loop so cut your data into single-MODEL PDB files and name them in alphanumeric succession.  

Note that there are pauses built into the scripts in order to play nice with CASTp's bandwidth. Please do *not* shorten these. So far I've done about 250 "models" at a time (a model from each ns of my quarter microsecond simulation). 
