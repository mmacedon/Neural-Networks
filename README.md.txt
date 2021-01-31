Neural Networks Traffic Signal Categorization:

	The logical first step in this assignment was to gather all the images and convert them to the proper format to input into the neural network.
Using the python OpenCV2 library, the imread() function first reads the data as BGR format. The cvtColor() function converts the image from BGR to RGB format.
Next, the resize function is called to size the images to the required IMGWIDTH and IMGHEIGHT to input into the network. After the image and the appropriate label was added
to an image and label list. This tuple of lists was returned to be split into an appropriate training and evaluating set.

	The next step was building the network. The first network built was the one found in the lecture material to get an idea of how a network as actually constructed.
Running the data under this input resulted in high loss and low accuracy since this network was not designed for this specific scenario. The test results are as follows:
	Trial 1:
		333/333 - 1s - loss: 3.4894 - accuracy: 0.0558
		Max Loss: 12.5081 at Epoch 1	Max Accuracy: 0.0588 at Epoch 3
		Min Loss: 3.023 at Epoch 9 	Min Accuracy: 0.0525 at Epoch 1

The second trial consisted of a new hidden layer within the network.
	Trial 2:
