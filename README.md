# random_barcode_sync
Use random sync pulses to map times from recording to another

## Usage
You can create a new conda environment from Cmder:
```
conda env create --file environment.yaml # Create a new environment
conda activate barcode_sync # Activate your new environment
jupyter lab # Start Jupyter Lab
```

The next time that you need to use the notebook, just open Cmder, activate your environment, and start Jupyterlab:
```
# Run these from Cmder
conda activate barcode_sync
jupyter lab
```

If you need maximally precise timing information, use SpikeGLX's AP binary file. The LFP binary works just fine and loads a lot faster, but rising edge times can have up to 400 usec uncertainty, vs. ~33 usec when using the AP file.
