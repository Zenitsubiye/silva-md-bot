## Deploy on VPS or PC or Termux.
- You need to Install git,ffmpeg,curl,nodejs,yarn with pm2 
   1. Install git ffmpeg curl 
      ``` 
       sudo apt -y update &&  sudo apt -y upgrade 
       sudo apt -y install git ffmpeg curl
      ``` 
   2. Install nodejs  
      ```   
      sudo apt -y remove nodejs
      curl -fsSl https://deb.nodesource.com/setup_lts.x | sudo bash - && sudo apt -y install nodejs
      ```
  
   3. Install yarn
      ```
      curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - 
      echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
      sudo apt -y update && sudo apt -y install yarn
      ```  
  
   4. Install pm2
      ```
      sudo yarn global add pm2
      ```
  
   5. Clone Repo and install required packages
      ```
      git clone https://github.com/SilvaTechB/silva-md-bot
      cd Gifted-Md
      yarn install --network-concurrency 1
      ```

   6. Create an env file for ENV. 
      ```
      touch config.env
      nano config.env
      ```
      copy paste lines below.

      ```
      OWNER_NUMBER="254743706010"
      SESSION_ID = "SESSION_85_23_59_01_kjgfgfclhj"
      THUMB_IMAGE = "https://telegra.ph/file/751eef74109e0e5c8916c.jpg"
      OWNER_NAME = "silva"
      PREFIX = .
      WARN_COUNT = 5
      DISABLE_PM = "true"
      THEME= "Silva"
      MODE = "private"
      ANTILINK_VALUES = "https://,chat.whatsapp.com"
      
      ```
      ctrl + o and ctrl + x, To save and exit

   7. start and stop bot
 
      To start bot ``` npm start ```,
      To stop bot ``` npm stop ```

 
<h2 align="center">  NOTICE </h2>
---
- *Silva-Md is not made by `WhatsApp Inc.` Sometimes or misusing the bot might `ban` your `WhatsApp account!`*
- *In that case, I'm not responsible for banning your account.*
- *Use Silva-Md at your own risk by keeping this warning in mind.*
 
