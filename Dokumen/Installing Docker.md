# Installing Docker: The Fast Way

## Installing Docker, Kubernetes, and a text editor

If you don't already have Docker installed, Docker already has some [great guides on how to do it](https://docs.docker.com/get-docker/), but if you already know which OS you want to install on, below are quick steps for downloading it. The videos after this Lecture are walkthroughs of installing Docker for each OS, then getting the GitHub repo, getting a code editor, and tweaking the command line if you want to. **Feel free to skip any of this Section if you have Docker Desktop and Visual Studio Code already installed.**

**I always recommend** [Visual Studio Code (vscode) as your editor](https://code.visualstudio.com/) for all things Docker, Kubernetes, and DevOps. It's free for all OSs and has plugins to help you with many tools in this course.

## Installing on Windows 10 and Windows 11 (any Edition)
https://docs.docker.com/desktop/windows/install/

This is the best experience on Windows, which [uses WSL2](https://learn.microsoft.com/en-us/windows/wsl/install). If you're new to WSL2, it's the best way to run Linux on Windows, and Docker Desktop will walk you through enabling it. Docker can technically still work on Hyper-V with "Windows Containers," but most of this course focuses on Linux Containers, which WSL2 is great at.

After installing [Docker Desktop for Windows](https://docs.docker.com/desktop/install/windows-install/). I recommend installing a Windows Store [Ubuntu for WSL2](https://apps.microsoft.com/store/detail/ubuntu/9PDXGNCFSCZV?hl=en-us&gl=us&rtc=1&activetab=pivot%3Aoverviewtab) distro and using its shell in [Windows Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701?hl=en-us&gl=us) is the best CLI experience! Make sure to check your Docker Desktop settings to give it enough resources and enable all your WSL2 distros for Docker Desktop.

## Installing on Windows 7 or Windows 8

Unfortunately, Microsoft's OS features for Docker Desktop don't work in these older versions. You'll need to use Hyper-V or install VirtualBox and manually setup a Linux VM. It's more involved than the other options, so I often recommend the easier option: using a DigitalOcean cloud server with my coupon code https://m.do.co/c/b813dfcad8d4 gets you $100 in credits over 60 days.

## Installing on Mac
https://docs.docker.com/desktop/mac/install/

You'll want to install Docker Desktop for Mac, which is great.

## Installing on Linux Desktop
**2022 update**: Docker Desktop for Linux is here!

https://docs.docker.com/desktop/linux/install/

## Installing on Linux Server
https://docs.docker.com/engine/install/

**Do *not* use your built-in default packages**  **```apt/yum install docker.io```**  because those packages are old and not the Official Docker-Built packages. 

I prefer to use [Docker's automated script](https://get.docker.com/) to add their repository and install all dependencies: ```curl -sSL https://get.docker.com/ | sh``` but you can also install in a more manual method by following specific instructions that Docker provides [for your Linux distribution.](https://docs.docker.com/engine/install/)

## Use Play With Docker
https://labs.play-with-docker.com/

Maybe you don't have local admin, or maybe your machine doesn't have enough resources. Well, the best free option here is to use [play-with-docker.com](https://labs.play-with-docker.com/), which will run one or more Docker instances inside your browser, and give you a terminal to use it with. You can create multiple machines on it and even use the URL to share the session with others in a sort of collaborative experience.  I highly recommend you check it out.  Most of the lectures in this course can be used with "PWD," but the **big limitation is it'll reset after 4 hours, at which time it'll delete your servers.**

## Use DigitalOcean as a remote Linux Server
If you signup for a new account with DigitalOcean, my favorite "simpler" cloud, you can use a smaller server for months with my signup credit. **Install Docker in the Cloud, via the above Linux links, and do the course without needing Docker locally.**
Thousands of students have done this: 

https://m.do.co/c/b813dfcad8d4 gets you $100 in credits over 60 days