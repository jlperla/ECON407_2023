# ECON407 Spring 2023
This is a trial of the new course [**ECON 408: Computational Methods in Macroeconomics**](syllabus.md), temporarily using the ECON 407 course code.

**(3 credits course)** Computational tools used in macroeconomics and financial economics including applications to unemployment, inequality, asset pricing, and economic growth

**Prerequisites:** One of ECON 301, ECON 304, ECON 308 and one of ECON 323, CPSC 103, CPSC 110, MATH 210, COMM 337 and one of MATH 221, MATH 223.

Note that unlike the listed ECON407, it is not mandatory to have ECON302 and ECON303 - but the programming and linear algebra requirements are essential.

But don't be scared off by the programming requirement!  Relative to many classes, the coding will be kept simple - just beyond the level of Stata/R.  The hard part will be the economic theory.

## Course Materials
- Consider selecting `Watch` at the top of this repository to be alerted to all file changes
- Since you will need to setup VS Code on your computer, you may find it easiest to clone this repository using [VS Code](https://docs.microsoft.com/en-us/azure/developer/javascript/how-to/with-visual-studio-code/clone-github-repository?tabs=create-repo-command-palette%2Cinitialize-repo-activity-bar%2Ccreate-branch-command-palette%2Ccommit-changes-command-palette%2Cpush-command-palette) directly.
- I strongly suggest signing up for GitHub's [student developer pack](https://education.github.com/pack) which gives you lots of free stuff (and even access to the AI [GitHub Copilot](https://docs.github.com/en/copilot/quickstart) )

## Syllabus
See [here](syllabus.md) for more details

## Problem Sets and Exams
1. **Due Midnight PST on January 15th** - [Problem Set 0](/problem_sets/problem_set_0.pdf). Basically just setup and a trivial notebook.
2. **Due Midnight PST on January 29th** - [Problem Set 1](/problem_sets/problem_set_1.ipynb). Variations on the Geometric Series Code and some simulations.
3. **Due Midnight PST on February 7th** - [Problem Set 2](/problem_sets/problem_set_2.ipynb)
4. **Due Midnight PST on February 14th** - [Problem Set 3](/problem_sets/problem_set_3.ipynb)
5. [Midterm Practice Problems](/problem_sets/midterm_practice_problems.ipynb)
6. **February 27th:**  MIDTERM EXAM

Note that the midterm is the day after spring-break and cannot be moved as it requires booking a computer lab.  Travel schedules are not a valid excuse for missing the midterm.

Problem sets that involve code are submitted on Canvasby the deadline:
1. Submit a **both** the **executed** Jupyter notebook (`.ipynb`) and a rendered HTML or PDF file.
   - To save as HTML or PDF, you can use the `File` menu in Jupyter Lab or choose `Export` for the built-in VS Code.
  
3. Problem sets that are a mixture of code and theory should be submitted as a combined PDF with both.
   - You do not need to type your equations in latex, but you should make the handwritten equations clear.
4. Make sure to put your name on the ipynb and pdf/html files so that we can keep track of them if we download all students in the same directly.
     - For the naming convention: "FIRST_LAST_ASSIGNMENT_0.ipynb` or something like that works best

## Lectures
The first few weeks will introduce Julia, and then we will move on to the core topics of the course which will be a combination of theory and computational examples.
1. **January 9th** - Introduction, course overview, VSCode and [Julia Overview](https://julia.quantecon.org/getting_started_julia/getting_started.html) and start of [Introductory Examples](https://julia.quantecon.org/getting_started_julia/julia_by_example.html)
2. **January 11th** - [Introductory examples/fixed point problems](https://julia.quantecon.org/getting_started_julia/julia_by_example.html) including examples from linear-asset pricing
3. **January 16th** - Finish [Introductory Examples](https://julia.quantecon.org/getting_started_julia/julia_by_example.html) with some in [Essentials](https://julia.quantecon.org/getting_started_julia/julia_essentials.html) and [Fundamental Types](https://julia.quantecon.org/getting_started_julia/fundamental_types.html)
4. **January 18th** - Finish off remainder of Julia overview and move to [Geometric Series/Money Multiplier Model](https://julia.quantecon.org/tools_and_techniques/geom_series.html).
   - Optional: [Application to Asset Pricing](https://julia.quantecon.org/tools_and_techniques/geom_series.html#application-to-asset-pricing) in detail.  The basic results near the beginning are essential, though.
5. **January 23rd** - Finish [Geometric Series/Money Multiplier Model](https://julia.quantecon.org/tools_and_techniques/geom_series.html), a little more on fixed-points, and start [Dynamics in One Dimension](https://julia.quantecon.org/introduction_dynamics/scalar_dynam.html)
   - Optional: [math on stability analysis](https://julia.quantecon.org/introduction_dynamics/scalar_dynam.html#stability) details
6. **January 25th** - FInished [Dynamics in One Dimension](https://julia.quantecon.org/introduction_dynamics/scalar_dynam.html) and started [AR1 Processes](https://julia.quantecon.org/introduction_dynamics/ar1_processes.html)
   - Optional: [ergodicity](https://julia.quantecon.org/introduction_dynamics/ar1_processes.html#ergodicity) details and formal derivations on [stationarity](https://julia.quantecon.org/introduction_dynamics/ar1_processes.html#stationary-distributions)
7. **January 30th** -  [AR1 Processes](https://julia.quantecon.org/introduction_dynamics/ar1_processes.html) and [Wealth Distribution Dynamics](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html)
    - Optional: [in-place functions and performance](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html#in-place-functions-preallocation-and-performance) and other performance tips on [parallelization](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html#parallelization-and-vectorization)
    - Optional: [detailed interpretation of the wealth process](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html#a-model-of-wealth-dynamics) since this is just one example.  Understand it mechanically, but no need to analyze every term carefully.  This is just one of many ways you could write a joint process of wealth and income.
8. **February 1st** - [Wealth Distribution Dynamics](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html)
9.  **February 6th** - Finish [Wealth Distribution Dynamics](https://julia.quantecon.org/introduction_dynamics/wealth_dynamics.html) and start [Linear State Space Models](https://julia.quantecon.org/introduction_dynamics/linear_models.html)
10. **February 8th** - [Linear State Space Models](https://julia.quantecon.org/introduction_dynamics/linear_models.html)
    - Optional: [derivations for the evolution of the moments beyond simple forecasting](https://julia.quantecon.org/introduction_dynamics/linear_models.html#distributions-and-moments) 
    - Optional: [detailed derivation of the ensembles](https://julia.quantecon.org/introduction_dynamics/linear_models.html#ensemble-interpretations), though the concept is essential.
    - Optional: [detailed derivations of ergodicity and stability](https://julia.quantecon.org/introduction_dynamics/linear_models.html#stationarity-and-ergodicity), though the concept is essential.
12. **February 13th** - Review problem sets 1 and 2
13. **February 15th** - Review problem set 3 and some of the extra problems ([Midterm Practice Problems](/problem_sets/midterm_practice_problems.ipynb))
14. **February 20th** - BREAK
15. **February 22nd** - BREAK
16. **February 27th** - **MIDTERM EXAM** class time
17. **March 1st** - [The Permanent Income Model](https://julia.quantecon.org/dynamic_programming/perm_income.html)
18. **March 6th** - 
19. **March 8th** -
20. **March 13th** -
21. **March 15th** -
22. **March 20th** -
23. **March 22nd** -
24. **March 27th** -
25. **March 29th** -
26. **April 3rd** -
27. **April 5th** -
28. **April 10th** -
29. **April 12th** -
