# Claude-API-AMSTAR2-Reliability
# Reliability of LLM-Assisted AMSTAR-2 Critical Appraisal: Controlled Claude API Experiments

**Status: Protocol development / pre-experiment. No empirical findings are reported in this repository.**

**Research lead:** Carole Lunny, MPH, PhD, University of British Columbia
**Program:** AI for Science (Anthropic API-credit award, $25,000 USD, October-March 2026)  
**Domain:** Scientific evidence evaluation, systematic reviews, reliability of LLM judgements

## Why this matters
Large language models can produce plausible methodological quality assessments of systematic reviews, yet similar answers do not necessarily reflect correct judgements. An evaluation should therefore check both the final classification and whether it is supported by evidence from the review. Changes in task presentation or prompt structure may also alter model decisions even when the underlying review is unchanged.

This project examines the sensitivity and reliability of LLM-assisted **AMSTAR-2** methodological appraisal using systematically structured comparisons, human reference assessments and source-evidence checks.

## Research questions
1. Under controlled conditions, do changes in how AMSTAR-2 appraisal questions or decision rules are presented affect judgements?
2. Does asking about items separately versus together change the resulting decisions and their evidentiary support?
3. How frequently do repeated executions of a defined condition yield different outputs?
4. Where a model agrees with a reference judgement, does its quoted evidence actually support the answer?

## Planned study design
The study uses systematic reviews from the **WISEST AI** research program, which includes a benchmark of human expert assessments of methodological quality and risk of bias, source quotations, rationales and evidence-clarity ratings. 

The current experimental plan investigates two prompt-design contrasts:

| Comparison | Planned contrast | Purpose |
|---|---|---|
| A | Item-by-item versus bundled AMSTAR-2 assessment | Test whether evaluating several items in one request changes responses |
| B | Structured decision-rule wording versus original AMSTAR-2 question wording | Test whether task specification affects results |

The planned model environment is **Claude API**, with a fixed model snapshot and documented settings for each run. Conditions will be compared using the same source-review evidence wherever required by the protocol. Repetitions will be scheduled to measure variability; exact review sampling, repeat counts and analysis methods will be specified in the finalized protocols.

## Planned workflow
```text
Eligible systematic-review PDF
          |
          v
Controlled document preparation and model input
          |
          v
Condition-specific prompt and question/decision rules
          |
          v
Claude API response: step answers, quotations, rationale, locators
          |
          v
Schema checks + deterministic decision-rule application (when used)
          |
          v
Comparison with independent reference assessments
          |
          v
Source-quote/evidence verification and adjudication
          |
          v
Accuracy, evidence support, variability and sensitivity analyses
```

## Planned outcomes
- **Judgement accuracy:** agreement with prespecified expert reference judgements, using explicitly documented scoring rules.
- **Evidence-supported judgement:** whether supporting quotations and rationales substantiate the model's response.
- **Repeat-run variability:** frequency and patterns of changes across replicated runs under specified conditions.
- **Evaluation-design sensitivity:** differences in outputs across controlled prompt designs.
- **Auditability:** completeness of structured outputs, source locators and run metadata.

Evidence support and answer accuracy will be treated as distinct outcomes. A reproducible answer is not necessarily a valid answer; a changed answer is not necessarily an error.

## Reproducibility commitments
The protocol experiment workflow is being designed to record, where applicable: exact model identifier, API parameters, prompt and decision-rule versions, document-processing method, review identifier, condition, run identifier, timestamps, structured output, validator results and adjudication status. 

## Repository roadmap
- [ ] Two experimental protocols and analysis plan
- [ ] Frozen prompt versions and decision-rule specifications
- [ ] Schema validation and reproducible run log
- [ ] A small technical pilot
- [ ] Reference-judgement verification procedures
- [ ] Controlled API experiments
- [ ] Permitted scripts, documentation and aggregate results

## Data availability and research integrity
The WISEST Benchmark corpus, full-text PDFs, review-specific human labels, proprietary instrument text, prompts containing protected material, API credentials and unpublished results are **not included** in this public repository. Any future data release will follow legal, ethical, licensing and scientific-validity requirements. 

## Related projects
- [TRAILS taxonomy](https://github.com/carolelunny/TRAILS)
- [Carole Lunny GitHub profile](https://github.com/carolelunny)
- [Google Scholar](https://scholar.google.com/citations?user=iJKQnaYAAAAJ)

## Contact
For research collaboration, see the linked GitHub profile or [LinkedIn](https://ca.linkedin.com/in/carole-lunny-56973a294/).

