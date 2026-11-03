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

_Windows icon + R and type msinfo32, to see specs_

---

## How to use git (This is so our workspace/files/codes are all in one place and shared)

### Step 1: Generate your Personal Access Token (PAT)
GitHub requires a **Personal Access Token (PAT)** instead of your account password to push code from the terminal.

1. Log in to Github
2. Click your **profile picture** (top-right) -> **Settings**.
3. Scroll down the left sidebar and click **Developer settings**.
4. Click **Personal access tokens** -> **Tokens (classic)**.
5. Click **Generate new token** -> **Generate new token (classic)**.
6. Enter a Note (e.g., `any name`), select an `no expiration date`, and check the **`repo`** checkbox.
7. Scroll to the bottom and click **Generate token**.
8. Copy the token (the one that starts with gph_) and save it somewhere you can easily copy and paste later.

---

### Step 2: Link The Existing Folder to GitHub
Open ubuntu and run:
_Paste the lines 1 by 1_
```bash
cd ~/krpc/krpc7th-simulator/users

git init

git remote add origin [https://github.com/cian198/Krpc7th-Group-1.git](https://github.com/cian198/Krpc7th-Group-1.git)
```

### Step 3: Updating the files online with the code you've edited/made on your laptop
```bash
git add .
git commit -m "describe what you edited"
git pull origin main --rebase
git push -u origin main
```
**If the terminal asks for your password, paste the Token you got from Step 1**
