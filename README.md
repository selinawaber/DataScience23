# Data Science Project 

Make sure that `jupyter-nbconvert` is installed [https://nbconvert.readthedocs.io/en/latest/usage.html](https://nbconvert.readthedocs.io/en/latest/usage.html)

Then (on Mac) run the following command once in the git repo directory:

`git config filter.strip-notebook-output.clean 'jupyter-nbconvert --ClearOutputPreprocessor.enabled=True --to=notebook --stdin --stdout --log-level=ERROR'`

On Linux or Windows, the following command should work instead (not tested):

`git config filter.strip-notebook-output.clean 'jupyter nbconvert --ClearOutputPreprocessor.enabled=True --to=notebook --stdin --stdout --log-level=ERROR'`

This removes the jupyter output in every commit and ensures that there are fewer conflicts. Otherwise, every run of jupyter will create outputs that create hard to resolve conflicts.
