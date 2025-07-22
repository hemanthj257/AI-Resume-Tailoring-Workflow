AI Resume Tailoring Workflow (n8n + Adzuna + LangChain)

This n8n workflow automates job discovery and resume personalization using Adzuna, LangChain, and OpenRouter's DeepSeek model. It searches for relevant job listings, extracts structured metadata, and tailors your resume to match each job—hands-free.
✨ What It Does

    🔎 Searches Jobs via the Adzuna API based on role, location, and keyword filters.

    🧠 Extracts Key Metadata (skills, qualifications, job level, etc.) from each job description using an LLM (DeepSeek via LangChain + OpenRouter).

    📝 Tailors Your Resume to each job, rewriting it based on the extracted requirements.

    📄 Uses a Google Doc as the base resume source.

    📊 Stores Results in a Google Sheet, with smart duplicate detection to avoid reprocessing.

    ⏱️ Runs Automatically on a schedule using a Cron node.

📥 How to Use

    Open n8n on your local or hosted instance.

    Import the provided .json file using the “Import from File” option.

    Set up your credentials (Google Sheets, Google Docs, Adzuna, OpenRouter).

    Run the workflow or enable it to run on a schedule.

🧰 Tools Used

    n8n – Workflow automation platform

    Adzuna API – For job listings

    LangChain + DeepSeek (OpenRouter) – For extracting structured metadata and rewriting resumes

    Google Docs – Stores your base resume

    Google Sheets – Logs job metadata and tailored resumes

📌 Notes

    All tailored resumes are saved into the Google Sheet with the job title as the filename.

    You can tweak prompts in the LangChain nodes for different tones or styles.

    Designed for local workflows, but works on n8n Cloud or Docker too.
