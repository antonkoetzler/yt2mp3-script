# yt2mp3-script
A Windows/Linux friendly executable that converts a YouTube link into an MP3. Made for converting YouTube links to MP3 faster than using solely youtube-dl.

# Installing on Windows
1. Install ffmpeg: https://www.geeksforgeeks.org/how-to-install-ffmpeg-on-windows/
2. If you get a "MSVCR100.dll missing" error, install vcredist_x86.exe here: https://www.microsoft.com/en-ca/download/details.aspx?id=26999
3. Go to https://github.com/antonkoetzler/yt2mp3-script/releases/tag/1.0 and download yt2mp3-script-windows.zip
4. Extract yt2mp3-script-windows.zip into desired directory (examples: C:/ or C:/Users/$USER/)
5. Add this directory as an environment variable
- Open windows settings

![image](https://user-images.githubusercontent.com/66643637/169671768-2074b618-d2b4-4cf5-b7fc-f655ecddfbad.png)

- Search "Environment" and click "Edit the environment variables"

![image](https://user-images.githubusercontent.com/66643637/169671787-7fce3dd1-647a-4059-adb6-6f64d6114914.png)

- Click "Environment Variables..."

![image](https://user-images.githubusercontent.com/66643637/169671803-d9cd25e0-25ae-4152-8fbf-f981a8dc6364.png)

- Click the highlighted option "Path" in the previous screenshot
- Click "New" on the left and add the directory to yt2mp3-script (examples: C:/yt2mp3-script or C:/Users/$USER/yt2mp3-script

# Installing on Linux (compiling from source)
1. Install dependencies: `sudo pacman -S ffmpeg youtube-dl base-devel`
2. `git clone https://github.com/antonkoetzler/yt2mp3-script.git; cd yt2mp3-script; g++ yt2mp3.cpp -o yt2mp3`
3. Move the executable anywhere and add the directory as a path
- vim ~/.bashrc
- Add `export PATH="$HOME/.local/bin/:$PATH"`
