# update
##Main Features:- 

1. OTA Updates through Github

2.Change ESP8266 WiFi credentials without uploading code from Arduino IDE

#Steps :-

      1.Downlaod  [ino file](https://github.com/sagarkayarkar/update) from this Repo  .

      2.Create the new Repository and add the 'version.txt'file in to repo 
      
      3.Increase the version no by 1 in the (for ex if the flashed program version is 1.0 then it should be 1.1) .ino file code and create the binary file of the same file .
      
      4.open the .ino  file in arduno from obove link and create binary file .for creating binary file click  >Sketch>Export Compiled Binary . Binaryu file will be save in the same folder where 
      the .ini file is present .
      
      4.Copy that binary file in to the Repo folder and and edit the version.txt file .
      
      5. Write '1.1' in 'version.txt' as older version in '1.0'
      
      6. NOw commit your changes .
      
      7 Copen the repo from web browser and copy the link of all the two file version.txt and binary file i.e .bin file 
      6.It will be look like this 
        -https://github.com/sagarkayarkar/update/blob/master/ota_update.ino.nodemcu.bin
        -https://github.com/sagarkayarkar/update/blob/master/version.txt
        
      6. for downloading this files from the node mcu this link wont work we need redirection link 
      7 .edit same link to 
        -https://raw.githubusercontent.com/sagarkayarkar/update/master/version.txt
        -https://raw.githubusercontent.com/sagarkayarkar/update/master/ota_update.ino.nodemcu.bin
        
        that means you have to replace 'github.com/' to 'raw.githubusercontent.com' this and remove '/blob/" file the link that will work
        
      8.Copy the edited link in the ino file and flash the same code in nodemcu using USB cable . the version should be 1.0 
      9. increase the version to 1.1 in .txt and binary file and commit to git .
      10 .node mcu will contusly read the .txt file and it will check the data of .txt file file the version of .txt file and firmawere running inthe code is differnt it will update the firmware .
      11. for updating the firmware again 
      -change the version in .txt and ino file 
      -genrate binary file and paste it to repo folder 
      -commit changes
      make sure the file name should not be change .
      
