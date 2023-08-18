
#This is a script to execute assignment given in class

#cmd to create new user
echo "sudo useradd Moyo"
![image1](/Tech/task1/screenshot/S1.png)


#Set expiry date of 2weeks for Moyo
echo "sudo usermod -e 2023-08-29 Moyo"
![image2](/Tech/task1/screenshot/s2.png)

#Prompt User to change password on login and return back as root user after changing password
echo "sudo chage -d 0 Moyo"
echo "su Moyo"
echo "sudo su"
![image3](/Tech/task1/screenshot/s3.png)

#Create a group called altschool and add the user
echo "groupadd altschool"
echo "gpasswd -a Moyo altschool"
![image4](/Tech/task1/screenshot/s4.png)

#Give read only access to altschool on /etc
#echo "sudo chmod -R g+rX /etc"
![image5](/Tech/task1/screenshot/Screenshot%20(15).png)

#New user without home directory
echo " useradd -M comfort
![image6](/Tech/task1/screenshot/Screenshot%20(16).png)

#Thank you