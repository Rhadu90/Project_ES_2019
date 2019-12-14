# Project_ES_2019

Pre-conditions:
  Sniper installed -> follow the HowTo

Setting up the project:
  1. Create a new folder in Home called bin
  2. Copy the benchmarks_auto bash script in the new folder
  3. Update fix paths in the script to match your folder structure (e.g. "/home/rhadu/sniper/benchmarks/results/"$benchmark"/"$((cores))"/sim.out" 
  
Execution:
  1. cd bin
  2. make
  3. benchmarks_auto -b fft -n 4
  Where "-b" represents the option that the next argument is the type of benchmark we want to execute. We will run fft or barnes benchmarks. "-n" represents the option of how many cores we want to run the benchmarks on
  
Note:
  1. "/home/rhadu/sniper/benchmarks/results/..." new folders will be generated where the results of the executed benchmarks will be stored. Look for the file called sim.out
  2. In the "bin" folder a .csv file will be created containing the name of the benchmak and the number of cores for each execution. In this file we will store all the sim.out results and draw the graphics
  
