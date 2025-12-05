# Desktop File Organizer - Lazy Automation

## Overview
A Python-based automation tool that organizes desktop files by type, eliminating the tedious manual task of file management. Built with AWS Kiro to accelerate development.

## The Problem
Manually organizing 150+ files scattered across my desktop was taking 20-30 minutes every week - images, PDFs, code files, and documents all mixed together.

## The Solution
This automation script:
- Scans specified directories (Desktop/Downloads)
- Groups files by extension automatically
- Creates organized folder structure (Images, Documents, Videos, Code, Archives)
- Handles duplicate filenames intelligently with timestamps
- Logs all operations for tracking

## How Kiro Accelerated Development

### 1. Spec-Driven Development
Kiro helped generate the initial project structure from simple specifications:
```
Create a Python script that:
- Scans a directory for files
- Organizes files by type into folders
- Handles duplicate filenames
- Logs all operations
```

### 2. Intelligent Code Generation
Kiro assisted with:
- File type detection logic
- Safe file moving with error handling
- Duplicate file renaming strategy

### 3. Automated Documentation
Kiro Hooks automatically update README.md when code changes:
```python
# Hook Configuration
Hook: Update documentation on code change
Trigger: On file save
Action: Update README.md with features and usage
```

## Installation

```bash
# Clone the repository
git clone https://github.com/chakreshkatari/.kiro.git
cd .kiro

# Install dependencies
pip install -r requirements.txt
```

## Usage

```python
python organize_files.py
```

The script will organize files in your Desktop directory by default.

## File Categories

- **Images**: .jpg, .jpeg, .png, .gif, .bmp, .svg, .ico
- **Documents**: .pdf, .doc, .docx, .txt, .xlsx, .pptx
- **Videos**: .mp4, .avi, .mkv, .mov, .wmv
- **Code**: .py, .js, .java, .cpp, .html, .css, .json
- **Archives**: .zip, .rar, .7z, .tar, .gz
- **Others**: Any file not matching above categories

## Results

**Before:**
- Manual organization: 20-30 minutes per week
- Error-prone process
- No documentation

**After:**
- Automated organization: 2 seconds
- Zero errors with proper error handling
- Auto-generated documentation via Kiro Hooks
- **Time saved: ~100 minutes per month**

## Project Structure

```
.kiro/
├── .kiro/
│   ├── hooks/
│   │   └── update_docs.hook
│   └── specs/
│       └── file_organizer.spec
├── organize_files.py
├── README.md
├── requirements.txt
└── .gitignore
```

## Dependencies

- Python 3.8+
- pathlib (built-in)
- shutil (built-in)
- os (built-in)
- datetime (built-in)

## Contributing

Feel free to fork this repository and submit pull requests for improvements.

## License

MIT License

## Acknowledgments

- Built for the Kiro Heroes Week 2 Challenge - Lazy Automation
- Powered by AWS Kiro for AI-accelerated development

## Blog Post

Read the full story: [Automating Desktop Organization with AWS Kiro](https://builder.aws.com/content/36PtvNu6cZ0T5hToCDQSP0CFFJp/automating-desktop-organization-with-aws-kiro-a-lazy-developers-solution)
