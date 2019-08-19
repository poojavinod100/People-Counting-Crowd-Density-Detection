# The Crowd Density Project 

This is a project at #sg_wonder_vision study group of the Facebook Secure and Private AI Scholarship Challenge 2019

****************************************************************************************************************************************
## PROJECT OBJECTIVE AND DESCRIPTION:
****************************************************************************************************************************************
-The main objective of this project is to build a self-sufficient software, that can accurately predict whether or not a stampede is imminent, based on the incoming live visuals of a place. 

-Often, huge footfall is associated with various popular festivals, religious ceremonies, public events, concerts etc. The enormous count of people coupled with their density(how close they are to each other) easily poses the risk of a normal crowd turning into a dangerous stampede that could potentially cost many lives. 

-This has happened several times in the past, especially at the world-famous Kumbh Mela(a festival where 30 million people take part in Allahabad, when the city can only hold about 9 million), and the recent tragedy at Elphinstone Railway station, Mumbai. 

-Most current stampede prevention solutions are reliant on hardware(footfall mats based on sensors etc), bringing along with it the question of capital investment, installation and maintenance costs and issues in the long run. 

-The key innovation we hope to create here is steer this project in the direction of a **completely software-based solution(based on Computer Vision Technology, that does not depend on inputs from any electronic hardware, which can be done using only the live CCTV visuals of the area we are monitoring)** for this problem, that can provide good levels of accuracy to accurately predict stampedes, so that some kind of intervention can be done at the right time to prevent such incidents in the future.
****************************************************************************************************************************************
## Team Members(Slack Handles):
________________________________________________________________________________________________________________________________________

@Pooja Vinod(Project Lead)

@Sreekanth Zipsy

@Viper

@Suraiya Khan

________________________________________________________________________________________________________________________________________

_See the exclusive website we have created for this project showcase
(Do make sure to go through all the sections, and please read the 'Concluding Notes' section to read about our thoughts on the future of this project)_: https://poojavinod100.wixsite.com/crowddensityproject

****************************************************************************************************************************************
## SUCCESSFUL IMPLEMENTATIONS:
****************************************************************************************************************************************

## 1. Visitor Counter for Events from overhead live visuals:

-Achieved using **OpenCV,Numpy,dlib,imutils and MobileNet-SSD model.**

-This is the implementation of a people counter to be used at doors of exhibitions/public events to count the net number of  visitors, inflow and outflow of people from a specific event. 

-Can be used to determine the most popular choice of events/performances/talks at concerts/festivals where multiple events happen simultaneously. 

-Can be used to determine popularity statistics for large-scale events(that have multiple sub-events) so they can plan accordindly for future editions. 

-The counts of visitors at different areas of a big venue, could further be used to detect crowded areas that are at risk of stampedes. This information could be used to take appropriate crowd control measures like crowd routing and redirection to avoid the possibility of stampedes.

-Apart from this, this kind of information coming from multiple cameras recording visuals of multiple areas of a venue, could be used to improve the crowd counting model to make accurate predictions about future crowd counts(and thus take precautionary measures), through **Federated Learning**.

-Output rate: 34 FPS

-**See output here**: https://drive.google.com/open?id=1xB9FA0hkU-ns3o5Zs4uCwAwZOY8uCWvA

-**See code in our repo**:

**_Related files and folders:_*

pyimagesearch

videos

people_counter.py

mobilenet_ssd

-**See SPAIC Medium blog written about implementation, by Pooja Vinod**: https://medium.com/secure-and-private-ai-writing-challenge/creating-a-direction-sensitive-people-counter-with-opencv-and-mobilenetssd-454627fe3c84

## 2. People Counter for Public Places(using to get live statics counts) from face-level visuals:

-Achieved using **DeepSort Algorithm, NumPy, sklean, OpenCV, Pillow and YOLOv3.**

-Can be used to get live counts of individuals from live cameras, that face incoming crowds. 

-Can be used to get dynamic stats of net number of people in a room/area at malls/public places at once, irrespective of which direction they are walking in. Counts coming from different regions can be used to update and constantly improve a crowd count predictor, using Federated Learning approach.

-Can be integrated with a decentralized approach to get live stats about crowds at different places at once.

-Output rate: 10 FPS

-**See output here**: https://drive.google.com/open?id=1h-XJTDbw_h-v3iaAf_z-1HXVkojOhRNL

-**See code in our repo**: See 'Crowd Counting & Tracking with Deep Sort & Yolo @ Sreekanth Zipsy' folder in 'Contributions' 

