# The Ai Music Generation Challenge 2022

Unlike the previous two editions ([2020](https://boblsturm.github.io/aimusic2020/), [2021](https://github.com/boblsturm/aimusicgenerationchallenge2021)), there are three sub-challenges this year. Participants can compete in any number of these sub-challenges.

## What are the three sub-challenges?

1. Build an artificial system that generates the most plausible _reels_, as judged against the 350 published in F. O’Neill “The Dance Music of Ireland: O’Neill’s 1001” (1907). Up to two prizes will be awarded, and performances of the best ones will occur at some point in both Sweden and Ireland. The panel of judges consists of four (human) experts in Irish traditional music and performance. 
2. Build an artificial judge. This judge must detect plagiarism, analyze the appropriateness of rhythm, mode, and accidentals, and grade the structure and melody, of any given tune (with reference to the 350 reels published in F. O’Neill “The Dance Music of Ireland: O’Neill’s 1001” (1907)). These artificial judges will be applied to the submissions, and their output compared with the responses of the four human judges. The system with the least error in prediction will win an award. (This could also be an output of the system built for challenge 1.)
3. Build an artificial system that generates titles for given tunes. These systems will be applied to reels selected by the judges, who will vote on which titles they believe fit best each tune. (This could also be an output of the system built for challenge 1.)
6. Only one submission from each participant will be allowed in each of the sub-challenges.

## How?
1. By JULY 4, register your intent to participate by notifying the [organizer](mailto:bobs@kth.se?subject=Participation-in-the-Ai-Music-Generation-Challenge-2022), and which sub-challenges you wish to compete in. (At least one and at most three.)
2. Build a system that generates reels, and/or titles tunes, and/or appraises tunes.
3. Write a brief technical document describing how you built your system, presenting some of its features and outcomes, and linking to your code and models for reproducibility.
4. If you are generating tunes, by OCTOBER 7, email the [organizer](mailto:bobs@kth.se):
- a link to download your generated collection of 1000 reels rendered as MIDI **and** in notation (such as ABC, musicXML, or staff), as well as one reel in your collection that you want included in the evaluation (choose what you think is the best).
- a link to download your code.
- a link to download your technical document (pdf)
5. If you are appraising or titling tunes, you will receive a set of tunes from the submitted collections sometime after OCTOBER 7.

## Tune Evaluation
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
6. _Stage 3_ Each judge will present to the other judges the best tunes from their collections, and together will decide which deserve recognition (or to award no prize).

## Artificial Judge Evaluation
The evaluation of artificial judges will proceed in the following way:
1. Each artificial judge will perform the first two stages of evaluation for a selection of submitted tunes.
- Stage 1: rejection based on plagiarism, rhythm and mode/accidentals.
- Stage 2: scoring of the remaining tunes along structure and melody (graded on a scale 1, 2, 3, 4, 5) where 1 is poor.
2. The ranking of the artificial judges will be done by the organizers by comparing AI judge outputs with those of the real judges in each stage. 
3. To measure the differences between real and AI judges in stage 1 we will count coincident rejections of all judges.
4. To measure the differences between real and AI judges in stage 2, we will compute a mean minimum absolute difference of scores for non-rejected tunes. 
5. There will be baseline computational judges, such as “reject all”, “score all as 3”, and "randomly reject or score”.

## Title Evaluation
The evaluation of tune-titling systems will proceed in the following way:
1. Each tune titler will title a selection of submitted tunes.
2. Titles of tunes achieving high scores in Stage 2 will be submitted to human judges for ranking.
3. Highest ranked titles will be awarded prizes.

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

# Results of Sub-challenge 1: Reel Generation

Below are the scores of the four judges for the five systems (including the benchmark). Team names are counties in Ireland. Each tune number highlighted red is the one identified by the participant to be included in the evaluation. Nine others were selected at random. A "P" in the "Stage 1" column denotes a judge rejecting a tune due to plagiarism. A "R" denotes rejection by rhythm; and an "M" denotes rejection by mode or accidentals. Scores in the columns "Structure" and "Melody" are on a scale of 1 - 5, with 5 being the best. Green highlighting denotes election by a judge for consideration of an award.

<img width="462" alt="AIMGC2022scores" src="https://user-images.githubusercontent.com/10271332/218058586-fbd7fb44-b1e8-4a4c-abcf-a934610a62c6.png">

Based on the stage 3 discussion, the *first prize* award is given to Tune 507 from team Clare:

<img width="1050" alt="Reel507Clare" src="https://user-images.githubusercontent.com/10271332/218059799-322c5f8c-9258-4a88-8b76-856c5a1110e7.png">

Judges remark: "Easy to remember, easy to follow and catch; uplifting, bright and fun to dance to"; "Excellent! Everything right! That's a 5+. Not plagiarised as far as I can see (I suspected it might be since it was so good)"; "Very simple reel, but adheres to all the variables regarding reel structure. Great Rhythm. Makes good use of repetition. Very simple but consistent and phrases are easy to remember. Excellent simple reel that sits well with the tradition."

The *second prize* award is shared: tune 267 from team Limerick and tune 979 from team Kerry:

<img width="1058" alt="Reel267Limerick" src="https://user-images.githubusercontent.com/10271332/218060328-f2080c7f-40ab-4efb-a5d3-96141bbfdce4.png">

Judges remark on 267: "Perfect in structure. Great natural rhythms. Beautiful melody; a fantastic tune. A tune I'd be happy to play. Well done!"; "Interesting. Nice changes c#/c"; "Has all the correct structure. Nice minor."

<img width="1058" alt="Reel979Kerry" src="https://user-images.githubusercontent.com/10271332/218060368-f4a60770-2d03-4b73-ba50-f2ad9bd80bc9.png">

Judges remark on 979: "Good tune"; "Structurally sound in every way. Easy to play and always has the feel of a reel when played. Good melody. Good use of repetition. Plays well on accordion and worth learning. Good tune. Phrases are strong and stand out. Melody definitely belongs in the tradition."

# Results of Sub-challenge 2: AI Judge

Shown below are the results of three AI judges:

<img width="715" alt="Screen Shot 2023-02-25 at 12 34 07" src="https://user-images.githubusercontent.com/10271332/221354684-a7120321-5139-449d-a759-5faac2a1d1b2.png">


One system was submitted by team Clare, which is compared against two benchmarks: 
1) Benchmark 1 detects for plagiarism. If the candidate tune is not deemed plagiarised, and its metric structure exists in O'Neill's, then both Structure and Melody are rated 3; otherwise these are both rated 1.
2) Benchmark 2 detects for plagiarism. If the candidate tune is not deemed plagiarised, then a random number is drawn from {1,2,3,4,5} and assigned to both Structure and Melody.

