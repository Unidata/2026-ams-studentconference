# Exploring Meteorological Datasets with NSF Unidata AWIPS & MetPy

AMS Annual Meeting Student Conference Workshop

### ⌨ Getting set up

For synchronous workshop learners, we have two separate ways you can participate, work ahead, and follow along.
During the workshop, you will be given access to NSF Unidata's Science Gateway to do your work on NSF's Jetstream Cloud.
If you prefer or require doing the work with your offline environment, please do.

#### ☁️ Using the [NSF Unidata Science Gateway](https://science-gateway.unidata.ucar.edu/) cloud environment

During the AMS Annual Meeting, you can do all of this work on our very own _gateway_ to the NSF Jetstream Cloud!
You have received instructions from NSF Unidata on how to access Science Gateway.
After you are given access, you can sign in to Science Gateway with at [pyaos-workshop.unidata.ucar.edu](https://pyaos-workshop.unidata.ucar.edu "Access the NSF Unidata JupyterHub").

When you first sign in, it may take a few seconds for your personal workspace to populate and your coding environment to be fully set up.
From here you will discover a Jupyter Lab interface pre-populated with these materials and a few tools to enable you to update the materials if needed.
Once you are given access, you will be able to download materials and notebooks from your workspace if you'd like/

#### 💻 Using your own offline environment

**Note that we at NSF Unidata are not able to plan for any hardware limitations your personal computer might have, and we will not have time during the workshop to diagnose issues on personal computers.**
Please plan to use Science Gateway if this is a concern for you.
We will be using and supporting [Conda](https://docs.conda.io/en/latest/ "Conda documentation") for installing and managing a Python environment from your computer's command line.
Please have this environment prepared ahead of time if you'll be using your own computer.

> 1. [Install Miniforge](https://github.com/conda-forge/miniforge?tab=readme-ov-file#miniforge "Miniforge download and installation page") if you don't already have command-line access to `conda`.
> 1. Get a copy of this code!
>    You have a few options from the green button above,  
>    a. `git clone https://github.com/Unidata/2026-ams-studentconference.git` from your command line, within some directory on your computer.
>    [Install git](https://github.com/git-guides/install-git "Git download and installation page") if necessary.
>    If you're comfortable with `git`, we recommend this approach as it will let you keep this code regularly up to date.  
>    b. [`Open with GitHub Desktop`](https://desktop.github.com/ "GitHub Desktop app download page") if you have and prefer this graphically-focused software.  
>    c. [`Download ZIP`](<(https://github.com/unidata/2026-ams-studentconference/releases/refs/heads/main.zip)> "Download link for these course materials") if you prefer to get a single snapshot of the code right here and now.
> 1. Wherever you have this code saved, set up your Python environment with `conda env create -f environment.yml` from your command line.
> 1. Give this some time.
>    Once it's done, activate this new environment with `conda activate 2026-ams-studentconference`.
>    Always do this before starting on work for this workshop!
> 1. Launch Jupyter and get to coding with `jupyter lab`.
>    Don't forget to activate your environment first!

### 💬 Acknowledgements

The JupyterHub for this workshop is part of the [U.S. National Science Foundation](https://www.nsf.gov/ "U.S. National Science Foundation homepage") funded [NSF Unidata Science Gateway](https://doi.org/10.5065/688s-2w73 "NSF Unidata Science Gateway permalink") (doi:10.5065/688s-2w73) (under NSF Award [1901712](https://www.nsf.gov/awardsearch/showAward?AWD_ID=1901712)).
We thank Andrea Zonca (San Diego Supercomputing Center), Jeremy Fischer (Indiana University), the NSF funded [Jetstream](https://dx.doi.org/10.1145/2792745.2792774) team, and the NSF funded XSEDE [Extended Collaborative Support Service](https://doi.org/10.1007/978-3-319-32243-8_1) (ECSS) program for assistance with this JupyterHub.

### 📖 License

Code and content are licensed together under **both** the MIT license [1] and the CC0 1.0 Universal license [2]:

- [1]: [LICENSE.MIT](LICENSE.MIT) or <https://opensource.org/license/mit>
- [2]: [LICENSE.CC0-1.0](LICENSE.CC0-1.0) or <https://creativecommons.org/publicdomain/zero/1.0/>

`SPDX-License-Identifier: MIT AND CC0-1.0`
