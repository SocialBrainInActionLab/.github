# Social Brain in Action Lab

Github organization for the [Social Brain in Action Lab](https://www.soba-lab.com/).

In this document, you will find links to all relevant code repositories used for different
experiments.

# Organizations

We currently have multiple Github organizations used to compile repositories relevant to different
topics.
Depending on your project, you might be required to join one or more of these organizations:

- [Social Brain in Action Lab](https://github.com/SocialBrainInActionLab)
- [Cozmo Game 4 Sobot](https://github.com/CozmoGame4Sobot)
- [Nao Pepper 4 hri](https://github.com/NaoPepper4hri)

# Relevant projects

Some of our code might not belong to our organisations, and are stored under a different account
(e.g., the account of the author).
This list contains references to the relevant repositories for each project in the lab, so we can
keep track of them.

## Reading with Robots

The Reading with Robots project aims to study the efficiency of robots as support for teachers in
engaging children with reading.

The program required to run this project requires two main components:

- [Reading To Robot Web App](https://github.com/SocialBrainInActionLab/readingtorobot_app)
- [Reading To Robot Python package](https://github.com/chaudhuryB/ReadingToRobot)

In the experiments performed, we created a webapp that works as control centre for the robots, as
well as questionaire.
The experimenter can access this app and use it to provide questions to the children during the
experiment, and start and control the robots when required.
In order for the robots to work, the webapp server starts the robot processes defined in the
reading to robot python package.

## Embodied Support Robots

This project focus on the study of the effects of embodiment in people's subjective experience.
We use Pepper as a support agent in a speech learning task.
The experiment has two variants, used to explore the effects of embodiement in the task:
executing the learning task with the robot in the same room, and communicating with the robot using
Zoom (virtual interaction).

The code for this experiment is divided in two repositories:

- [Speech Learning Web App](https://github.com/NaoPepper4hri/speech-learning):
  Main webapp including the learning exercise for the participant and a Wizard of Oz control page
  for the experimenter.
- [Pepper Base](https://github.com/NaoPepper4hri/PepperBase):
  An android app that allows executing specific actions in pepper remotely.

The web app is the core of the experiment.
The server side of the app takes care of connecting the front end (web browser) with Pepper.
This allows us to execute actions with the robot in the right moment.
The Pepper Base app works as a passive endpoint for this communication, but is required in order for
the robot to respond to the webapp commands.

## Other tools and relevant repositories:

- [Virtual environment for NAO](https://github.com/NaoPepper4hri/nao_virtualenv):
  Install a python virtual environment in the NAO robot to allow manually installing python
  packages without need for root access.
- [Pepper Base](https://github.com/NaoPepper4hri/PepperBase):
  Template project for Android applications for the Pepper robot.
  You can use this as an example for any new application you make, or add new functionalities to the
  template.
- [Heartbot](https://github.com/SocialBrainInActionLab/Heartbot):
  Synchronize user heartbeat to robot light pulse.
- [NaoPupper](https://github.com/NaoPepper4hri/NaoPuppet):
  Use Kinect V1 to mimic human arm movements on NAO.
- [Synchronised Movement With Pepper](https://github.com/NaoPepper4hri/SynchronisedWithPepper):
  Used on drawing synchronization task with Pepper.
- [WizOfOz Chat](https://github.com/NaoPepper4hri/WizOfOz_Chat):
  A html page based wizard of oz application to control what Nao or Pepper says using Flask.
- [Prisonners Dilemma Experiment](https://github.com/CozmoGame4Sobot/Prisonners-Dilemma-Experiment):
  Prisoners Dilemma with Tit-for-Tat and Random strategy with an angry or sad Cozmo.
- [QuickTap Game With Set Emotion](https://github.com/CozmoGame4Sobot/QuickTapWithSetEmotion):
  The QuickTap game from Cozmo, but with custom reactions.

# Contributing

You will most likely contribute to the lab with your own project.
This means that it will be up to you how you manage your code and repositories, however, you might
need to make changes to an existing repository, or you might want to add a link to your code or
project documentation here so other people can benefit from it.
If you would like to contribute to an existing repository, please follow these simple steps:

1. Fork the base repository:
   you should create a fork of the original repository to make changes as you see fit before
   appying the final version to the original.
2. Make any changes you want/require.
3. Create a pull request (also known as PR) to the original repository.

Once you have created a PR, anyone with administrative rights to the original repository can review
your changes, ask for clarifications or changes to your code and finally approve and apply those
changes in the original repo (Merge the PR).

# Licensing

Generally, all the code in the lab should be licensed under GPLv3 (GNU General Public License v3.0).
When you create a new code repository for your work with the lab, you should license it under GPLv3.
Please check with your supervisor if you would like to use a different license for your project.

You can add the license when creating the repository, or before making it public.
