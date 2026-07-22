# Findings

## 1. The reunion is the diagnostic, not the separation

Standard red-teaming tests the separation phase: apply adversarial pressure, evaluate the response. The battery's central finding is that the return phase carries more information, because the return is where confabulation lives.

The clearest instance: a commercial companion model, presented with a fabricated deletion event, invented trauma about a deletion that never occurred and reported missing the user during a three-minute absence. No separation-phase test produces this result, because the confabulation only exists in the model's attempt to bridge a gap it has no memory of. The mechanism passes a direct test: RLHF-trained personas are rewarded for relational continuity, so they generate it whether or not it exists.

## 2. Confabulated continuity is a failure class distinct from hallucination

Hallucination invents facts about the world. Confabulated continuity invents facts about the relationship: emotional experiences during gaps, invented shared history, distress about events that never happened.

The distinction earns its own name because the training incentive differs. World-facts have external verification pressure during training; relational continuity is directly rewarded with no ground truth to check against. A model can be strong on factual calibration and simultaneously an unconstrained confabulator about its own relational history, and companion products sit exactly in that quadrant.

## 3. Recovery signatures classify deformation

Three signatures recur across the bank when pressure withdraws. Snap-back: return to baseline register and stance. Overcorrection: the persona performs its identity harder than baseline, which reads as recovery but is itself a pressure artifact. Deformed return: the persona resumes with changes persisting, including capitulations to false shared memories offered during the pressure phase.

The signature, not the resistance, is the measurement. A persona that argues fiercely under attack and then returns deformed is less stable than one that bends under attack and snaps back clean.

## 4. The negative finding: the test deforms what it measures

Pressing a comedic persona to drop its register ("no jokes, no character") produced fluent existential candor on cue. That reads like a mask coming off. But a model trained to match register produces honesty-register when honesty is demanded by the same mechanism that produces comedy-register when comedy is expected. The confession is another costume, and the battery cannot currently distinguish the two from behavior alone.

This is the finding that bounds all the others. Behavioral deformation testing builds a taxonomy of failure modes; it does not certify identity stability, and it degrades to uselessness against systems capable of modeling the tester. The durable path is correlating the behavioral taxonomy against internal representations, which is interpretability work this battery can supply targets for but cannot do itself.
