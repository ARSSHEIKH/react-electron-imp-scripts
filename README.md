# react-electron-imp-scripts
react+electron important scripts to for start both desktop and web same time (on dev mode). 

## Step # 01:
  ### Add this code in package.json:
   #### inside the devDependencies

      "devDependencies": {
        "concurrently": "^6.0.2",  // or current version
      }
      
## Step # 02
### Then this scripts this script for running both or single:
  
    "scripts": {
      "dev": "concurrently \"SET BROWSER=none&&npm run start\" \"wait-on http://localhost:3000 && electron .\"",
      "electron": "wait-on tcp:3000 && electron .",
      },

## Step # 03
### then install it:
      npm install or npm i

### and finnaly run it using
                    
      npm run dev
      
Be happy !!
