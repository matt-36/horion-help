# Crash on join

## causes

- A unsafe module is enabled in config which can cause the client to crash

## Solutions

### Modify, or Delete config

config

#### Step 1: find the configuration file

Press the windows key + r (win+r) to bring up the run menu

Then input

```
%localappdata%\Packages\Microsoft.MinecraftUWP_8wekyb3d8bbwe\RoamingState
```

and press enter

A file explorer should appear

#### Step 2: Delete config

Delete the file named Default.h or edit it if you know what you are doing
