# Krpc7th-Group-1
How to install and use workspace repository

# Installation
We'll install it using a pre-built image (on my hard drive) instead of the processes listed on the programming Manual pdf so it will be faster 
* Won't get limited by school wifi
* Since its pre-built, installation will be faster and easier and won't require a couple hours to built/install

**Or if you can install it yourselves using the Programming Manual pdf (it will take about 3hrs)**

### Pre-built installation
1. Bring me your laptop face to face and I'll install it 😁
   
    * Specs of the laptop should be at least 4+ cores, 16gb+ ram, and have free storage of about 15gb

### Windows icon + R and type msinfo32, to see specs
<br>
<br>
<br>
<br>

## How to use git 
In order to update our code online collaboratively we use github/git, think of it as a shared google doc but for files and codes 👍

### Step 1: Making a SSH Key
1. Make a github account
2. Open **Ubuntu** using windows search
3. Copy paste the command
```bash
# Replace the "your_email@gmail.com" with your actual email you used for github
ssh-keygen -t ed25519 -C your_email@gmail.com
```
4. Press enter when asked for a directory
5. Enter a passphrase (aka any password)
6. Copy paste the command, this will show the SSH Key
```bash
cat ~/.ssh/id_ed25519.pub
```
### Setting SSH Key in github
1. Copy the entire line printed on the screen (starting with ssh-ed25519 up to your email).
2. Go to GitHub.com -> Click your profile picture -> Settings.
3. In the left sidebar, click SSH and GPG keys.
4. Click New SSH key.
5. Give it any title you like, set Key type to Authentication Key, paste your key into the Key field, and click Add SSH key.
6. Verify connection
```bash
cd
cd ~/krpc/krpc7th-simulator/users/catkin_ws/src/krpc_user
ssh -T git@github.com
```
If ever prompted with "Are you sure you want to continue connecting (yes/no/[fingerprint])?"

type yes and press Enter.
<br>
<br>
<br>
<br>

### How to actually edit the codes
1. Pull the latest changes from GitHub
Before writting any new code or make changes, always pull the latest updates from github to ensure your local workspace is up to date:
```bash
cd
cd ~/krpc/krpc7th-simulator/users/catkin_ws/src/krpc_user
git pull origin main
```
2. Editing the code

Only edit the files inside the src(c++) and script(python) folders using whatever coding program you are using

4. Saving locally

When committing write a message of what you change (e.g "Revised movement codee")
```bash
git add .
git commit -m "Revised movement code"
```

4. Updating the files online
```bash
git push origin main
```
👍👍👍

## Where to find the scripts

Run the lines 1 by 1
```bash
cd
cd ~/krpc/krpc7th-simulator/users/catkin_ws/src/krpc_user
explorer.exe .
```
Then open src (if you wanna code in c++) or open scripts (if you wanna code in python)
