Installing the Package:

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
NOTE: You may need to update ffmpeg (or install it in the first place) in order for the Matplotlib animation to work. To initially install, run the following script:

```
pip install ffmpeg
```

To update to the most recent version of ffmpeg:

```
conda update ffmpeg
```

