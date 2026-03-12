DOM-based XSS Detection in Multi-File Environments (Matilda Jean Framework)
This repository contains the benchmark dataset and experimental results for the research paper: "Web Application Security Enhancement through Dom-based XSS Vulnerabilities Detection in Multi-File Environments".

🚀 Overview
The Framework is a hybrid security analysis tool designed to detect DOM-based Cross-Site Scripting (XSS) vulnerabilities in complex, multi-file web environments, specifically focusing on the Laravel framework. By combining enhanced static analysis (via Semgrep and PHP-Parser) with dynamic verification (via Selenium), this framework achieves a high detection rate with minimal false positives.

📂 Repository Structure
/Dataset: Contains the open-source projects and code snippets used for benchmarking (e.g., Microweber, BookStack, etc.).

/Rules: Custom Semgrep rules and detection patterns developed for Laravel-specific sinks and sources.

/Results: Detailed CSV/Excel files containing the identified vulnerabilities, data flow paths, and verification status.
The results file contains the sources extracted using the PHP Parser tool.

The unified_results file contains the sinks extracted using the Semgrep tool.

The related_issues file contains the tracing paths of DOM-Based XSS vulnerabilities in multi-file environments.

🛠️ Methodology
The framework operates in three main phases:

Static Analysis: Utilizing custom rules to scan PHP, Blade, and JS files.

Cross-File Taint Tracking: Linking data flow between backend controllers and frontend templates.


📊 Key Findings
Analyzed 12 open-source projects with over 599 unique sinks.

Identified 3,263 critical data flow paths.

Improved Semgrep detection accuracy from 52.9% to 100% in the tested environment.

Achieved a 0% False Negative rate through rigorous dynamic validation.

📖 Citation
If you use this dataset or framework in your research, please cite our paper:

👨‍💻 Author
Eng. Omar Al-Zamar Master's Researcher in Cybersecurity
