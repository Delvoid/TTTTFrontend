<!-- PROJECT LOGO -->
<p align="center">
  <a href="https://github.com/DanGiaime/ClipbotFrontende">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">CLIPBOT</h3>

  <p align="center">
    All it takes to go viral on TikTok is one good clip.
Clipbot automatically posts your Twitch clips to TikTok and Youtube so you'll go viral overnight.
    <br />
    <a href="https://clipbot.tv/"><strong>Website</strong></a>
    <br />
  </p>
</p>

## Clipbot Frontend

Clipbot frontend repo. Help make Clipbot better!

<!-- GETTING STARTED -->

## Getting Started

### Prerequisites

<br />

- npm

  ```sh
  npm install npm@latest -g
  ```

- Download [Clipbot](https://clipbot.tv/download)

<br />

### Installation

<br />

1. Clone the repo
   ```sh
   git clone https://github.com/DanGiaime/ClipbotFrontend.git
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Run the app <br />
   To run the backend you need to run the live version of clipbot
   ```sh
   npm start
   ```
   This will open an electron app. To open dev tools in electron you can press 'crtl'+'shift'+i you will also need add the enviroment variable. Ask in [discord](https://clipbot.tv/discord) for this

<!-- CONTRIBUTING -->

## Contributing

<br />

Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b newBranch`)
3. Commit your Changes (`git commit -m 'New Changes'`)
4. Push to the Branch (`git push origin newBranch`)
5. Open a Pull Request

