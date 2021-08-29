# 2021-benchmarking-workshop

Materials for the 2021 OpenFF benchmarking workshop.

## Installation and getting started

1. Clone the repository:

```
git clone git@github.com:openforcefield/2021-benchmarking-workshop.git
cd 2021-benchmarking-workshop
```

2. Install and activate the conda environment:

```
conda env create -f env.yml
conda activate 2021-benchmarking-workshop
```

3. Start up the jupyter notebook with:

```
jupyter notebook workshop.ipynb

```

### Using a remote environment

If you performed the installation instructions above on a remote host accessible via SSH,
you can connect to the Jupyter notebook server through an SSH tunnel.

Among the notebook server output from the instructions above, you should see a line like:

```
[I 17:17:45.169 NotebookApp] http://localhost:<port>/?token=<token-content>
```

You will need this for the below instructions.

1. Open a terminal on your local host, and run the following, noting `<port>` from the server output above:

    ssh -N -L 8801:localhost:<port> <remote-host>

2. In a web browser on your local host, enter the following in the URL bar

    localhost:8801

3. Copy the token from the terminal running the server.
   It should be among the output like that given above, where `<token-content>` is shown.
   Enter this into the prompt for the token to access the notebook.
