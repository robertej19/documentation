# Sample Results

Please find green checkmark at https://github.com/mit-mc-clas12/clas12simulations/commits/master
This means that the travis build was successful at the commit.
If you click the detail, you will get a feel for what business travis exactly does.

# What is Travis

- Automatic sanity check tool for each commit with  to run a sanity check everytime we make commit by running scripts at travis environment equipped with almost every version of languages including python
- installing custom files via git, setup.py, wget, .. also possible
- custom sanity check tool like pytest, coverage also supported
- bitbucket often used as a counterpart of github provides built-in integrity check tool called pipeline.

# How to start travis?

- A guide from travis--https://docs.travis-ci.com/user/tutorial/ is well-documented.
- Check a permission of travis granted to the targeted repo
- What is needed to be done is to edit .travis.yml. The minimum scripts go like below.
```
language: python
python:
  - "2.6"
  - "2.7"
# command to run tests
script:
  - python2 test.py
```
- Of course, .travis.yml can be complex as much as needed. Samples are at (https://docs.travis-ci.com/user/languages/python/#examples)
