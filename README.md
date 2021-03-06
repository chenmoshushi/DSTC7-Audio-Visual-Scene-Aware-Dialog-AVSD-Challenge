Dialog System Technology Challenges 7 (DSTC7) Track 3: Sentence generation task

# Audio Visual Scene-Aware Dialog (AVSD)
Data collection description paper: Please cite this paper if you will use the shared data sets.
   
      @inproceedings{alamri2019audiovisual,
                  title={Audio-Visual Scene-Aware Dialog},
                  author={Huda Alamri and Vincent Cartillier and Abhishek Das and Jue Wang and Stefan Lee and Peter Anderson                    and Irfan Essa and Devi Parikh and Dhruv Batra and Anoop Cherian and Tim K. Marks and Chiori Hori},
                  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
                  year={2019}
      }
      
# AVSD sentence generation task for DSTC7 Challenge

AVSD@DSTC7 Challenge decription paper:
http://workshop.colips.org/dstc7/papers/DSTC7_Task_3_overview_paper.pdf

Data set for settence generation: 
https://drive.google.com/drive/folders/1SlZTySJAk_2tiMG5F8ivxCfOl_OWwd_Q?usp=sharing      
      
## News:

### - Data will be publicly available: April. 1st, 2019

You can donwload the full oficial data set and the refereces for AVSD@DSTC7 from here:
https://drive.google.com/drive/folders/1SlZTySJAk_2tiMG5F8ivxCfOl_OWwd_Q?usp=sharing

### - New submission deadline: Oct. 15th

The official submission site had problems to upload files.
The problems were fixed now. 
Let us extend the submission deadline to * Oct. 15th *

### - Submission site  
Now the submission site is open. 

      The data format is the same as test_set4DSTC7-AVSD.json.
      Please replace __UNDISCLOSED__ with your generated answers.

https://docs.google.com/forms/d/e/1FAIpQLSd5DssD8hjrLI77oUPijVheX8RQTJGjXJYH78UJF2Le-lxXLw/viewform

### - New baseline system 
Please go to the following link to get the new baseline system:
https://github.com/dialogtekgeek/AudioVisualSceneAwareDialog            

### - Data use policy
      1. Registrant will submit system results and system description papers: 
         Publish results anywhere as DSTC7 participants
         
      2. Registrant will not submit results or system description papers:
         Please wait using the data until it will be publicly available
         
      3. Others:
         Currently, you cannot access the data.
         Please wait until the data will be open.

### - Official data set is released
  *DSTC7 is ongoing and the data is not publicly available now.
    
  The data format of the output should be the same as the given test set file in the shared directory:
  
      train_set4DSTC7-AVSD.json
      val_set4DSTC7-AVSD.json
      test_set4DSTC7-AVSD.json
  
  The original videos of the test sets of the official Charades Challenge
  
      http://ai2-website.s3.amazonaws.com/data/Charades_vu17_test.tar
   
  Please fill your answers into `__UNDISCLOSED__`  below:

      -----------------------------------------------------------------------------------------------------------
      "dialog" : [
                  {
                     "answer" : "no and it is a window that he is standing in front of .",
                     "question" : "hello . did someone come to the door ?"
                  },
                  {
                     "answer" : "__UNDISCLOSED__",
                     "question" : "is he looking at something outside the window ?"
                  }
               ]
      ----------------------------------------------------------------------------------------------------------

### - System submission deadline is changed.
      http://workshop.colips.org/dstc7/dates.html
      
      The submission can be done from Sep 24th to Oct 8th from the following link:
             Submission URL: Not open yet

### - Registration 
   Please register:  https://docs.google.com/forms/d/e/1FAIpQLSf4aoCdtLsnFr_AKfp3tnTy4OUCITy5avcEEpUHJ9oZ5ZFvbg/viewform  
   Please let us share the data with you using your registered e-mail.

### - Data release
   Video dat: CHARADES for human action recognition datasets.
   
   
   https://allenai.org/plato/charades/

   Prototype datasets: 6172(training), 732(validation), 733(test)
   *DSTC7 is ongoing and the data is not publicly available now.
  
   
         - text dataset: 10 QAs + 1 summary       
         - Audio features: VGGish 
         - Visual features: I3D 
          * You can use your own audio and visual features extracted using publicly available tools and models.
         
### - Baseline system release
      The system release is scheduled on July 20th
      *You can find a setup using the prototype data and the released audio and visual features: 
      https://arxiv.org/abs/1806.08409
      

## - Track Description
Welcome to the Audio Visual Scene-Aware Dialog (AVSD) challenge and dataset. This challenge is one track of  the **7th Dialog System Technology Challenges (DSTC7) workshop.**
The task is to build a system that generates responses in a dialog about an input video.

### - Tasks

In this challenge, the system must generate responses to a user input in the context of a given dialog.  
This context consists of a dialog history (previous utterances by both user and system) in addition to video and audio information that comprise the scene. 
The quality of a system’s automatically generated sentences is evaluated using objective measures to determine whether or not the generated responses are natural and informative.

#### 1. Task 1: Video and Text 
    a. Use the video and text training data provided but no external data sources, 
       other than publicly available pre-trained feature extraction models.

       There are two options: with or without using the summary generated by the questioners after holding 10 QAs.

    b. External data may also be used for training.

#### 2. Task 2: Text Only 
    a. Do not use the input videos for training or testing. 
       Use only the text training data (dialogs and video descriptions) provided. 
    b. Any publicly available text data may also be used for training.

### - Dataset
#### Proto type data set:

|               |   Training    |  Validation   |     Test      |
| ------------- | ------------- | ------------- | ------------- |
| # of Dialogs  |     6172      |      732      |      733      |
| # of Turns    |    123,480    |     14,680    |     14,660    |
| # of Words    |    1,163,969  |    138,314    |    138,790    |

      The training data is part of the training data.
      The validation data is half of the officila validation data.
      The test data is the rest of the official validation data.

#### Official data set:
The number of tunrs for the test set is smaller than the validation
because they are not always full dialogs.

|               |    Training    |  Validation   |     Test      |
| ------------- | -------------- | ------------- | ------------- |
| # of Dialogs  |       7,659    |      1,787    |      1,710    |   
| # of Turns    |     153,180    |     35,740    |     13,490    |
| # of Words    |   1,450,754    |    339,006    |    110,252    |


### - Contact Information

halamri3@gatech.edu & chori@merl.com
