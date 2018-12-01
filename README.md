# COMP 551: Final Project

## Connecting to and Using AWS
Make sure you have the AWS key downloaded
Then run:
```
chmod 400 aml-final.pem
ssh -i aml-final.pem ec2-user@ec2-35-172-191-188.compute-1.amazonaws.com
```
This will connect you to the instance. From there you can run your notebooks from the command line using:
```
jupyter nbconvert --execute <notebook>
```
I would suggest updating files by making changes to files on your local system and uploading them to github, and then calling:
```
git pull
```
Lastly, I suggest adding a cell in the notebooks that downloads processed data from 
```
https://www.cs.mcgill.ca/~glluch/
```
instead of processing data repeatedly or having to manually transfer data every time.