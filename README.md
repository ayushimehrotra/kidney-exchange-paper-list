# A Paper List for Kidney Exchange Research

## Changelog
 - 12/2023: added some papers
 - 12/2023: thought it was a good idea to release the background research I've accumulated

## Table of Contents

## Organization
I organize the paper list by topic, first by introducing the topic and then adding my notes on each paper.

## What is Kidney Paired Donation?
With many patients on the waiting list, Kidney Paired Donation (KPD) allows patients to bring a donor who is incompatible with the accompanied patient into the donor pool to trade with another patient and donor. Essentially, the accompanied donors of two patients donate their kidneys to the other patient. This swap allows for more transplantations to occur, further reducing the waiting list. 

The start of this area of research started with [Roth et al](https://www.nber.org/system/files/working_papers/w10002/w10002.pdf), introducing *cycle formulation* to calculate the set of optimal cycles in a given patient-donor pool. While the concept may seem simple, it holds many nuances. The objective function when optimizing for the best set of cycles can be changed to fit a certain purpose, whether it is to optimize for the maximum amount of transplants, the likelihood of transplants to occur, or for highly sensitized patients. This motivation leads to an array of algorithms proposed over the past two decades, which I compiled in this paper.

## Optimizing using Preferences
[Aligning with Heterogeneous Preferences for Kidney Exchange](https://ceur-ws.org/Vol-2640/paper_15.pdf)
CEUR Workshop 2020
 - Quantifies societal values and human ethical judgments to break tiebreakers between multiple optimal sets of viable transplants
 - Uses data extracted from Amazon Mechanical Turk, intricate formulation

[Transplant quality and patients’ preferences in paired kidney exchange](https://www.sciencedirect.com/science/article/pii/S0899825611000947)__
Games and Economic Behavior 2012
 - Concludes that patient preferences cannot be added to optimize for the best set of cycles with minimal efficiency
 - Very heavy assumptions during problem formulation: incrementally allocating, no non-directed donors

[Patient Choice in Kidney Allocation: A Sequential Stochastic Assignment Model](https://pubsonline.informs.org/doi/abs/10.1287/opre.1040.0180)
Operations Research 2005
 - Focuses on patient choice and rejection if the patient believes there will be a better kidney in the future
 - Very strong assumptions: static waiting list, constant influx of kidneys, balanced supply and demand, does not allow the kidney to go to the next best fittest

## Optimizing for Sensitized Patients
[Balancing Lexicographic Fairness and a Utilitarian Objective with Application to Kidney Exchange](https://cdn.aaai.org/ocs/ws/ws0424/16193-75982-1-PB.pdf)
AAAI Workshops 2018
 - Creates rules to balance between highly sensitized patients and a utilitarian motive
 - Static model

[Optimal Kidney Exchange with Immunosuppressants](https://ojs.aaai.org/index.php/AAAI/article/view/16073)
AAAI 2021
 - Integrates immunosuppressants into the optimization, considers three different models
 - PICEF on UNOS data

## Optimizing for Success Probability
[Failure-Aware Kidney Exchange](https://dl.acm.org/doi/10.1145/2492002.2482596)
ACM-EC 2013
 - Reflects on the use of KPD and identifies points of failure
 - Integrates expected utility in the objective function and creates unique solver

[Cutting Plane Approaches for the Robust Kidney Exchange Problem](https://www.sciencedirect.com/science/article/pii/S0305054823003349)
 Computers and Operations Research

[Maximizing the expected number of transplants in kidney exchange programs with branch-and-price](https://link.springer.com/article/10.1007/s10479-017-2647-4)
Annals of Operations Research 2017
 - Use probabilities for each edge to simulate the failure rate for each donation, but keeps them all the same
 - Use branch-and-price to enumerate through the cycles in the graph

[Scalable Robust Kidney Exchange](https://ojs.aaai.org/index.php/AAAI/article/view/3899/3777)
AAAI 2019


## Optimizing for Waiting Time

