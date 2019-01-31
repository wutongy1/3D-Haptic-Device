This code is used for nearest point searching using flann library. data used for test is generated inside of the code. detail installation for the needed library is in the following

First, uninstall the default flann and lz4 using this command:
sudo apt-get remove liblz4-dev sudo apt-get remove libflann-dev then install flann and lz4 from github

Install flann library from github: https://github.com/mariusmuja/flann
Install lz4 from github: https://github.com/lz4/lz4

# provide permission to access usb without use of sudo or root
we have to give read, write, execute privilege for all user/group/other to access the device by using the following command
sudo chmod 777 /dev/ttyACM0 
a detail explantion about permission grant can be found here.
https://www.maketecheasier.com/file-permissions-what-does-chmod-777-means/
