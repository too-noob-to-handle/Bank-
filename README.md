#  UPSTREAM_REPO.

This is a modified repo of [anasty's mltb](https://github.com/anasty17/mirror-leech-telegram-bot/tree/h-code) 'h-code' branch.

# Features:

## ALL FEATURES OF [ANAS](https://github.com/anasty17/mirror-leech-telegram-bot)

## By [Maverick](https://telegram.dog/Maverick9099):
- Direct Clone from 
  > GDToT, AppDrive, DriveApp, DriveLinks, DriveAce, DriveBit, DriveSharer, DrivePro, GDFlix, HubDrive, KatDrive, DriveHub, Kolop, DriveFire, DriveBuzz and Sharer.pw links
- Nothing more !

### Note:
I am not the owner of these scrapers. The credit goes to the developer who developed these scripts.
I just made some changes in these scrapers for bypassing more google drive sharers and fixed some issues regarding the compatibility with the code.

# DEPLOY:

### STEP - 1:
Fork [MLTB](https://github.com/anasty17/mirror-leech-telegram-bot) with all branches or use his public template.

### STEP - 2:
Go to 'heroku' branch in your forked repo and add this line in Dockerfile. (MUST else Sharer.pw Links won't be cloned):
```
RUN pip3 install cloudscraper
```
<p><img src="https://telegra.ph/file/dd60c2c30ad81a241e44b.png"/></p>

### STEP - 3:
Create config.env file using this template. [config_sample.env](https://raw.githubusercontent.com/majnurangeela/For-Upstream-Mltb/master/bot/modules/config_sample.env).

Don't touch `UPSTREAM_REPO` & `UPSTREAM_BRANCH` env vars else all these features won't be there !

### STEP - 4:
Fill All Action Secrets.

- `HEROKU_API`: Get it from your heroku account.
- `HEROKU_APP_NAME`: Set unique appname.
- `HEROKU_EMAIL`: Heroku Email ID
- `CONFIG_FILE_URL`: Optional ENV.. You can upload config.env on gist or in heroku branch

### STEP - 5:
RUN workflow with heroku branch from GitHub Action section !

## IMPORTANT ! :

For the simplification I've made some terms..

- `UNIFIED` = AppDrive, DriveApp, GDFlix, DriveBit, DriveLinks, DriveSharer, DriveAce, DrivePro Sharer Links
- `UNIFIED_EMAIL`: USE SAME GMAIL ACCOUNT IN ABOVE MENTIONED SHARERS
- `UNIFIED_PASS` : USE SAME PASSWORD IN ABOVE MENTIONED SHARERS

- `HUBDRIVE_CRYPT`: IT WILL BE USED TO BYPASS HUBDRIVE LINKS ONLY.
- `KATDRIVE_CRYPT`: IT WILL BE USED TO BYPASS KATDRIVE, KOLOP, DRIVEHUB LINKS.
- `DRIVEFIRE_CRYPT`: IT WILL BE USED TO BYPASS DRIVEFIRE & DRIVEBUZZ LINKS.

- `XSRF_TOKEN` & `laravel_session`: BOTH COOKIES WILL BE USED TO BYPASS SHARER.PW LINKS.

## CREDITS:
- [Maverick](https://github.com/majnurangeela) for integration and compatibility fixes
- [Anasty17](https://github.com/anasty17/mirror-leech-telegram-bot) for his MLTB & Heroku Bypass !
- [xcscxr](https://github.com/xcscxr) for his wonderful google drive link scrapers !