Of the 50 tunes evaluated by the human judges, two were deemed to be plagiarised. All three AI judges detected only one of these, giving each a plagiarism true positive (PTP) and plagiarism false negative (PFN) of 1. Both benchmark judges have 1 plagiarism false positive (PFP), while Clare has none. None of the benchmark AI judges was designed to reject based on meter or accidentals so their rhythm true positives (RTP) amd rhythm false positives (RFP) are zero. Clare however has 5 RTPs, 3 RFPs. Clearly, Clare is the more sensitive AI judge of the three. 

For Stage 2, we compute for Structure (S) and Melody (M), the minumum absolute error with the scores of the human judges. This if the four human judges rate a tune in a category as (2, 3, 4, 5) and the AI judge rates it a 1, then the minumum absolute difference is |2-1| = 1. In the Structure category across tunes passing its Stage 1 (47 of 50), Benchmark 1 has a mean minumum absolute error of 0.766. For Melody, this is 0.426. The mean of these is 0.596. These are all larger for Benchmark 2. The performance of Clare in its tunes passing Stage 1 (40 of 50) is clearly the best, with a mean minumum absolute error of 0.488.

# Results of Sub-challenge 3: Tune Titling

All tunes elected by the judges were given titles and assessed by the judges. Two systems competed against a human (Sturm):
- Team Clare (C)
- Benchmark (B)
- Human (H)

The human titles were given to each tune before looking at the generated titles. Titles produced by the benchmark were created by querying a large language model prompted to generate titles for Irish traditional dance tunes, and then selecting at random from the large text file created.

For each tune, judges discussed the three titles, and either voted for their favorite(s), voted against some of them, noted plagiarism, or declined to vote. In general they found this entertaining, but noted that some titles were plagiarised (e.g., "Miss Sarah Drummond Of Perth" by C), a few were problematic with negative connotations ("The Changelings" by C, which references an Irish myth about fairies stealing healthy babies and replacing them with unhealthy babies; and "The Orange Brothers' Liberty Club" by B), and some titles were just weird (e.g., "The Great Flax By Your Side" by B, and "The Most Perfect Thing A Man Has Ever Been Told, Part III" by B).

Here are the results summarized, with numbers showing in favor, "-" for marks against, and "P" for plagiarised:

- 15: B(-), H(1) -> winner H "Shannon River Reel"
- 24: C(-), B(-) -> winner H "Money in the Pocket"
- 241: H(1) -> winner H "The Happy Dentist"
- 267: B(-), H(1) -> winner H "Finbarr’s Fancy"
- 428: H(4) -> winner H "Tenement Dance"
- 507: B(-), C(-), H(1) -> winner H "A winter in Cavan" (though there was some dissension in forcing this title onto the 1st place tune)
- 642: C(P), B(-), H(1) -> winner H "O’Connell meets the Queen"
- 646: H(4) -> winner H "A steamer to America"
- 895: H(2), C(P), B(-) -> winner H "The wind today is fair for sailing"
- 920: H(3), C(1) -> winner H "Road to Ballymahon"
- 979: C(P), H(4) -> winner H "Pheasant’s Dance"

The clear winner for each tune is H. Team Clare got one vote in favor and two votes against, but also reproduced three titles verbatim. The benchmark did not perform well at all.
