# Data Science Project 

Run the following command once in the git repo directory:

`git config filter.strip-notebook-output.clean 'jupyter-nbconvert --ClearOutputPreprocessor.enabled=True --to=notebook --stdin --stdout --log-level=ERROR'`

This removes the jupyter output in every commit and ensures that there are fewer conflicts. Otherwise, every run of jupyter will create outputs that create hard to resolve conflicts. The command works on Mac, on Linux or Windows the `jupyter-nbconvert` might be different.
