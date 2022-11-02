# OutOfTheBlue

Winner Project of HackZurich for the "4D buildings" challenge by Siemens

![This is us winning](https://github.com/hackzurich-2022/OutOfTheBlue/blob/main/ClosingCeremony_HackZurich-24%20(2).jpg)

## Inspiration

Software can make people's life easier, but sometimes it can even save their lives. 
We wanted to do both! 
We were trying to find a helpful interface for fire fighters in real live scenarios based digital data and visualization.

## What it does

Out of the Blue is a versatile tool that allows anyone to obtain a detailed 4D model based on a 2D blueprint, unlocking a set of new services that vary from creating a perfect digital twin of the house (that supports smart automated routines to reduce risks) to an optimized instrument for crisis containment which could be a keystone tool into the daily work of firefighters.

## How we built it

Out of the Blue grants a fully automated process that can start from any blueprint and generate a precise, multi level, three dimensional model. These are the main steps that characterize the generation pipeline:
Noise Reduction: Files might be from different sources (pdf, png, jpgs) and might contain different information (schematics, notes…), that’s the reason why the first step is to remove all the unwanted data/lines/text that would impact on the final output of the model.
Image interpolation: With the help of a python library, all the schematics are converted into a 3D Blender model that tries to maximize the alignment and the scaling of the building’s floors.
Smooth Transition: As soon as all the modeling is done, the software exports the file as a .fbx and imports it into the application ready to be used.
In Unity, we again smothen and filter the model and then we visualize the environment based on the occurences.

## Challenges we ran into

Obtaining a 3D model from PDFs has revealed to be tougher than we thought. There are many things that must be considered and we had to do a lot of preprocessing to remove noise, such as the furniture or text that were wrongly interpreted. Our code now even works for multiple floors! 

Another challenge has been to make the fire propagate in a realistic way, following natural restrictions.

## Accomplishments that we're proud of

We are very proud of our automated pipeline (from paper to 4D model), the work we managed to do within 2 days and even though we ran in many problems, we didn't give up and managed to accomplish our goal.

## What we learned

We have learned to work in an international environment with different people from different nationalities. We have learned to hear different mindsets and work under time pressure to meet the deadlines and follow a structured work division.
We have learned to know Zurich, through the city but mostly through the Technopark. 

## What's next for out of the blue

Next would be to implement full AR/VR experiences. 
And test it out in  areal time scenario with real time sensor data
