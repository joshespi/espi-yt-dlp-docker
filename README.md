# espi-yt-dlp-docker
simple dockerized version of yt-dlp. 

To use the yt-dlp-docker container, follow these steps:

Open a terminal or command prompt and navigate to the yt-dlp-docker directory.

Build the Docker image by running the following command:
```docker build -t yt-dlp-image .```

Invoke the  script with bash
```bash scrape_yt.sh```
This will prompt you for a YouTube link and download the video into the ~/yt-downloads directory. (Note: This has only been tested on Ubuntu.)

If you want to simplify the execution of the  script, you can create an alias or function in your shell configuration file (e.g., bashrc, .zshrc) to run the script with a single command. Follow these steps:

Open your shell configuration file with a text editor (e.g., nano ~/.bashrc).

Add an alias or function definition to the file. Here are examples of both options:

Alias example:
```
alias yt-dlp="/bin/bash /home/joshe/docker/espi-yt-dlp-docker/scrape_yt.sh"
```

Replace /path/to/download_youtube.sh with the actual path to your  script.

Save the changes to the file and exit the text editor.

Reload the shell configuration file to apply the changes:
```source ~/.bashrc```
Now, you can execute the script using the defined alias or function. For example:```yt-dlp```

This allows you to run the download_youtube command in your terminal, and it will automatically execute the  script, prompting you for the YouTube link and initiating the download.

Remember to adjust the alias or function name to your preference.