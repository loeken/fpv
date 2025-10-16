# introduction

this is setting up betaflight on geprc cinelog 25 v2 from scratch using app.betaflight.com ( at the writing of this article 2025.12.0-RC1 )


## flashing 

- heading to app.betaflight.com click on "connect" to connect normally
- retrieving the name of the board ( firmware flasher - press the yellow detect button )


### dfu mode

my button is hard to reach some boards dont have a button the universal way ( on linux )
- have dfu-utils installed
- connect in betaflight head to cli and type in "bl" this will result it in being restarted in dfu mode ( you should see at top right in betaflight )
- for me it says "betaflight dfu in fs mode"


- enable export mode
- show release candidates
- Development
- TAKERG4AIO
- 2025.12.0-beta [latest]
  

on the right side select osd ( me dji so digital ), also select 
- altitude hold
- position hold

i have the gps 10 nano which doesnt have magnometer if yours does maybe add that too


click "load firmware (online)"

followed by flash firmware


once it say "programming successful" you are done and can "connect"


# config start

## configuration
### system configuration
changing pid loop to 8khz
magnometer unchecked ( gps 10 nano doesnt have it )


### board alignment
as this is a pusher board i ll do a board alignment of:
- 180° pitch
- 90° yaw


### personalization
- aircraft name
- pilot name

### camera angle
25° for me