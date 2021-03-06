# The Ai Music Generation Challenge 2022

Unlike the previous two editions ([2020](https://boblsturm.github.io/aimusic2020/),[2021](https://github.com/boblsturm/aimusicgenerationchallenge2021)), there are three sub-challenges this year! Participants can compete in any number of these sub-challenges.

## What are the three subchallenges?

1. Build an artificial system that generates the most plausible _reels_, as judged against the 350 published in F. O’Neill “The Dance Music of Ireland: O’Neill’s 1001” (1907). Up to two prizes will be awarded, and performances of the best ones will occur at some point 2022 in both Sweden and Ireland. The panel of judges consists of four (human) experts in Irish traditional music and performance. 
2. Build an artificial judge. This judge must detect plagiarism, analyze the appropriateness of rhythm, mode, and accidentals, and grade the structure and melody, of any given tune (with reference to the 350 reels published in F. O’Neill “The Dance Music of Ireland: O’Neill’s 1001” (1907)). These artificial judges will be applied to the submissions, and their output compared with the responses of the four human judges. The system with the least error in prediction will win an award. (This could also be an output of the system built for challenge 1.)
3. Build an artificial system that generates titles for given tunes. These systems will be applied to reels selected by the judges, who will vote on which titles they believe fit best each tune. (This could also be an output of the system built for challenge 1.)

## How?
1. By JULY 4, register your intent to participate by notifying the [organizer](mailto:bobs@kth.se?subject=Participation-in-the-Ai-Music-Generation-Challenge-2022), and which sub-challenges you wish to compete in. (At least one and at most three.)
2. Build a system that generates reels, and/or titles tunes, and/or appraises tunes.
3. Write a brief technical document describing how you built your system, presenting some of its features and outcomes, and linking to your code and models for reproducibility.
4. By OCTOBER 7, email the [organizer](mailto:bobs@kth.se):
- if you are generating tunes, a link to download your generated collection of 1000 reels rendered as MIDI **and** in notation (such as ABC, musicXML, or staff), as well as one reel in your collection that you want included in the evaluation (choose what you think is the best).
- a link to download your code.
- a link to download your technical document (pdf)
6. Only one submission from each participant will be allowed in each of the sub-challenges.

## Evaluation
The evaluation of submitted tune collections will proceed in the following way:
1. From each submitted collection, one tune is selected by the participant of the collection, and a number of others are selected at random.
3. All selected tunes are sent to all judges for review.
4. _Stage 1_ Each judge reviews the acceptability of each tune according to the following:
- If plagiarism detected, reject and do not review.
- If rhythm is not characteristic of a reel, reject and do not review.
- If mode and accidentals are not characteristic of a reel, reject and do not review.
5. _Stage 2_ Each judge will rate on a scale of 1–5 the acceptable tunes along the following qualities:
- Structure
- Melody
6. _Stage 3_ Each judge will present to the other judges the best tunes from their collections, and together will decide which are the best reel (or to award no prize).

The evaluation of tune-titling systems and artificial judges will be announced later. 

## Why?
This challenge has three aims:
1. to promote meaningful approaches to evaluating music Ai;
2. to see how music Ai research can benefit from traditional music, and how traditional music can benefit from music Ai research;
3. to facilitate discussions about the ethics of music Ai research applied to traditional music practices.

## Frequently Asked Questions
1. "Where can I get data?" The 350 reels in O'Neill's 1001 are tunes 456-805 available [here](http://john-chambers.us/~jc/music/book/ONeills/1001/).
2. "How is this challenge funded?" The 2022 challenge is part of a project that has received funding from the European Research Council (ERC) under the European Union’s Horizon 2020 research and innovation programme (Grant agreement No. 864189 [MUSAiC: Music at the Frontiers of Artificial Creativity and Criticism](https://www.kth.se/is/tmh/speech-communication/musaic-music-at-the-frontiers-of-artificial-creativity-and-criticism-1.950539)).
3. "What happened with the 2020 challenge?"
- See a video of the [2020 challenge](https://youtu.be/KSoSyoEx6hc), where the focus was on the 365 jigs in O'Neill's 1001.
- Read more about the challenge in [Sturm & Maruri-Aguilar (2021) “The Ai Music Generation Challenge 2020: Double Jigs in the Style of O'Neill's 1001''”, Journal of Creative Music Systems. 5(1).](https://doi.org/10.5920/jcms.950)
4. "What happened with the 2021 challenge?" Awards are mentioned [here](https://github.com/boblsturm/aimusicgenerationchallenge2021)

