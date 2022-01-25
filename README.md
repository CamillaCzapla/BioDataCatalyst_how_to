# BioDataCatalyst_how_to

Create an account on BioDataCatalyst and apply for pilot fund.

Here is a link to the log in.

https://accounts.sb.biodatacatalyst.nhlbi.nih.gov/auth/login?next=https%3A%2F%2Faccounts.sb.biodatacatalyst.nhlbi.nih.gov%2Foauth2%2Fauthorization%3Fresponse_type%3Dcode%26client_id%3D74735b722c33498cb981b6b6e24f659f%26redirect_uri%3Dhttps%253A%252F%252Fplatform.sb.biodatacatalyst.nhlbi.nih.gov%252Foauth2%252Fredirect%26state%3D56VfYiGpbqzHFugrQww5q1Mt52d1gy%26scope%3Dopenid%26nonce%3D4629593785763062241636731129#

Once I was approved in a project in BioDataCatalyst, I could access my project dashboard. 
In order to download/upload files to your project, one needs to download the Seven Bridges Command Line Interface (SB CLI).
From the Dashboard, this can be found by clicking Data > Data Tools. I clicked Download under SB CLI. 
I downloaded the interface for my preferred system. I chose Linux x64. 

On the terminal I went through my files until I was in the folder with "sb." 
Secure transfer command: scp sb camilla@10.22.9.205:/home/camilla
Once I had sb on the server, I needed to use this command to be able to run it as a program: chmod a+x sb.
Note: I needed to put "./" in front of all my commands
