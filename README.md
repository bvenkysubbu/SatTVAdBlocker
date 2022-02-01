# SatTVAdBlocker
Block Satellite Television channel Advertisements in realtime

The End Goal - 
Give users an advertisement free experience when they are watching a satellite channel on their TeleVision.

Let us break it down to parts -
1. Realtime identification of advertisement started/stopped events in live TV.
2. Broadcast the advertisement started/stopped event to end user.
3. Automatically, take the desired action on the user's TV. e.g. mute the TV, unmute the TV, turn off TV.

## Overview

### Serverless Architecture
Using In Memory Database like Redis

### Publish/subscribe messaging

  Administrators = Publishers<br>
  Users = Subscribers<br>
  Particular TV Channel = Particular Topic<br>

### Example

Let us say that we have to block the ads for a particular TV channel, e.g. Sun TV.

#### When an advertisement starts
Administrator has to click a button to publish the message that advertisement has started. This will benefit all users interested in blocking ads for this channel.

#### When an advertisement ends
Administrator has to click a button to publish the message that advertisement has ended. This will benefit all users interested in blocking ads for this channel.
