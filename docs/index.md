# SCORIA: International Thesis Supervision & Open-Source Collaboration

---
## Scorification
Music scorification is the process to get from a symbolic MIDI recording to a readable score, that is, to estimate the quantization of onsets and offsets into musical time and to estimate meter, key, voice, and several more attributes. Scorification is a hard technical problem for which no satisfactory solutions exist yet.

## About the Project
We aim to create a complete pipeline to automatically and beautifully typeset scores from recorded MIDI data. This is a huge undertaking encompassing many music information retrieval tasks. To make it manageable, we break this goal down into challenging subtasks, each addressed in its own thesis.

Scoria is an international collaborative thesis project involving the Institute of Computational Perception at Johannes Kepler University in Linz, Austria and the Prague Music Computing Group at Charles University in Prague, Czechia. Through this collaboration, we aim to advance research in scorification while contributing to open-source development.

## Goal
SCORIA is a scorification project. We aim to collaboratively create a complete pipeline to automatically and beautifully typeset scores from recorded MIDI data.

---
## Research Areas & Tasks
**Scorification** is the process of transforming a real-life MIDI recording into a quantized, typeset musical score. This can be divided into two key areas: **MIDI Normalization** and **MIDI Scorification**:
- **MIDI Normalization** focuses on time-related aspects, such as quantizing note onsets and durations. The main objective is to adjust the timing of MIDI events (onsets and offsets) to align with meaningful musical values, like beats and note lengths.
- **MIDI Scorification** deals with all other musical elements and attributes required for a readable typeset score. This includes estimating the correct time and key signatures, clef and staff placement, voice assignments, note stemming, and classifying musical ornamentation.

