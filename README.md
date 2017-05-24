# youtube-recommendation-link-prediction
Given a dataset of thousands of YouTube videos, their attributes and a set of 20 videos they each linked to, we had to determine if each set of two videos in the test data were linked. We managed to come 2nd in this “Kaggle in class” competition. We used the Python package NetworkX to graph the entire train set, assigned weighted directed edges from each movie to those it recommends, used PCA to weed out the unimportant features, mined the data using k-means to find sub-clusters and calculated the shortest path between test data records, and fine-tuned the model by modulating the sum of weighted arcs. The entire problem was parallelized using Python’s multiprocessing module over Amazon EC2 m4.16xlarge equipped with 64 cores.