-**See SPAIC Medium blog written about implementation, by Sreekanth Zipsy**: https://medium.com/@sreekanthj244/udacitys-secure-private-ai-project-showcase-challenge-i-de38729ca530

## 3. CSRnet implementation on ShanghaiTech Dataset: Generating crowd counts from images-

-Achieved using **PyTorch, CUDA and CSRnet model on ShanghaiTech dataset.**

-Can provide impressively accurate counts of people from images alone

-Can be used for creation of crowd count predictors specific for various events and programmes, trained on counts generated from images alone(no need for live video capture). Past records of images taken at the venue can be used to predict future crowd counts to plan in advance for stampede prevention measures. 

-Would be especially useful at large scale religious festivals like the Kumbh Mela to accurately predict and prepare for crowds based on past images.

-Would be ideal to use with a Federated Learning Approach if image dataset is too large and spread across several machines.

-Would have comparively much less data storage requirements as images are being used, not space-consuming video archives. 

-**See output here**:https://drive.google.com/open?id=1h-XJTDbw_h-v3iaAf_z-1HXVkojOhRNL

-**See code in our repo**: See 'CSRNet @ Sreekanth Zipsy' folder in 'Contributions'

-**See SPAIC Medium blog written about implementation, by Sreekanth Zipsy**:

## 4. C3(Crowd Counting Code) Framework implementation on ShanghaiTech Dataset: Open Source Crowd Counting Framework using PyTorch

-Generates Gaussian Density Maps from images, detects and count crowds. 

-Reduces human cost in training

-**See code**: Link to repo included in 'Contributions' folder. 

-**See output**: At destination repo, please visit results_reports folder  for details of results obtained.

-**See SPAIC Medium blog written about implementation, by Pooja Vinod**: https://medium.com/secure-and-private-ai-writing-challenge/c3-crowd-counting-code-an-open-source-crowd-counting-framework-in-pytorch-b0a8b94036ba

________________________________________________________________________________________________________________________________________
## RESEARCH AND BLOG
(All below research-based articles have been published on the SPAIC Medium Publication)
________________________________________________________________________________________________________________________________________

## 1. Topic: The Wide Array of Use Cases where Crowd Density Detection can prove useful 

Author: Suraiya Khan

Read here:  https://medium.com/secure-and-private-ai-writing-challenge/crowd-counting-approaches-use-cases-and-importance-part-1-ad9c3cb12f13  

## 2. Topic: Exploring The Most Widely Used Datasets for Crowd Density Detection

Author: Ramkrishna Acharya

Read here: https://medium.com/@qrka/crowd-counting-made-easy-1bf84f18ff61

## 3. Topic: Summarizing The Crowd Density Project

Author: Pooja Vinod

Read here: https://medium.com/secure-and-private-ai-writing-challenge/concluding-notes-the-crowd-density-project-df22af5b3f6f

## 4. Topic: Crowd Counting with DeepSort and YOLO

Author: Sreekanth Zipsy

Read here: https://medium.com/@sreekanthj244/udacitys-secure-private-ai-project-showcase-challenge-i-de38729ca530

## 5. Topic: Crowd Counting on images with CSRnet

Author: Sreekanth Zipsy

Read here: https://medium.com/@sreekanthj244/implementation-of-csrnet-crowd-counting-project-for-udacity-project-showcase-a451b4397d71

## 6.Topic: Creating a net crowd counter with OpenCV and MobileNetSSD

Author: Pooja Vinod

Read here: https://medium.com/secure-and-private-ai-writing-challenge/creating-a-direction-sensitive-people-counter-with-opencv-and-mobilenetssd-454627fe3c84

## 7.Topic: The C3 Framework: An open source Crowd-Counting-Code framework

Author: Pooja Vinod

Read here: https://medium.com/secure-and-private-ai-writing-challenge/c3-crowd-counting-code-an-open-source-crowd-counting-framework-in-pytorch-b0a8b94036ba

________________________________________________________________________________________________________________________________________

**_See our project board of tasks, used to organize the project work and divide tasks among members:_**
https://github.com/poojavinod100/People-Counting-Crowd-Density-Detection/projects/1
____________________________________________________________________________________________________________________________________
## PROJECT TIMELINE AND PROGRESS UPDATES:
___________________________________________________________________________________________________________________

