# BioDataCatalyst_how_to

Create an account on BioDataCatalyst and apply for pilot fund.

Here is a link to the log in.

https://accounts.sb.biodatacatalyst.nhlbi.nih.gov/auth/login?next=https%3A%2F%2Faccounts.sb.biodatacatalyst.nhlbi.nih.gov%2Foauth2%2Fauthorization%3Fresponse_type%3Dcode%26client_id%3D74735b722c33498cb981b6b6e24f659f%26redirect_uri%3Dhttps%253A%252F%252Fplatform.sb.biodatacatalyst.nhlbi.nih.gov%252Foauth2%252Fredirect%26state%3D56VfYiGpbqzHFugrQww5q1Mt52d1gy%26scope%3Dopenid%26nonce%3D4629593785763062241636731129#

Once I was approved in a project in BioDataCatalyst, I could access my project dashboard. 

UPLOADING FILES TO BIODATACATALYST

In order to download/upload files to your project, one needs to download the Seven Bridges Command Line Interface (SB CLI). 

From the Dashboard, this can be found by clicking Data > Data Tools. I clicked Download under SB CLI. 

I downloaded the interface for my preferred system. I chose Linux x64. 

On the terminal I went through my local machine's files until I was in the folder with "sb." 

Secure transfer command: scp sb camilla@10.22.9.205:/home/camilla 

Once I had sb on the server, I needed to use this command to be able to run it as a program: chmod a+x sb

Note: I needed to put "./" in front of all my commands since the program I'm running is only in my directory.

NEXT, in the terminal use command: ./sb configure (You will get prompted for three pieces of information. Read on.)

MEANWHILE, on BioDataCatalyst, go to Developer > Authentication Token > API endpoint. HERE, one can find the API endpoint URL (copy and paste) and generate the Authentication Token (only once). For the last prompt I chose true...

***In order to download/upload files using the SB CLI, one needs to be the admin of a controlled project. Create a new controlled project on BioDataCatalyst if needed.

To see the projects you can access, use the command: ./sb projects list --user cczapla ##your username

Here is an example of a command I used to download: 

./sb upload start /home/camilla/PrediXcan_tutorial/data/ --destination cczapla/test-cli --tag upload1

Important notes: The format is command > path to directory or file to download > --destination username/project name > --tag name of upload in BioDataCatalyst. ALSO, your project name will need to be lowercase even if the "sb projects list" command shows the name with uppercase letters as in BioDataCatalyst.

From here, one can access the project on BioDataCatalyst. Files can be moved to different projects from there. Select the file and choose copy or move, etc. 
