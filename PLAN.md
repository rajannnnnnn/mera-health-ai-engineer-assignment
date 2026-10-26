# Plan — mera.health Lab Report Extraction

1. Inspect the starter extractor, twelve sample reports, output schema, and eight imperfect gold labels.
2. Define a fixed, clinically meaningful evaluation for missing/extra rows, analyte identity, values, units, and reference ranges. Freeze rules before modifying extraction.
3. Run and record the unchanged baseline, including latency and cost assumptions. Diagnose the top three failures with report-row evidence.
4. Make focused, generalizable improvements; rerun the same evaluation, compare accuracy, latency and cost, and document one unsuccessful experiment.
5. Manually assess the four unlabelled reports, write concise tradeoffs for RAG, fine-tuning and multi-step agents, and preserve actual prompts, verification notes and honest git history.

Keep `python extract.py <file>` returning schema-valid JSON. Never commit secrets or fabricate results. Avoid UI, deployment or unnecessary complexity.
