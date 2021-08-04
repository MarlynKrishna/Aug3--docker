# Aug3--docker

3)setup python notebook 

a)Installing python->https://www.datasciencelearner.com/install-and-run-python-in-docker-container/
 
->running ubuntu->docker run -ti -d ubuntu: latest 
->To get images ->docker ps  
->Updating ubuntu to latest version ->apt-get update 
->Install python ->apt-get install python3 
->apt-get install python3 

1.sudo ls 
2.su - 
3.apt-get update 
4.apt-get install sudo 
5.sudo ls 
6.sudo apt update 
7.sudo apt install python3-pip python3-dev 
8.it will asks do you want to continue [y/n] we should give y to install 
9.sudo -H pip3 install --upgrade pip 
10.sudo -H pip3 install virtualenv 

##some members got some errors here ...we tried to rectify, but we couldn't 
11.mkdir ~/myproject_dir 
12.cd ~/myproject_dir 
13.virtualenv myproject_env 
14.source myproject_env/bin/activate 
15.pip install jupyter 

16.jupyter notebook --allow-root 

Reference link:: How To Set Up Jupyter Notebook with Python 3 on Ubuntu 18.04 | DigitalOcean 

@@ only few people got connection with jupyter by  doing above commands, rest didn't get. 

ssh -L 8888:localhost:8888 root@rootaddress 

docker run -p 8888:8888 jupyter  

docker run -p  8888:8888 jupyter minimal-notebook(name of the directory) 

##we got link to connect jupyter  

@@who got local host link  they got error. That  link refused them to connect the jupyter. 

And they did cntrl -c to close all the terminals.  

Then they did port forwading.Then they got accesss to connect jupyter, and they performed sample code it worked. 

 

 

 

 
____________________________ 
1)docker pull jupyter/datascience-notebook 
2)mkdir notebook(name of directory) 
3)cd notebook 
4)docker run --rm -p 8888:8888 -e JUPYTER_ENABLE_LAB=yes -v "c:/foldername (where we created that directory/located)/notebook":/home/acn/work jupyter/datascience-notebook 
5)then we will get some local host link to connect jupyter. 

6)we connected to the jupyter and we selected  the python version, and then we created sample code. 

@@@ rest people got result by using above commands. 

 

Reference link::    https://hub.docker.com/r/jupyter/datascience-notebook 

 

 
 


 

 
