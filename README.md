# python-app

Here we are containerizing python django application using docker.
tzdata provides timezone information

While writing the Dockerfile- <br>
Step 1: Take the ubuntu version<br>
Step 2: Create a working directory (WORKDIR /app)
Step 3: Copy the data/files into working directory (/app)
        Initial step it to copy the requirements.txt file
        Then other files ( devops ie main code fiels)
Step 4: (Operations)
        Install required tools if they are not present in the base VM
        eg. in our case
        1. Install python 
        2. Install requirments.txt (imp)
        3. Go inside the project main folder(devops)
Step 5: (Execution)
        This is an entry point to aur application
        Here we actually execute the file 
        We write runnable files, server ports in CMD[]

        ENTRYPOINT[] - We cannot change/overwrite the content present in ENTRYPOINT
                        Like python version, etc
        CMD[]- We can overwrite anything
        
