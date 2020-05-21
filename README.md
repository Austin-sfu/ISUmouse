# ISUmouse

This is the "ISUmouse" dataset. 

Originally collected by the Kinesiology Department of Iowa State University.

Data was collected through an online game programmed in Javascript, embedded in a Qualtrics survey and running in Windows 10 environment. In the game subjects were asked to perform a predefined mouse task (denoted as one trial) which includes 10 consecutive movements in a pattern illustrated in figure "game_of_one_trial.pdf". Subjects are instructed by the following rules:
	(1)Use the mouse to move the cursor to the green target as quickly as possible.
	(2)Left click once the cursor is inside the green target before the target disappears. 
	(3)After clicking on the green target, the next target will appear.
	(4)Stay inside the green target until you see the next target. Click ONLY when you are inside the green target.
	(5)Always keep the mouse in constant contact with the surface. 
	(6)Simply continue this in the same manner until the pattern stops.

This dataset is generally used for individuals' mouse operation behavior study

# How to Access
As our data collection experiments were approved by IRB, we are not able to directly release the dataset to public. 
However, if you want to use this dataset for research proposes, you can contact the authors to get permission and get access to it. More specifically, please answer the questions in "Access_Request_Form.docx" and send it to the email addresses in the "Contact" section below.


# Data layout:
	Each folder under "./data/" directory is the collection of a subject. E.g. "N606"
		Within each subject's raw data folder, e.g. "./data/N606/RawData/", each trial of this user is collected in one .txt file, named by the index of this trial.
			In each .txt file, there are 4 columns: 
				(1) current mouse state: Enumerated integer from {512, 513, 514}. 
					512: indicate there is no mouse click event. (basically just moving the mouse)
					513: indicate there is a left-key press event.
					514: indicate there is a left-key release event.
				(2) x position: The x-position of the mouse cursor on the screen. In pixels (float).
				(3) y position: The x-position of the mouse cursor on the screen. In pixels (float).
				(4) timestamp: The time the current mouse point was sampled. In milliseconds (integer).

# Citation
If you are using the data in your publication, please cite it as follows:

The Kinesiology Department of Iowa State University (2018). ISUmouse dataset. Available at: https://github.com/Austin-sfu/ISUmouse.git

# Contact
If you wish to contact the authors you may reach them through the either of the following email addresses:
dqin@iastate.edu 
or
shenfu@iastate.edu
