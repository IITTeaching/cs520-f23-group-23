README 

Steps to reproduce the project

Installation of the latest Python version 3.10 on Unix
sudo apt install python3.10
or preferably if you have homebrew on MacOS then:
brew install python@3.10

Activation of virtual environment
----------------------------------------------------------------------
python3 -m venv .venv  
source .venv/bin/activate  
which python  



Ensure the python version is 3.10 and JDK is 8+ there is a bug in JDK 9 
that prevents saving of dataframe because of non-compatbility with latest pyspark
----------------------------------------------------------------------

wget https://maven.mimirdb.info/info/vizierdb/vizier  

chmod +x vizier  

sudo mv vizier /usr/local/bin  


Disclaimer: Please note that there is an alternate installation of vizier listed in https://vizierdb.info/, however, on Unix, Solaris and MacOS there is an error that states the snappy codec tool is not compatible with the version of pyarrow contained in the Dockerfile on DockerHub which results in an exception being thrown upon saving of a dataframe . Bottom line: Docker based vizier is not yet fully functional as of this writing and so we would need to manually bootstrap the client and server app using the npm based backend.
---

pip3 install numpy==1.26.2  
pip3 install bokeh==3.3.2  
pip3 install matplotlib==3.8.2  
pip3 install astor==0.8.1  
pip3 install pyarrow==14.0.1  
pip3 install pandas==2.1.4  
pip3 install shapely==2.0.2  
pip3 install pyspark==3.5.0  
pip3 install jellyfish==1.0.3  
pip3 install dedupe==2.0.23  
pip3 install nltk==3.8.1  
pip3 install IPython==8.18.1  

Proceed to localhost:5000 on the browser and import the cs520_museum file into a new project 
----------------------------------------------------------------------

vizier


