# People-Counting-Crowd-Density-Detection
This is a project at #sg_wonder_vision study group of the Facebook Secure and Private AI Scholarship Challenge 2019

**Project Description:**
****************************************************************************************************************************************
-The main objective of this project is to build a self-sufficient software, that can accurately predict whether or not a stampede is imminent, based on the incoming live visuals of a place. 
-Often, huge footfall is associated with various popular festivals, religious ceremonies, public events, concerts etc. The enormous count of people coupled with their density(how close they are to each other) easily poses the risk of a normal crowd turning into a dangerous stampede that could potentially cost many lives. 
-This has happened several times in the past, especially at the world-famous Kumbh Mela(a festival where 30 million people take part in Allahabad, when the city can only hold about 9 million), and the recent tragedy at Elphinstone Railway station, Mumbai. 
-Most current stampede prevention solutions are reliant on hardware(footfall mats based on sensors etc), bringing along with it the question of capital investment, installation and maintenance costs and issues in the long run. 
-The key innovation we hope to create here is steer this project in the direction of a **completely software-based solution(based on Computer Vision Technology, that does not depend on inputs from any electronic hardware, which can be done using only the live CCTV visuals of the area we are monitoring)** for this problem, that can provide good levels of accuracy to accurately predict stampedes, so that some kind of intervention can be done at the right time to prevent such incidents in the future.
****************************************************************************************************************************************
________________________________________________________________________________________________________________________________________
**Team Members(Slack Handles):**
@Pooja Vinod(Project Lead)
@Sreekanth Zipsy
@Viper
@Suraiya Khan
________________________________________________________________________________________________________________________________________
**Project Progress Updates:**

-**31/7/19 :Pooja:** Completed implementation of a people counter to be used at doors of exhibitions/public events to count the net number of  visitors, inflow and outflow of people from a specific event. Can be used to determine the most popular choice of events/performances/talks at concerts/festivals where multiple events happen simultaneously. This implementation uses OpenCV, dlib and MobileNet SSD. Output rate:34 FPS

Tutorial followed: https://www.pyimagesearch.com/2018/08/13/opencv-people-counter/

You can see how the output looks here:https://drive.google.com/file/d/1xB9FA0hkU-ns3o5Zs4uCwAwZOY8uCWvA/view

If you are using the code download from the tutorial link, please note the change at line 160 to prevent Boost Error, concerning type mismatch. (See comments beneath the tutorial)(people_counter.py in this repo has the edited code)

*Related files and folders:*

pyimagesearch

videos

people_counter.py

mobilenet_ssd

-**02/08/19 :Pooja:** Interest form for the Project Showcase Challenge submitted. 

-**03/08/19 :Sreekanth:** Completed implementation of crowd counting and tracking using deepsort and YOLO. Recommendation for improvement required in FPS noted(current rate:8-10 FPS). 

Pull request for code merged in the 'Contributions' folder.

Code reference used: https://github.com/Qidian213/deep_sort_yolov3 

-**06/08/19 :Pooja:** Project board with tasks created on the GitHub repo. 

-**09/08/19 :Pooja:** Tasks assigned to all team members. See Project Board for tasks in progress. 

-**13/08/19 :Pooja:** Review #1 of research article by Ramkrishna Acharya done. Feedback given. 

-**14/08/19 :Pooja:** Work on website for project work consolidation started.

-**15/08/19 :Pooja:** Work on website for project work consolidation almost complete. Requirements from team members communicated. 

-**15/08/19 :Pooja:** C3 framework explored and link to repo included in 'Contributions' folder. At destination repo, please visit results_reports folder  for details of results obtained.  

-**15/08/19 :Pooja:** Review #2 of research article by Ramkrishna Acharya complete. Edits made and article recommended for submission to SPAIC Medium Publication. 

View the slack posts on #sg_wonder_vision related to this project here: https://docs.google.com/document/d/1U-sp_a3jg-xSMCdwziBvDC6xdWLUsFe1TPLIE-EqCzU/edit?usp=sharing
