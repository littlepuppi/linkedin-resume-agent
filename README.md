# LinkedIn Resume Agent

A tool that customizes a resume based on a job description. It loads a user profile, extracts keywords from the posting, tailors the summary and experience bullets, and writes the result as text and JSON. The JavaScript version can also generate a Word document.

The GitHub description for this repository is: “Intelligent resume tool that customizes resumes based on job descriptions.” The code lives in the `linkedin-resume-agent/` folder. A copy of the same project also appears in the [ExpressMongo](https://github.com/littlepuppi/ExpressMongo) repository.

## Features

- Keyword extraction from a job description (technical and soft-skill lists)
- Tailored summary and experience text
- Output as plain text and JSON
- JavaScript version can also write a `.docx` file

The job description and profile path are currently hard-coded in the scripts; edit those values before running.

## Tech stack

- JavaScript (Node.js) with the `docx` package
- Python 3 (standard library only)

## Getting started

All commands below are run from the `linkedin-resume-agent/` folder.

### JavaScript

```bash
cd linkedin-resume-agent
npm install
npm start
```

`npm start` and `npm run dev` both run `node linkedinResumeAgent.js`. The script loads a profile from a local JSON file and writes text, JSON, and Word output files in the same folder.

### Python

```bash
cd linkedin-resume-agent
python linkedin_resume_agent.py
# or
python my_resume.py
```

No third-party Python packages are required.

## Project structure

```
linkedin-resume-agent/
  linkedinResumeAgent.js      # Node entry point (npm start)
  linkedin_resume_agent.py    # Python agent and a sample __main__ profile
  myResume.js / my_resume.py  # Profile-specific runners
  package.json
```

The folder also includes sample profile and output files. Be careful about committing personal contact details in a public repository.
