# Deep Operator Learning

A talk for the Seminar "Scientific Machine Learning" \
Hosted by Tobias Buck at Ruprecht Karls Universität Heidelberg

### Content
In this repo you will find:
- The [slides](Slides-talk-27-11-2023.ppsx) of the talk, held on the 27th of November 2023
- The code presented to the audience as a test case. Specifically: 
   - [Test case 1](Heat_forcing-term-1D/Heat_forcing-term-1D.ipynb):  Learning the operator from the forcing term <span style="color:red"> **u(x)** </span> to the solution s(x,t) for the heat equation
   - [Test case 2](Heat_forcing-term-2D/Heat_forcing-term-2D.ipynb): Learning the operator from the forcing term <span style="color:red"> **u(x,t)** </span> to the solution s(x,t) for the heat equation
- A detailed [report](Report.pdf) on the study of the subject 

### Instructions to run the code
0. Clone the repository
1. Initialize submodules deepxde, deepxde_v0.11.2

        git submodule init
        git submodule update


2. Run the desired notebooks: [Test case 1](Heat_forcing-term-1D/Heat_forcing-term-1D.ipynb) and [Test case 2](Heat_forcing-term-2D/Heat_forcing-term-2D.ipynb)

Notes:
- Verify that deepxde_v0.11.2 is checked out at branch "v_0_11_2" and not "master"
- I'm totally aware of the lack of professionality in using two versions of the same library, but, as explained in section "Code" of the report, this code has only didactic purposes. It was chosen as best course of action to load some functions from the last realease of deepxde and some from the earlier one. It's unfortunately not possible to initialize two submodules of the same library at two different commits, therefore one is a fork.