### Nine Challenging Thesis Topics
To make both MIDI Normalization and MIDI Scorification more accessible and approachable, we have broken both areas into the following subtopics and related tasks:
1. **MIDI Normalization**: [Free Performance Quantization (FP)](#free-performance-quantization-fp)
2. **MIDI Normalization**: [Performance to Click Quantization (PC)](#performance-to-click-quantization-pc)
3. **MIDI Normalization**: [MuseScore MIDI Normalization (MS)](#musescore-midi-normalization-ms)
4. **MIDI Scorification**: [Meter / Barline / Tie Estimation (MBT)](#meter--barline--tie-estimation-mbt)
5. **MIDI Scorification**: [Key / Pitch Spelling Estimation (KPS)](#key--pitch-spelling-estimation-kps)
6. **MIDI Scorification**: [Beaming / Grouping Estimation (BG)](#beaming--grouping-estimation-bg)
7. **MIDI Scorification**: [Clef / Staff Estimation (CS)](#clef--staff-estimation-cs)
8. **MIDI Scorification**: [Stemming / Voice Estimation (SV)](#stemming--voice-estimation-sv)
9. **MIDI Scorification**: [Ornamentation Classification (OC)](#ornamentation-classification-oc)


For more details, see each project description below. 

---
### MIDI Normalization
#### Free Performance Quantization (FP)
Free performance quantization involves processing a MIDI recording of a performance that doesn’t follow a strict tempo (e.g., a live, expressive piano performance) and aligning the timing of the notes to a structured, musical grid. The challenge here is preserving the nuances of the performance while still making the timing conform to standard musical values (e.g., quarter notes, eighth notes). This task requires creating algorithms that intelligently adjust note onsets and durations while maintaining the musical expressiveness of the original performance.
#### Performance to Click Quantization (PC)
In performance to click quantization, the goal is to synchronize a MIDI performance that was played without a metronome (free time) to a predefined tempo or click track. This involves adjusting the note onset timings so they align with the beats of the click track, i.e., ensuring consistency with a metrical grid.
#### MuseScore MIDI Normalization (MS)
MuseScore MIDI normalization refers to developing methods to process and clean up MIDI data so that it can be directly imported and used in [MuseScore](https://musescore.org/en), a popular open-source music notation software. This involves quantizing note timings, estimating note durations, and making the MIDI data compatible with standard notation rules. The goal is to ensure that MIDI recordings, which typically have irregular or non-standard note durations, are normalized for accurate and efficient conversion into readable sheet music within MuseScore.

---
### MIDI Scorification

#### Meter / Barline / Tie Estimation (MBT)
In this task, the focus is on detecting the meter (time signature), barlines (measure divisions), and ties (which connect notes across bars) from MIDI data. Since MIDI data doesn’t inherently include this information, the challenge is to analyze the timing and rhythmic structure of the notes to infer where the barlines should be placed and how notes should be tied across them. The aim is to ensure that the score reflects a musician's intuitive understanding of meter and phrasing.
#### Key / Pitch Spelling Estimation (KPS)
This task involves estimating the key signature and determining the correct pitch spelling for each note in the MIDI data. While MIDI data represents pitches with numerical values, translating them into musical notation requires understanding which pitches should be spelled as sharps, flats, or naturals (e.g., determining if a pitch is C# or Db). The task also includes identifying local changes in key signature, which influence local adjustments in pitch spelling and make the score easier to read and interpret.
#### Beaming / Grouping Estimation (BG)
Beaming refers to grouping notes together with beams (horizontal lines connecting note stems) in a way that visually reflects the rhythmic structure of the music. This task focuses on automatically determining how notes should be grouped together, especially in faster rhythms like eighth notes or sixteenth notes. The goal is to make the score visually clear and musically logical, following standard notational conventions for grouping notes within beats and measures.
#### Clef / Staff Estimation (CS)
In MIDI standard notation, notes are not assigned to specific clefs or staves (e.g., treble, bass). This task involves analyzing the pitch range of the notes and determining the most appropriate clef and staff assignment. For instance, higher notes are typically placed on the treble staff, while lower notes go on the bass staff. This estimation ensures that the resulting score is readable and follows conventional music notation practices.
#### Stemming / Voice Estimation (SV)
Stemming refers to deciding the direction of note stems (up or down), which helps visually organize the score, especially in polyphonic music. Voice estimation involves assigning notes to separate musical voices or parts when multiple lines of music are being played simultaneously (e.g., in piano music with independent left and right-hand parts). This task is about properly assigning notes to different voices and determining the correct stem directions to clearly represent multiple musical lines within a single staff.
#### Ornamentation Classification (OC)
This task focuses on detecting and classifying ornamentation—decorative musical elements such as trills, grace notes, or mordents—that are often present in performance recordings but not explicitly encoded in MIDI data. The challenge is to identify when and where these ornaments occur and then properly represent them in the musical score using appropriate score onset and duration values. This ensures the score is both accurate and consistent, while (more) closely reflecting the nuances of the intended performance.

---
## How It Works
1. **Student Enrollment**:
Select a research topic.
2. **Mentor Assignment**:
International experts provide guidance and supervision.
3. **Project Integration**:
Thesis work is aligned with open-source contributions.
4. **Collaboration & Feedback**:
Regular mentorship sessions ensure steady progress.
5. **Final Submission & Contribution**:
Each thesis work contributes to the open-source scorification pipeline, which will be released around September 2025. 

--- 

## How to Apply:
- **Process**: 
Select a research topic and task **by October 24, 2024**. (Note that topics are assigned on a FIFO basis.)
- **Requirements**: 
strong AI/ML/music computing background, motiovation and time commitment
- **Deadlines**: 
(Latest) by September 2025, when we'll release the scorification tool. 

---

## FAQs

**What should my thesis look like in the end?** 

The goal of each thesis is to: 
- write a comprehensive overview of both traditional and machine learning based approaches to the topic
- (re)implement or adapt one state-of-the-art algorithm to work within the API specification of SCORIA
- finish at latest by September 2025, when we’ll assemble all parts and release the scorification tool

**Why should I join the SCORIA project?** 

We offer you: 
- interesting and challenging music AI tasks
- supervision by experts in the field
- collaborative work with peers across Czechia and Austria
- lasting contributions to an open source project beyond your own thesis
- a specified API for the pipeline
- a utility codebase for symbolic music processing python and data which gets you started on the task right away

**Which prerequites are necessary?** 

We need you to: 
- have a strong background in AI/ML/music computing
- be interested in music scores and their intricacies, and you must be able to read music
- be able and willing to complete a thesis within the time allotted.

---
## Contact Us
If you’re interested in a task or thesis or just need more information, please reach out to:
- Institute of Computational Perception / Johannes Kepler University: 
  coordination: Silvan Peter, silvan.peter@jku.at 
  
  https://www.jku.at/en/institute-of-computational-perception/
- Prague Music Computing Group / Charles University: 
  coordination: Jan Hajič jr., hajicj@ufal.mff.cuni.cz 
  
  https://ufal.mff.cuni.cz/prague-music-computing-group

![CP](./assets/img/logo-cp.png) ![PMCG](./assets/img/logo-pmcg.png)
