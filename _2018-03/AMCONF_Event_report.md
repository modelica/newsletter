---
title: Report from the American Modelica Conference 2018
author: "Luigi Vanfretti ([Rensselaer Polytechnic Institute, Troy, NY, USA](https://alsetlab.github.io/))"
category: "conference"
---

# The new world opens to Modelica: Highlights from the very first **American Modelica Conference 2018!**

![American Modelica Conference 2018](AMCONF_2018.png 'American Modelica Conference 2018')

## Thanks!

The very first
[American Modelica Conference](https://www.modelica.org/events/modelica2018Americas), was
held in Cambridge, MA, USA on October 9-10, 2018. The conference had 2 keynotes, 36 papers, 11 exhibitors and almost 100 attendees, among which 59 regular attendees, 15 students, 2 keynote speakers, and ~20 vendor representatives.

Having the honor of being the Program Chair, I am delighted to inform that the event was an outstanding success in every aspect. I do not want to list everyone involved in making this a success to avoid the risk of missing someone, so I would like to personally thank everyone involved in the conference and most importantly, our conference presenters, for sharing with the Modelica community about their exciting research and projects! It goes without saying that I had a wonderful time meeting old friends and meeting new colleagues.

As the Modelica community grows in the USA and North America, I am very hopeful that we will be able to replicate and synchronize with what makes the Modelica community unique - a truly open, welcoming, and above all, ** super cool ** technical collective of modeling and simulation experts that through its efforts it is making true impact in different domains crucial for today's society. With the substantial challenges that the future holds for our world, the Modelica ecosystem and community is positioning itself as vital set of technologies and experts that can enable and inspire people to address these challenges.

Below, I have tried to provide you with some of the highlights of the event, from my perspective; hoping to encourage you to join us in the next edition of this event in this "new world" for Modelica.

## Warm up!
As one of the traditional highlights of Modelica conferences for participants, this conference included three "pre-conference" workshops, organized on October 8th.

At Mitsubishi Electric Research Laboratories, two sequential workshops took place. In the morning workshop, Modelon provided an "Introduction to Modeling with Modelica" workshop, where more than 20 participants from industry and academia learn about the basics of Modelica with a web browser-based tool being developed by Modelon. Next, Michael Wetter of LBNL gave a workshop on "Thermo-fluid Modeling with Applications from the Buildings Library," which made use of the aforementioned tool, and with more than 20 participants also; who learned the basics of the Buildings' library, best practices in developing models using it, and built several models of their own. The participants, including this reporter and his students, found both workshops informative and very useful for their future research.

As a personal highlight, I had the pleasure of having lunch with "il Padrino", Hilding Elmqvist, during the lunch break of this workshop. It was of course a great moment for someone like me that only joined the Modelica community 7 years ago, and I truly enjoyed discussing with Hilding about the enabling features of Modelica for cyber-physical system modeling. More on that below.

Concurrently, Jiri Kofranek's team from Charles University offered a 1 day workshop on "Introduction to Equation Based Modeling and Simulation with Modelica with a Focus on Physiological Modeling." This workshop was possible thanks to Michael Tiller's efforts and aimed at exposing physiology experts to Modelica and the dedicated libraries from Charles University developed for this purpose. Participants learned how to model the cardiovascular system dynamics using principles from the hydraulics domain, among other interesting applications!

## The Main Event!
We had the pleasure of having two amazing keynotes from two unique perspectives.

The first keynote was given by Dr. John F. Mckibben of Proctor and Gamble on "Simulation Led Innovation at Proter & Gamble". P&G is one of America's major source of "consumer packaged goods", think about toiletries, shampoo, and yes, toilet paper!
The talk was an exciting expose of how simulation is enabling massive innovation possibilities with lower costs as compared to previous conventional prototyping approaches. Most importantly, Dr. Mckibben made a case that beyond mastering technology, to truly take advantage of modeling & simulation approaches, any business will need to change their mindset: the entire life cycle of digital assets (our models and simulators), needs to become as important of the physical assets. This aspect really struck a chord with me, as the world continues with the trend of digitalization - from smart homes to smart grids -, our "digital twins" will become a crucial part of our society, and as one of the world's premier community of modeling and simulation experts, bringing this message out is an important role we can play.

The second keynote was given by Dr. Hilding Elmqvist, CEO of Mogram AB, and most importantly, the pioneer of Modelica. The talk "Modelica - History, State, Needs, Trends, and Possibilities" was an entire educational experience of its own. From the early challenges that Dr. Elmqvist faced with limited hardware, to the **universe of opportunities** that can be enabled with Modelica technologies, this talk made me learn, think and even laugh! To illustrate the point of evolution of the technology and current needs (i.e. self-driving cars), Dr. Elmqvist showed how he used a web-based tool to develop a Modelica model while letting his Tesla drive for him in the road; luckily, this was not illegal in Sweden when he recorded it!
This really made me ponder on how **digital assets, physical systems, and humans** are becoming more interweaved, and how now, more than ever, the technologies of the Modelica ecosystem have a crucial role to play. To this point, Dr. Elmqvist illustrated the importance of making Modelica evolve through prototyping languages, such as Modia, to expand simulation standards to take advantage of Virtual and Augmented Reality (AR/VR), and other visions where modeling and simulation can help meeting the challenges today and the future.

![Elmqvist Vision](amconf_03.png 'Elmqvist Vision')

Finally, something that is really important for me as a Professor, was the topic of low-cost HIL simulation. Dr. Elmqvist showed a low-cost prototype HIL system with the controller on an Raspberry Pi and the model on a PC, to highlight that the available technologies today for HIL are now opening new opportunities. I loved this kind of "toy" examples because not only I work with real-time HIL simulation at [ALSETLab](https://alsetlab.github.io/lab/) and I want the models I run in my targets to one day be portable, but more importantly because they can truly help bringing more people young to the Modelica world, specially young students. I really hope Dr. Elmqvist will continue this effort, it can make my job as an educator much better, and help foster the future Modelica generations.

![RPi](amconf_01.png 'RPi')

## A Glimpse into the Conference Papers: My Top 3 Pics!
With nothing else than my own biased selection, I present to you some of my favorite papers during the conference, along with my own **Guerilla-style** photography, ;-)

### 1. A Total Eclipse of The Heart - On Mobile Now!
My dear friends of Charles University don't stop surprising me every Modelica conference!

In this conference, Filip Ježek (shown in action below) presented their work using Modelica to publish and share biomedical models. I don't need to emphasize how meaningful this work is, but I would like to show you how cool it is!

![Filip](amconf_02.png 'Filip')

Take a look at a heart model on your mobile phone running on an FMU, [here](http://physiomodelling.com/mobile.html), or if you are sitting on your PC, open your browser and learn how circulation is affected by weight, height, and other factors [here](http://physiomodelling.com/circulation/). You can find the full presentation [here](https://github.com/ALSETLab/2018_American_Modelica_Conference/raw/master/FullPaper/Modelica2018US_Presentations_21.pdf)

![Circulation](amconf_01.gif 'Circulation')

### 2. Born in the USA - There's nothing cooler than DLM!
Have you ever heard of Dirt Late Model cars?

Me neither, but they are cool! Nothing more fitting for the 1st American Conference than a truly American sport!

Check out this amazing application of Modelica by Nate Horn of Claytex on developing Dirt Late Model car models and simulations [here](https://github.com/ALSETLab/2018_American_Modelica_Conference/blob/master/FullPaper/Modelica2018US_Presentations_27.pdf).

![DLM](amconf_02.gif 'DLM')

### 3. Too Hot! - In space?!
Tobias Posilek presented his work on "A Modelica Library for Spacecraft Thermal Analysis". I'm a big fan of the work of DLR, and this library is an exceptional sample of their amazing work.

The library allows the simulation of the complete spacecraft system (thermal system, electric and mechanical), system solar angles, the form factor and a shadow function. Check out the slides [here](https://github.com/ALSETLab/2018_American_Modelica_Conference/blob/master/FullPaper/Modelica2018US_Presentations_24.pdf).

![DLR](amconf_03.gif 'DLR')

## More Coming Soon!

### Where's the proceedings?
Along with Christopher Laughman of MERL, we are putting together the conference proceedings which should be available in the coming month.

### Repository with Presentations
For those that can't wait to enjoy the fun, for the time being, an unofficial draft of a repository (which will be transferred to the Modelica Association upon completion) is available [here](https://github.com/ALSETLab/2018_American_Modelica_Conference).

## See you next time!
I hope you enjoyed reading this report, and I encourage you to join us in the next edition of this event in this "new world" for Modelica - I will personally be very happy to see so many of my colleagues in Europe more often!

Thanksgiving Day of 2018-11-22.

Dr. Luigi Vanfretti,
Associate Professor, [ALSETLab](http://alsetlab.com),
[ECSE Department](https://ecse.rpi.edu),
[RPI](http://www.rpi.edu), Troy, NY, USA
