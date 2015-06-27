## Updates [06/27/2015]
> We have Docker and Vagrant images working locally.
> We are now wrapping up everything and will update the documentation accrodingly. 
> Couple more weeks and we should have a usable product

# What is Cloud Transcode ?
Cloud Transcode is a custom distributed transcoding stack using Amazon AWS services.

The goal of this project is to create an open source, scalable and cheap distributed transcoding platform where users have complete control over
performance and cost. 

We start with video transcoding which is the most costly, but the goal is to transcode any media (audio, documents and images). We use FFMpeg for video transcoding.

Today's commercial solutions for video transcoding are very expensive for large volumes. With this solution you can transcode large quantity of videos at the pace you want, thus controling your cost. 

With Cloud Transcode, you control: scale, speed and cost. You can run everything locally if you want, no Cloud instance required. You only need an Amazon AWS account and an Internet connection to use the required Amazon services: SWF, SQS and S3. 

It means that you can have a local, hybrid or full cloud setup on Amazon Ec2 instances, it's up to you.

# Transcoding supported
- **Video to Video transcoding**: One video IN, many videos OUT. Any formats and codecs supported by your ffmpeg.
- **Video to Thumbnails transcoding**: Snapshot at certain time in video or intervals snapshot every N seconds.
- **Watermark integration in video**: Take image IN and position a watermark on top of the video. Custom position and transparency.

# High Level Architecture
![Alt text](/../images/high_level_arch.png?raw=true "High Level Architecture")

# Quick start with Vagrant
A Vagrant box (Virtual Machine) which provides pre-configured environment to run the stack has been created to help you test the stack and work on it. You can use Vagrant on any OS and quickly bootstrap.

See: https://sportarchive.hackpad.com/Cloud-Transcode-project-poG8vKTC16J#:h=Quick-start-with-Vagrant

# Deep dive
Find the detailed documentation here: https://sportarchive.hackpad.com/Cloud-Transcode-project-poG8vKTC16J

# Task tracking
Check the project status and tasks in the pipe on Pivotal Tracker:
- https://www.pivotaltracker.com/n/projects/1044000

# FFMpeg performance benchmark on Amazon EC2
Download the spreadsheet to compare the different Amazon EC2 instances cost and performances:
https://github.com/sportarchive/CloudTranscode/blob/master/benchmark/benchmark-aws-ffmpeg.xlsx

