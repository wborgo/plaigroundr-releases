# plAIgroundr free - a windows UI for generating images using StableDiffusion

I have just started this "dream tool/UI", I want to bring AI to everyone and make it easy for begginers and non tecnical professionals.
Any feedback will be apreciated, if you have any problems or suggestions, feel free to open a discussion or an issue.

There is a lot of features that I will try to bring to this tool, like generations queue,  online community share library, prompt templates, features recommendations and much more.

### new in 0.2.1
- Added a Setup Wizzard window, that guides you to setup the StabbleDiffusion envrironment

### features
- Workspaces: organize your creations with workspaces. Saves your configurations, prompts, images library and will be used with future features.
- From Image: like any UI, you can select an image as start
- Library: realtime generated image seeker, keep all your creatios together in your workspace
- Property panel: select an image in the Library and you can visualize the generation data. From this panel, you can reuse the generation setup clicking in "use this setup", use the selected image as Initial Image by clicking in "use this image" or reveal the file in Windows Explorer by clicking in "show in explorer"
- Quick "use this setup": just double click in a image and it will setup the prompt, quality settings, from image and future features.

### how to install

##### installation
- No need to install, just click Code (green button in the top of this page) -> Download ZIP
- Unzip it in any folder and you are good to go
- Click in plaigroundr.exe

##### requisites:
- The software is developed in native WinForms, this mean that it will work only in Windows.
- You need to install the .Net Core Desktop Runtime -> https://dotnet.microsoft.com/en-us/download/dotnet/3.1
- The AI calculation is very instensive and a good NVidia GPU is required*
- This softwares don't generates the images, it has tools to you organize and help you, it works over the StableDiffusion (aka SD), you will need to have the SD running on your machine.**
 
\* The AI used is StableDiffusion, there is a lot of working around the card graphics requisites, for now, only NVIDIA is compatible. There is some threads that some people is going able to run on AMD, I will try to stay updated and will bring any solutions out there asap.

\** this software was developed and tested using the basujindal optimized script cause I have a GTX 980 and I can't run the oficial release version, but feel free to help me testing and giving me feedbacks, this will help me as a solo developer without the proper equipment.

### configurations
There is a Setup Wizzard window when you open the software. It will guides you to configure your version of StableDiffusion. (see requisites above)
If you close this wizzard, you can click in "Open Wizzard" in the configurations panel at any time.
The wizzard will auto check and will guide you to setup:
- Anaconda/Minicoda (aka Conda): Conda is a python distribution, it creates the environment required by StableDiffusion, as the python dependencies.
- StableDiffusion (aka SD): The IA code, it runs over python, it is open source, created and mantained by HuggingFace (https://huggingface.co/)
- CKPT Model: The brain file, it contains every "neural connection weight" for the whole brain, SD uses this model to generate the images

### Known problems
- libray preview is using full size image, so, if you have a lot of generated images in a workspace, it can take sometime to load (just seconds, but perceptible) - will be fixed
- when generating images using iteration or samples, all these images will have the same initial seed, until I fix this
- I have a GTX 980 and all my tests was using the optmizedSD script, any feedback using other scripts will be really appreciated

### awesome links
- an extensive list of artists: https://f000.backblazeb2.com/file/clip-artists/index.html