Github standard [Form & Pull request](https://gist.github.com/Chaser324/ce0505fbed06b947d962) workflow

# TTTT Frontend UI Spec

Pages

- Main Screen

  ![Untitled](TTTT%20Frontend%20UI%20Spec%20ea1c97f7f85443ef8be0b006ce25ee4a/Untitled.png)

  - Displayed info
    - CLIPBOT Title
    - Short blurb of text describing that clips are uploaded while the window is open
      - "While this window is open, we'll be uploading your twitch clips to TikTok every few hours! Keep this program open, and change any settings below."
    - Title of next clip
      - (I will fill this in, just need placement)
      - Example value:
        - Spaghetti is ready THE LEGEND OF ME
      - Notes:
        - This can sometimes be really long make sure to cut it off if in css, `...` is fine for overflow
    - Video of next clip
      - (I will fill this in, just need placement)
    - Last Upload:
      - (I will fill this in, just need placement)
      - Example value:
        - September 3, 1:17PM
    - Next Upload:
      - (I will fill this in, just need placement)
      - Example value:
        - September 3, 7:17PM
    - Default Vertical video
      - (I will fill this in, just need placement)
      - Example value:
        - ON
        - OFF
      - (Feel free to make this a button or icon or something else if you want
    - Clip Hotkey
      - (I will fill this in, just need placement)
      - Example value:
        - F10
        - Shift+F10
    - Current status
      - (I will fill this in, just need placement)
      - Example values:
        - Waiting for next upload
        - Checking tiktok login
        - Downloading clip from twitch
  - Buttons/Inputs
    - Manage Clips
    - Turn Clipbot ON/OFF
      - Notes
        - This is a toggle, feel free to move this button into another menu if you'd like
    - How it works
    - Main settings
    - Video Settings
    - Need Help

[]()

- Manage Clips

  - Displayed info

    - List of video clips, display by thumbnail
      - Notes:
        - I will provide thumbnail images, expect 720p or 1080p
    - For each clip
      - Is the clip approved?
      - Has the clip been uploaded?
      - Clip Title
      - Notes:
        - I will provide data on approved/uploaded true/false
        - Feel free to display this however you want
        - Green shadow / faded view / etc, totally up to you as long as it's clear
    - Reference Image:

      ![Untitled](TTTT%20Frontend%20UI%20Spec%20ea1c97f7f85443ef8be0b006ce25ee4a/Untitled%201.png)

  - Buttons/Inputs
    - Filter by approval status
      - Type
        - Dropdown
      - Values
        - Approved
        - Rejected
        - Auto-approved
        - All Approved
    - Filter by view count
      - Type
        - Number input,
      - Values
        - Can take any number 0+
    - Filter by clips after a start date
      - Type
        - Some sort of date selector
      - Values
        - Any date
    - Filter by clips before an end date
      - Type
        - Some sort of date selector
      - Values
        - Any date
    - Filter by words in title
      - Type
        - Text entry
      - Values
        - Any set of characters

- Edit Clip
  - Displayed info
    - Clip Title
      - (I will fill this in, just need placement)
    - Approval Status
      - (I will fill this in, just need placement)
      - Example values:
        - Approved
        - Rejected
        - Approved By Default
    - Upload Status
      - (I will fill this in, just need placement)
      - Example values:
        - Uploaded
        - Not Uploaded
    - Clip Video
      - (I will fill this in, just need placement)
      - Just use 1080p image/video as placeholder
  - Buttons/Inputs
    - Approve
      - Simple icon button with word "approve"
    - Reject
      - Simple icon button with word "Reject"
    - Change Orientation
      - Swap between "vertical" and "horizontal"
      - Represent this however you like
    - Set Custom Crop
      - Simple icon button with word "Crop"
    - Title input
      - Single line text input
    - Save Title Button
      - Simple button near title input with word "Save" or "Save title" or just a save icon as long as it's clear
- Main Settings
  - Displayed info
    - Hashtags
      - Type
        - Text, list of hashtags separated by spaces
      - Example value:
        - #streamer #twitch #viral
    - Clip Hotkey
      - Type
        - Text
      - Example value:
        - F10
    - Clip Age
      - Type
        - Number / Text
      - Example value:
        - 8 hours
    - Minimum Views
      - Type
        - Number / Text
      - Example value:
        - 3 views
    - Time Between Posts
      - Type
        - Number / Text
      - Example value
        - 8 hours
    - Default Approve
      - Type
        - toggle (On/Off)
      - Example value:
        - On
  - Buttons/Inputs
    - Hashtags
      - Type
        - Text input
      - Notes
        - Must make it clear that the input format is a space-separated list of hashtags, like this:
          - `#tag #anothertag #thirdtag`
    - Clip Hotkey
      - Type
        - Text input
      - Notes
        - User will have to click the key they want, so make it look like a text input but it is technically not _really_ a text input
        - Must display this sentence as an input subtitle or similar:
          - `Press this to make a clip!`
    - Clip Age
      - Type
        - Number input
      - Notes
        - Must display this sentence as an input subtitle or similar:
          - `Clips must be this old to be posted`
    - Minimum Views
      - Type
        - Number input
      - Notes
        - Must display this sentence as an input subtitle or similar:
          - `Clips must have this many views to get posted`
    - Time Between Posts
      - Type
        - Number entry
      - Notes
        - Must display this sentence as an input subtitle or similar:
          - `Wait this long between posts`
    - Default Approve
      - Type
        - Toggle
      - Notes:
        - Must display this sentence as an input subtitle or similar:
          - `Upload any clip unless it has been rejected`
- Video Settings
  - Displayed info
    - Explainer text
      - Type
        - Text
      - Value
        - `Use these settings to make your videos vertical by default.`
        - After that sentence, either:
          - `Default Vertical Video is OFF, so your videos will be uploaded as horizontal unless you customize them individually.`
          - `Default Vertical Video is ON, so your videos will be cropped.`
    - Default Vertical Video
      - Type
        - Toggle (On/off)
      - Example value:
        - On
  - Buttons/Inputs
    - Default Vertical Video
      - Type
        - Toggle (On/off)
      - Example value:
        - On
    - Change Default Crop
      - Type
        - Button
- Help Menu
  - Displayed info
    - None
  - Buttons/Inputs
    - Join Discord
      - Type
        - Button
    - Bug Report
      - Type
        - Button
    - Logout
      - Type
        - Button
    - Force Upload Now
      - Type
        - Button
- How It Works
  - Displayed info
    - Title
      - Type
        - Text
      - **`How To Use Clipbot`**
    - subtitle
      - Type
        - Text
      - `Watch these videos to learn the best ways to use Clipbot!`
  - Buttons/Inputs
    - The Basics
      - Type
        - Button
    - Main Screen
      - Type
        - Button
    - Main Settings
      - Type
        - Button
    - Video Settings
      - Type
        - Button
    - Clip Hotkey
      - Type
        - Button
    - Help Menu
      - Type
        - Button
