# Seismic ML Quick Check

**Developed by [Dr. Heather Bedle](mailto:hbedle@ou.edu) and [Dr. April Moreno-Ward](mailto:April.MorenoWard-1@ou.edu)**  
AASPI (Attribute Assisted Seismic Processing & Interpretation)  
University of Oklahoma, School of Geosciences  
[aaspi.ou.edu](https://www.ou.edu/mcee/labs/aaspi)

**[Launch the tool](https://hbedle-subsurface.github.io/seismic_ml_quickcheck/)** - quick check version

---

**Version 1.0 - in active testing. If a question felt unclear, an answer option didn't fit your situation, or you kept thinking "but what about..." - please email hbedle@ou.edu. That feedback is genuinely how this gets better. Thanks!**

---

## The short version

You ran seismic ML. The result looks great. But did it find geology - or just patterns in whatever you handed it?

This is a ~5 minute, plain-English reality check for geoscientists at any experience level. Twelve questions across four topics. No statistics degree required. At the end you get a clear picture of where your workflow is solid and a short list of specific things worth fixing before this result goes anywhere important.

---

## Why this exists

Seismic machine learning is genuinely powerful. It is also genuinely indifferent to what you were hoping to find. Feed it acquisition footprint and it will cluster your footprint beautifully. Give it unnormalized attributes and the result reflects data scaling, not geology. Run it on a full 3D volume when you care about a 50ms reservoir window and the method spends most of its effort distinguishing overburden from basement.

None of these are software problems. They are workflow problems. And they show up constantly - in student projects, in industry practice, in published papers - regardless of what software produced the result.

The full AASPI uncertainty assessment tool covers all of this in depth. This shorter version exists for anyone who wants a quick, structured reality check without the full 15-20 minute commitment - whether you're new to ML-assisted interpretation or you've been doing seismic interpretation for decades and just want to know if a result holds up.

The questions are grounded in geologic reasoning, not ML theory. Every question has a plain-language explanation of why it matters. No prior background in machine learning is assumed or required.

---

## What it covers

Four sections, twelve questions:

1. **Your data - before ML touched it** - signal-to-noise quality, acquisition footprint, survey vintage consistency
2. **The attributes you fed it** - geologic rationale for attribute selection, normalization, redundancy
3. **How you set it up and ran it** - windowing to the target interval, number of classes, parameter stability testing
4. **Checking whether it actually worked** - prior hypothesis vs. post-hoc interpretation, calibration to independent geologic data, artifact checking

Methods covered: k-means, PCA/ICA, SOM, GMM, GTM, and any other unsupervised classification method.

---

## Who it is for

- **Anyone who has run seismic ML and wants a fast gut-check** before presenting results
- **Geoscientists new to ML-assisted interpretation** who want to know what questions they should be asking
- **Experienced interpreters** who are evaluating an ML result - theirs or a colleague's - and want a structured way to do it
- **Instructors** looking for a classroom discussion framework for seismic ML workflows

No ML background required. If you know what a time slice is and you've looked at seismic before, you have everything you need.

---

## How to use it

Open the link above. The tool runs entirely in your browser - nothing is stored or transmitted. Your answers stay on your machine. You can save a PDF at the end.

Work through the four sections. Answer honestly. "Not sure / doesn't apply" is always an option and scores as high uncertainty - not as a penalty, but because genuinely not knowing something is a real source of uncertainty in your interpretation.

At the end you get:
- An overall uncertainty score with a plain-language summary
- A section-by-section breakdown showing where the gaps are
- A prioritized list of specific actions to address what the check found

The whole thing takes about five minutes. And you will get a idea of how to take a few actions to improve your certainty in your ML results.

---

## Relationship to the full AASPI assessment tool

This quick check is a companion to the full [Seismic Multi-Attribute ML Uncertainty Assessment](https://hbedle-subsurface.github.io/seismic_ml_assessment/), not a replacement for it.

The full tool covers everything this one does, plus dimension reduction (PCA vs. ICA evaluation, component-by-component review, footprint in components), detailed attribute redundancy analysis, GMM covariance structure, explainability and sensitivity testing, geologic validation against depositional models and analogs, well calibration, and uncertainty communication. It also includes dedicated AASPI note boxes throughout with specific guidance for kmeans3d, pca3d, ica3d, som3d, gmm3d, gtm3d, analyze_input, and attribute_selection. It takes 15-20 minutes and produces two 2x2 uncertainty matrices.

If you finish this quick check and want to go deeper - or if you're working through a result that's going to drive a real decision - the full tool is where to go next.

---

## This is a living document

Planned additions to the quick check:

- A version covering supervised methods (PNN, RFC, CNN) for folks using those workflows
- Questions on SAM (Segment Anything Model) applications to seismic facies

If you used this and found a question that didn't fit, an option that wasn't quite right for your situation, or a workflow step you kept wishing it had asked about - please reach out. That kind of feedback is exactly what shapes the next version.

**Contact:** [hbedle@ou.edu](mailto:hbedle@ou.edu)  
Questions, feedback, and stories from the field all welcome.

---

## Citation

If you use this tool in research, teaching, or a publication, please cite it as:

> Bedle, H.; Moreno-Ward, A. (2026). *Seismic ML Quick Check*, v1.0., AASPI, University of Oklahoma. https://hbedle-subsurface.github.io/seismic_ml_assessment/

---

## License

This work is licensed under [Creative Commons Attribution ShareAlike 4.0 International (CC BY-SA 4.0)](https://creativecommons.org/licenses/by-sa/4.0/).

You are free to share and adapt this tool provided you give appropriate credit and distribute any adaptations under the same license.

---

## Acknowledgments

Developed at the Attribute Assisted Seismic Processing & Interpretation (AASPI), University of Oklahoma, School of Geosciences.  
Built with input from AASPI students, industry practitioners, and the broader seismic interpretation community.
