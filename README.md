# data_science_blog_post_udacity
Analysis of Stackoverflow developer survey 2019

Blog post:
https://medium.com/@robertanderson1993/can-development-practices-influence-developers-job-satisfaction-74841cc5cffb

## Installation

Tested on Python 3.7

To install dependencies and run:

```sh
python -m venv env

source env/bin/activate

pip install -r requirements.txt

./tools/extract_data.sh

jupyter notebook
```

## Libraries used

* Matplotlib
* NumPy
* pandas
* scikit-learn
* SciPy

## Project motivation

At my current organisation all of the Python code I write is unit tested, and must be reviewed by at least one other member of the development team before that code can be merged into any repository.

Despite this process initially being difficult to adapt to, the first time I had to refactor a large part of a service, the unit tests gave me confidence that my changes weren't going to affect the end user negatively.

Having my code reviewed, and reviewing other developers' code takes up time; but means developers often have a better idea of what their colleagues are working on, and ensures that all code being merged into a codebase is of a good standard.

This has (I believe) contributed to my satisfaction with my current organisation.

I wanted to analyse a recent StackOverflow developer survey to see if other developers were more satisfied with their jobs when they wrote unit tests and reviewed peers' code as part of their jobs.

## Analysis outcomes

Unfortunately, having done some analysis on the results of StackOverflow's developer survey from 2019, the main takeaways were that writing unit tests and spending time reviewing colleagues' code didn't have a strong correlation with developer job satisfaction, and that developer salary had a much larger influence on satisfaction.

Still, a negative result is still a result, and I enjoyed trying to gain some insight into developer satisfaction in this dataset.

## Files included

### development_job_satisfaction.ipynb
* The final notebook that performs any analysis used in the blog post
* Based on initial exploratory analysis performed with the notebooks in `src/`

### data.tar.xz
* The compressed dataset
* Decompress using the script in `tools/`

### requirements.txt
* Libraries to install using pip to run the notebook and analysis
