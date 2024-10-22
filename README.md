### Installing the Package:

To install this package, follow this procedure: 

```
cd /path/you/want/repo 
```

then clone the repo and cd into it:

```
 /git clone git@github.com:jrrice5908/PHY607_Project2.git # with ssh
cd PHY607_Project2
```

Now create the conda environment:


```
conda create -n "PHY607" python=3.12
```

Enter the environment:

```
conda activate PHY607
```
then install the package:

```
pip install -e .
```


### FFmpeg Installation:

**Note:** You may need to update or install `ffmpeg` to enable Matplotlib animations. Installing `ffmpeg` through `pip` will not work, as it i>

#### macOS:
To install `ffmpeg` on macOS, use [Homebrew](https://brew.sh/). If you don't have Homebrew installed, you can install it first by running:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Once Homebrew is installed, run the following command to install `ffmpeg`:

```bash
brew install ffmpeg
```
#### Linux:
To install `ffmpeg` on Linux (Ubuntu/Debian-based systems), use the following commands:

```bash
sudo apt update
sudo apt install ffmpeg
```

For other Linux distributions, use the appropriate package manager for your system (e.g., `yum` for CentOS).

#### Windows:
To install `ffmpeg` on Windows, follow these steps:
1. Download `ffmpeg` from the official website: [FFmpeg Download](https://ffmpeg.org/download.html).
2. Extract the downloaded files to a directory of your choice.
3. Add the `ffmpeg` binary to your system's PATH. To do this:
   - Right-click on `This PC` or `My Computer` and go to `Properties`.
   - Click on `Advanced system settings`.
   - Click on `Environment Variables`.
   - Under `System Variables`, find the `Path` variable and click `Edit`.
   - Click `New` and paste the path to the `ffmpeg/bin` directory.
   - Click `OK` to close all windows.

After installing `ffmpeg`, verify the installation by running the following command in your terminal or command prompt:

```bash
ffmpeg -version
```

### Updating FFmpeg:
To update `ffmpeg` to the most recent version within your conda environment:

```bash
conda update ffmpeg
```

### Running the Main Script:
Finally, to run the main script, you'll first need to make it an executable:

```bash
chmod +x main.sh
```


Additional Note: Testing parameters can be changed by altering values in the "if __name__= '__main__':" section of test.py if desired.
