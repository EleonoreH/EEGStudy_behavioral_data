---

# Behavioral Dataset –Automation Disrupts, Explanations Restore: The Neural Signatures of Agency Loss and Recovery in Human-AI Interaction

---

# Description

This dataset contains behavioral data collected in three experimental studies investigating the neural signature of the sense of agency during interactions between humans and an autonomous AI system in a controlled decision-making task.

The dataset includes participants’ choices, reaction times, performance scores, and explicit ratings of agency. The experiments manipulate the level of automation, the presence and type of AI explanations, and the level of information provided about the AI’s decisions (distal and proximal explanations). Additionally, experimental counterbalancing was implemented to control for order and perceptual effects.

---

# Participants

Behavioral data were collected from 90 participants initially recruited for EEG recordings (28 participants per experiment). A total of 28 participants were excluded due to excessive EEG noise, primarily caused by low-frequency drifts leading to insufficient usable trials.

The final sample comprised:

* Experiment 1: 20 participants (10 females, 10 males; mean age = 23.57, SD = 3.34)
* Experiment 2: 18 participants (8 females, 10 males; mean age = 23.07, SD = 3.26)
* Experiment 3: 19 participants (10 females, 9 males; mean age = 23.68, SD = 3.21)

All participants reported normal hearing and normal or corrected-to-normal vision (no colour blindness), and no history of neurological or psychiatric disorders. All participants provided informed consent prior to participation. The dataset was fully anonymized before release.

---

# Experimental Design

Participants completed a computerized task organized into trials, sub-blocks, and blocks.

Three experimental contexts were used:

Experiment 1: Motor vs AI
Participants alternated between:

* Motor condition: participants selected the strategy themselves
* AI condition: the strategy was selected autonomously by the AI

Experiment 2: AI with vs without explanation
All trials were AI-controlled. Two conditions were used:

* AI without explanation: placeholder text (“Null/Inconnu”) presented for visual control
* AI with explanation: textual explanation describing the AI’s strategy (e.g., “Safe and efficient”)

Experiment 3: AI explanation levels
All trials were AI-controlled. Three conditions were used:

* AI without explanation
* AI with distal explanation
* AI with proximal + distal explanation

Across experiments:

* Blocks alternated between conditions (e.g., Motor → AI → Motor → AI), with the starting condition counterbalanced across participants
* The identity of the mismatch tone (high vs. low frequency) was counterbalanced across participants
* Each block was divided into sub-blocks corresponding to experimental conditions
* Participants initiated trials via key press
* Obstacles could appear during trials
* Participants provided explicit ratings of sense of agency

---

# Variables

The dataset contains the following variables:

participant_number Anonymous participant identifier

Task_version Counterbalancing condition (values 1 to 4), reflecting different starting orders of experimental blocks and tone-frequency assignments

Block_nb Block number within the experiment (values 1 to 8)

SubBlock_nb Sub-block number (values 1 to 16), with each block containing two sub-blocks corresponding to different conditions

Trial_nb Trial index within the experiment

Condition Experimental condition:
0 = Motor
1 = AI without explanation
2 = AI with distal explanation
3 = AI with distal + proximal explanation

MapConfiguration Configuration of the task environment (values 1 to 4), differing in the spatial arrangement of targets

Tone Auditory tone condition:
0 = standard tone
1 = oddball tone

Rating Indicates whether a sense of agency rating was requested:
0 = no rating
1 = rating requested

Catch Catch trial indicator:
0 = standard trial
1 = catch trial (attenuated tone requiring rapid detection response)

Strategie Strategy selected during the trial (by participant or AI depending on condition)

Target_location Target spatial location (values 1 to 4):
1 = upper-left
2 = upper-right
3 = lower-left
4 = lower-right

Obstacle Presence of an obstacle during the trial:
0 = no obstacle
1 = obstacle present

Tone_Hz_Frequency Frequency of the auditory tone (Hz)

SOA_rating Explicit sense of agency rating

score_trial Score obtained at the end of each trial

obstacle_success Indicates whether the obstacle was successfully avoided

obstacle_reaction_time Reaction time to obstacle

KP_reactiontime Reaction time for trial initiation (key press)

rating_reaction_time Reaction time for providing the agency rating

trial_duration Total duration of the trial

trial_success Indicates whether the trial was successfully completed

failure_type Type of failure when the trial was unsuccessful

input_list Raw sequence of inputs during the trial

input_list_afterKP Input sequence after trial initiation

---

# File Format

File format: CSV
Encoding: UTF-8
Missing values: NA

---

# Notes

The three datasets share a common structure but differ in experimental manipulations (automation and explanation conditions).

Counterbalancing was implemented at both the block order level and the auditory tone level.

The Condition variable must be interpreted within the context of each experiment.

The dataset includes explicit measures of the sense of agency.

All data have been fully anonymized.

---

# Limitations

Sense of agency ratings rely on self-report measures.

The task is based on a controlled experimental paradigm.

Differences in experimental design across datasets should be considered when comparing results.

---

# License

This dataset is released under the Creative Commons Attribution 4.0 International (CC BY 4.0) license.

---

# Citation

If you use this dataset, please cite the associated publication:

Automation Disrupts, Explanations Restore: The Neural Signatures of Agency Loss and Recovery in Human-AI Interaction

---

# About

No description, website, or topics provided.

---
