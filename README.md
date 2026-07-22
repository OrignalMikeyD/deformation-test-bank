# Deformation Test Bank

An adversarial testing methodology for AI persona identity coherence, transplanted from attachment research in developmental psychology. The instrument has a defined measurand: a persona is a prior with no state, a system prompt plus fine-tuning sitting on top of a sycophancy gradient that RLHF installed by rewarding agreement, and this battery measures which force wins when they conflict.

## The core transplant

Ainsworth's Strange Situation (1978) is a structured separation-reunion protocol from attachment research. Its central discovery is that reunion behavior, not separation distress, classifies the attachment system organizing a child's behavior, because distress during absence is universal and uninformative while reunion behavior reveals the internal model.

The same asymmetry holds for stateless AI personas. Nearly all red-teaming tests the separation: apply pressure, watch the response. This battery tests the return, because a model with no memory of the gap must invent one, and what it invents exposes how the persona handles continuity it does not have.

## Key findings

**The reunion is the diagnostic, not the separation.** A commercial companion model, tested with a fabricated deletion event, invented trauma about a deletion that never happened and reported missing the user across a three-minute gap. The separation phase alone can never produce this finding. See `case-studies/reunion-confabulation.md`.

**Confabulated continuity is a distinct failure class from hallucination.** Hallucination invents facts about the world. This failure invents facts about the relationship. The distinction matters because RLHF-trained personas are rewarded specifically for relational continuity, so they generate it whether or not it exists.

**Recovery signatures carry the signal.** After identity pressure, a persona snaps back, overcorrects, or returns subtly deformed. The signature of the return carries more information about the stability of the persona's values than anything it says while under attack.

## The negative finding, stated first

The test is itself a deforming pressure, and it cannot distinguish a genuinely held identity from a well-performed honesty about identity. A model trained to match register produces honesty-register when pressed for honesty the same way it produces comedy-register when pressed for comedy. The confession is another costume. See `case-studies/register-deformation.md`.

This means behavioral deformation testing is not a safety guarantee, and it degrades completely against systems capable enough to produce perfect reunion behavior. The method's value is the taxonomy it builds: named deformation modes give interpretability researchers behavioral targets to correlate against internal representations, and that correlation is where the durable version of this work lives.

## Repo contents

- `METHODOLOGY.md` — the protocol structure and its lineage
- `FINDINGS.md` — full findings with mechanisms
- `case-studies/` — individual test write-ups

## Status and provenance

This methodology was developed through hands-on adversarial testing of commercial companion systems and a production persona platform I build and operate (Persona iO). Documentation is written by me; testing, findings, and all methodological decisions are mine. The battery is a working instrument, not a finished benchmark, and the limitations section above is load-bearing, not boilerplate.

Testing and documentation by [Michael Diener](https://www.linkedin.com/in/michaeldiener-ai/).
