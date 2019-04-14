### Homework
* Don't forget to fill up the Weekly Journal! 

##### Basic
1. Create a new repository called `docker-homework`, and in it, put the following:
  - LICENSE
  - README.md
  - Dockerfile
  - the `csvparser` from class 3
  - the data file from class 3
When “built”, the `Dockerfile` should install python3, contain your python script from last class, and set it up to run the script as soon as the container is turned on. To help with this, look up `Docker` + (`ADD`, `COPY`, `CMD`, `ENTRYPOINT`, and `volume mounting`). The container should either contain the data file, or use volume mounting to find it.
The `README.md` should contain instructions for A) building, B) showing us that it exists/when it was made, and C) running your Dockerfile.
2. Research “Continuous Integration” and write a short summary in your `README.md` that summarizes it and mentions one tool that you can use for it with GitHub.
3. Read the “Docker getting started guide” (this will help with 1. !!!)

##### Advanced
1. Adjust your homework from last week (parts 1 and 5) to work on the dataset your selected for your project. This means you should either a) have two scripts, one for part of number 1 and one for this, or b) refactor your script to be more “general” and accept the path to a file as input (this can be accomplished with the `argparse` library. You can also use libraries now, such as `numpy`, `pandas`, and `csv`. 

##### Reach
1. Extend the script you have created for your own dataset to compute the a) mean and b) standard deviation of each feature in your dataset. 
