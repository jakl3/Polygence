There are three files in this folder:

Note - if you want to run the notebooks, you may have to change the data file directory to wherever your OASIS csv data is placed.

1. lagrangian svm.ipynb
	- This is the main file that I showed during the meeting.
	- It has the Lagrangian and the gradient descent optimization via hinge loss.
	- I'll mainly be updating this file as I begin implementing kernels and PCA
	
2. oasis_svm.ipynb
	- This is the svm that I did based on the video guide from sentdex.
	- Because he used transformations, it's extremely time consuming as dimensions increase
		- In 2d, there's only 4 possible transformations.
		- With mine, even when I reduce the dimensions to 10, there is 1033 possible transformations.
	- When removing transformations to allow it to run in time, it has very low accuracy (around 40 to 50%, at most)
	- I haven't been able to run it with transformations included due to how much time it takes. In two hours of running, it completed half of the first step, and there is three steps, so it would take probably around twelve hours, which simply isn't feasible when the lagrangian one only takes a few minutes at most.
	
3. svm_from_scratch_linear.ipynb
	- This was the first test file I created when I played around with SVM, creating the model purely based on random weights and biases as suggested in your google doc. You can look at it if you want, but I don't think there's really anything interesting there since it's all random.
		
