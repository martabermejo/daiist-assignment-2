# Assignment 2 Report

- **Name**: Marta Bermejo Villaescusa
- **Student ID**: 18748
- **Email**:mbermejo.ieu2022@student.ie.edu
- **Group**: BBADBA 5B 

## Business problem, and the cost of being wrong

The townhall of a city has to make decisions on where to send employees to make repairs, and what streets to prioritize, which ones to improve. My idea would be that some cars will be driving around with cameras, and by analyzing the potholes and streets that are in bad shape, they send a technical maintenance team to fix what needs to be fixed. 
A false negative would be a real pothole that no one fixes, because it is not identified or found, which leads to the pothole becoming bigger, a bigger issue, harms vehicles, and becomes a more expensive issue and more difficult to fix. A false positive would be sending a repair team to a place that does not need fixing, causing the cost of opportunity of them going somwehere else, and the cost of moving to there, but does not generate any harm in itself. There would be more harm in false negatives, as they generate actual harm and certainly bigger expenses. As an estimate, I believe a false positive would be a cost of around 150 euros, because of being one hour of work of 3 workers, plus oil. For false negatives I assume a cost of 1000 Euros, because I have looked at costs of fixing potholes which is around 400 Euros, and took into account that if it grows it becomes bigger and there is the part of claims from citizens, which makes me think that 1000 is realistic.  

## Dataset
I found the dataset in roboflow, about road damage detection, from an author called firas. Theworkspace is firas, the project road-damage-detection-cu86 and it is the version 2. The classes are crack, pothole, and manhole. This version has around 2000 images. One image is a frame of the road taken from inside of a vehicle, with objects appearing as bounding boxes around a feature of the road. The potholes are what I want to focus on, cracks is a different surface damaged, and manholes are key because they can look like a pothole but they need no repair. 
This dataset serves my problem because my decision is whether to send a repair team to a segment of road using videos from vehicles that already are out there. This dataset matches that idea, as it contains pothole as the positive class and has manhole to serve as a potential false positive cause. 
The link for the dataset is this one:
https://universe.roboflow.com/firas/road-damage-detection-cu846


## What the dataset's composition implies

*Instances per class, train/val/test sizes, typical object size relative to the
image. Then the interpretation: which per-class numbers will be too thin to
trust, whether the test split resembles the images you'd really see, and what
you therefore can't conclude from your results.*

## Finetuning and baselines

*Which model and task (detection or classification) and why. A results table on
the same test split: your finetuned model, the pretrained COCO model zero-shot,
and a trivial baseline. What changed, and whether the gap is as large as you
expected.*

## Per-class evaluation and failure modes

*Per-class AP50, or per-class precision/recall and the confusion matrix.
Which class carries the headline number, which one is dragging, and what the
model actually confuses with what. Show where it breaks, not just that it
works.*

## Cost matrix and operating point

*Your euro cost for each kind of error and where each figure came from. The
base rate you assumed. The cost-against-threshold sweep, and the operating
point you chose. State the assumption that would most change your answer if it
were wrong.*

## What a person still has to check

*Your two thresholds, and what share of cases they send to a person. How many
that is per day, how long one takes to check, and how many people that needs.
Is that realistic? Then your design priced against the three alternatives:
doing nothing, having a person check everything, and letting the model decide
on its own.*

## Limitations & next steps

*Real limitations you found, and concretely how you'd address each one with
more time or data. Not generic hedging.*

## Generative AI use disclosure

*Per the syllabus AI Policy: what you used and how, or "no AI content used."*
