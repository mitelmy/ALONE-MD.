# ALONE-MD 

##
![spider](https://github.com/user-attachments/assets/477316e6-e1d2-40f6-9002-ba18050251b7)


## How to Get ALONE-MD 

1. Click on Fork repo <br>

<a href="https://github.com/Aloneboytech/ALONE-MD-/fork"><img title="FORK REPO" src="https://img.shields.io/badge/FORK REPO-h?color=black&style=for-the-badge&logo=stackshare"></a>


🌹 to copy the repo to your GitHub account. Don’t forget to add a star 🌟 to encourage the developers.💫

2. Obtain a bot session: 

<a href='https://alone-md-q9gg.onrender.com' target="_blank">
    <img alt='SCAN QR' src='https://img.shields.io/badge/Scan_qr-100000?style=for-the-badge&logo=scan&logoColor=white&labelColor=black&color=black'/>
</a>

##
<a href='https://alone-md-q9gg.onrender.com' target="_blank">
    <img alt='PAIR CODE' src='https://img.shields.io/badge/Scan_qr-100000?style=for-the-badge&logo=scan&logoColor=white&labelColor=Blue&color=Blue'/>
</a>

- **Render Deployment:**
1. If you don’t have a **Render** account, click [**here**](https://dashboard.render.com) to create one.
2. Create a new web service.  
3. Choose **Public Git Repository**.  
4. In the field, enter `https://github.com/Aloneboytech/ALONE-MD-`.
5. Click **Connect**.  
6. Select the **Free Plan** if you don’t want to pay.
7. In the **Environment Variable** section, click **Add from .env** and copy the content below:

```env
    
- **Github Deployement**

  1. Fork The Repo
  2. Edit the file `exemple_de_set.env` to `set.env` and put your session_ID in
  3. create a new file `.github/workflows/deploy.yml` and put this content in :

```yml
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: npm install

    - name: Start application
      run: npm start

 ```
