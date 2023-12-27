# python-app

Here we are containerizing python django application using docker.
tzdata provides timezone information

While writing the Dockerfile- <br>
Step 1: Take the ubuntu version<br>
Step 2: Create a working directory (WORKDIR /app)<br>
Step 3: Copy the data/files into working directory (/app)<br>
        Initial step it to copy the requirements.txt file<br>
        Then other files ( devops ie main code fiels)<br>
Step 4: (Operations)<br>
        Install required tools if they are not present in the base VM<br>
        eg. in our case<br>
        1. Install python <br>
        2. Install requirments.txt (imp)<br>
        3. Go inside the project main folder(devops)<br>
Step 5: (Execution)<br>
        This is an entry point to aur application<br>
        Here we actually execute the file <br>
        We write runnable files, server ports in CMD[]<br>

        ENTRYPOINT[] - We cannot change/overwrite the content present in ENTRYPOINT
                        Like python version, etc
        CMD[]- We can overwrite anything
        
