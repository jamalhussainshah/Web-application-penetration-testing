This lab is created by ghanimah in canada in order to capture the flag Hunt down social media accounts by username across social networks .
Here i have attahed snapshot to overlook that how sherlock is installed from github and how it perform step by step. 


You can seen below commands  run sherlock in Ubuntu OS for hunting user profile 

# clone the repo
$ git clone https://github.com/sherlock-project/sherlock.git

# change the working directory to sherlock
$ cd sherlock

# install the requirements
$ python3 -m pip install -r requirements.txt


There some problem during installation last command specially but its very sample to solve this issue by simply following below steps:

$ python3 -m pip install -r requirements.txt

Error shown : conda 4.10.3 requires ruamel_yaml_conda>=0.11.14, which is not installed.

So exit installation of this $ python3 -m pip install -r requirements.txt and try to install below command first

 conda install python=3

Then 

Install 

python3 -m pip install -r requirements.txt

and now you are ready to explorer through sherlock by simple input below command.

python3.7 sherlock userprofilename
