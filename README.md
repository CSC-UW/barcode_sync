# random_barcode_sync
Use random sync pulses to map times from recording to another

## Usage
You can create a new conda environment from the command line (reccomended):
```
conda env create --file environment.yaml # Create a new environment
jupyter lab # Then, start Jupyter Lab 
```
Alternatively, you can also try to update an existing environment:
```
conda activate myenv
conda env update --file environment.yaml
```
If you need maximally precise timing information, use SpikeGLX's AP binary file. The LFP binary works just fine and loads a lot faster, but rising edge times can have up to 400 usec uncertainty, vs. ~33 usec when using the AP file. 
