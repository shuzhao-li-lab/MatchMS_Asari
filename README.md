About
=====

This is a repo with submodules of MatchMS and SparseStack with patches that will enable install under Python3.13. This is not maintained by MatchMS developers. The current version of MatchMS does not install on Python3.13; however, this seems to be largely due to Poetry enforcing specific versions of packages that no longer work on 3.13, mainly numba. This repo will let you install MatchMS v0.28.2 on Python3.13.

This package is not actively maintained, this was just for testing but posted here for re-use. Please do not contact the maintainers of MatchMS for problems with this version. 

** NOTE: It is not tested. The only changes involve package versions, so the results are likely unchanged, but no guarentees are made about the correctness of these changes. **

Install
=======

1. Clone this repo to your local machine
2. Load python virtual environment (optional)
3. Replace their pyproject.toml files with the ones in the repository. Be sure to rename them to pyproject.toml inside each source dir. 
4. Install sparsestack using `pip3 install .` while in the sparsestack directory
5. Install matchms using `pip3 install .` while in the matchms directory
6. Run `import matchms` in the interpreter to verify install.

Tested on OS X.

Citations
=========

If you do use this, please cite: 

F Huber, S. Verhoeven, C. Meijer, H. Spreeuw, E. M. Villanueva Castilla, C. Geng, J.J.J. van der Hooft, S. Rogers, A. Belloum, F. Diblen, J.H. Spaaks, (2020). matchms - processing and similarity evaluation of mass spectrometry data. Journal of Open Source Software, 5(52), 2411, https://doi.org/10.21105/joss.02411

de Jonge NF, Hecht H, Michael Strobel, Mingxun Wang, van der Hooft JJJ, Huber F. (2024). Reproducible MS/MS library cleaning pipeline in matchms. Journal of Cheminformatics, 2024, https://jcheminf.biomedcentral.com/articles/10.1186/s13321-024-00878-1

Here are links to the main repos, you should look here for updates as they are actively developed. 

MatchMS:

https://github.com/matchms/matchms

Sparsestack:

https://github.com/matchms/sparsestack