-**31/7/19 :Pooja:** Completed implementation of a people counter to be used at doors of exhibitions/public events to detect,count and track the net number of  visitors, inflow and outflow of people from a specific event. Can be used to determine the most popular choice of events/performances/talks at concerts/festivals where multiple events happen simultaneously. This implementation uses OpenCV, dlib and MobileNet SSD. Output rate:34 FPS

Tutorial followed: https://www.pyimagesearch.com/2018/08/13/opencv-people-counter/

You can see how the output looks here: https://drive.google.com/open?id=1xB9FA0hkU-ns3o5Zs4uCwAwZOY8uCWvA

If you are using the code download from the tutorial link, please note the change at line 160 to prevent Boost Error, concerning type mismatch. (See comments beneath the tutorial)(people_counter.py in this repo has the edited code)

-**02/08/19 :Pooja:** Interest form for the Project Showcase Challenge submitted. 

-**03/08/19 :Sreekanth:** Completed implementation of crowd counting and tracking using deepsort and YOLO. Recommendation for improvement required in FPS noted(current rate:8-10 FPS). 

Pull request for code merged by Pooja into the 'Contributions' folder.

Code reference used: https://github.com/Qidian213/deep_sort_yolov3 

You can see how the output looks here: https://drive.google.com/open?id=1h-XJTDbw_h-v3iaAf_z-1HXVkojOhRNL

-**06/08/19 :Pooja:** Project board with tasks created on the GitHub repo. 

-**09/08/19 :Pooja:** Tasks assigned to all team members. See Project Board for tasks in progress. 

-**13/08/19 :Pooja:** Review #1 of research article by Ramkrishna Acharya done. Feedback given. 

-**14/08/19 :Pooja:** Work on website for project work consolidation started.

-**15/08/19 :Pooja:** Work on website for project work consolidation almost complete. Requirements from team members communicated. 

-**15/08/19 :Pooja:** C3 framework explored and link to repo included in 'Contributions' folder. At destination repo, please visit results_reports folder  for details of results obtained.  

-**15/08/19 :Pooja:** Review #2 of research article by Ramkrishna Acharya complete. Edits made and article recommended for submission to SPAIC Medium Publication. 

-**16/08/19 :Sreekanth:** Completed implementation of crowd counting on images using CSRnet model. Trials on videos done. 

Pull request for code merged by Pooja into the 'Contributions' folder.

-**17/08/19 :Ramkrishna:** Published Medium article on a research-based comprehensive study of Crowd Counting, specifically on the most popular datasets used: https://medium.com/@qrka/crowd-counting-made-easy-1bf84f18ff61

-**17/08/19 :Sreekanth:** Published Medium article on crowd counting implementation with DeepSort and YOLO: https://medium.com/@sreekanthj244/udacitys-secure-private-ai-project-showcase-challenge-i-de38729ca530

-**19/08/19 :Suraiya:** Published research-based Medium article about the wide diversity of use cases that Crowd Counting can be applied to: https://medium.com/secure-and-private-ai-writing-challenge/crowd-counting-approaches-use-cases-and-importance-part-1-ad9c3cb12f13

-**19/08/19 :Sreekanth:** Published Medium article on implementing crowd counting with CSRnet: https://medium.com/@sreekanthj244/implementation-of-csrnet-crowd-counting-project-for-udacity-project-showcase-a451b4397d71

-**19/08/19 :Pooja:** Published Medium article on implementing People Counter with OpenCV and MobileNet SSD: https://medium.com/secure-and-private-ai-writing-challenge/creating-a-direction-sensitive-people-counter-with-opencv-and-mobilenetssd-454627fe3c84

-**19/08/19 :Pooja:** Published Medium article about C3 framework, an open source crowd counting framework in PyTorch: https://medium.com/secure-and-private-ai-writing-challenge/c3-crowd-counting-code-an-open-source-crowd-counting-framework-in-pytorch-b0a8b94036ba

-**19/08/19 :Pooja:** Published Medium article on concluding remarks about the entire project: https://medium.com/secure-and-private-ai-writing-challenge/concluding-notes-the-crowd-density-project-df22af5b3f6f

-**19/08/19 :Pooja:** Finished maintenance and work on GitHub repo and website for Project Showcase. 

________________________________________________________________________________________________________________________________________
## Slack Communication Archive for this project:
_________________________________________________________________________________________________________________________________

View the slack posts on #sg_wonder_vision related to this project here: https://docs.google.com/document/d/1U-sp_a3jg-xSMCdwziBvDC6xdWLUsFe1TPLIE-EqCzU/edit?usp=sharing
