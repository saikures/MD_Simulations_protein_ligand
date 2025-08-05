GROMACS MD Protein Simulation on Google Colab

This repository contains a Jupyter notebook for performing Molecular Dynamics (MD) protein simulations using the GROMACS software. The notebook is specifically configured to run on Google Colab, leveraging its GPU resources for faster computation. It also provides instructions for using the notebook for terminal-based runs.

The primary goal of this notebook is to provide a reproducible and accessible environment for learning and performing GROMACS simulations without the need for a local high-performance computing setup.
Key Features

    GROMACS Installation: The notebook includes a script to download and compile GROMACS from source. It also handles the installation of necessary dependencies like CMake.

    Google Colab Integration: The notebook is designed to run seamlessly in Google Colab, with specific instructions for enabling GPU support and mounting Google Drive for data persistence.

    Terminal Commands: All simulation steps are executed using %%bash magic commands, making the notebook also useful as a reference for running GROMACS from a terminal.

    Customizable: Users can easily change the PDB ID to simulate different proteins or use their own data from Google Drive.

    Resource Check: A cell is included to check the available system resources (CPU, GPU, RAM) on the Colab instance.

Limitations and Important Notes

    Session Resets: Google Colab's free tier has a session limit. Data and installations are reset every 12 hours. Users must restart the notebook from the beginning after a session ends.

    Data Persistence: It is crucial to use Google Drive for storing any important data, as the temporary Colab environment is not persistent. The notebook includes a cell to mount Google Drive.

    GROMACS Version: The notebook is configured to use a specific version of CMake (e.g., 3.20.0-rc1) for a particular version of GROMACS (e.g., 2021). If you are using a different version, you may need to adjust the download and compilation steps.

How to Use

    Open in Google Colab: Upload and open the saikures_gromacs_runs_analyses.ipynb notebook in Google Colab.

    Enable GPU: Go to Runtime -> Change Runtime Type and select GPU as the Hardware Accelerator.

    Mount Google Drive: Run the cell to mount your Google Drive to /content/drive.

    Execute Cells: Follow the notebook by running each cell sequentially. The cells will guide you through:

        Checking system resources.

        Downloading and compiling GROMACS.

        Downloading a protein structure from the PDB.

        Running the various GROMACS commands for energy minimization, NVT, and NPT simulations.

        Analyzing the simulation results.

    Change PDB ID: To simulate a different protein, simply change the PDB ID in the relevant cell.
