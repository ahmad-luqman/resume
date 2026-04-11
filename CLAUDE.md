# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Build

```bash
make compile    # Compiles resume.tex → resume.pdf (uses texi2pdf)
make clean      # Removes aux/log/out/sync files
```

Requires `texi2pdf` (part of TeX Live distribution).

## Architecture

This is a LaTeX-based resume. The single source file `resume.tex` defines custom commands for formatting (`\employer`, `\header`, `\school`, `\contact`, `achievements` environment) at the top, then uses them throughout the document body. `Talks.Md` contains the same talks section in Markdown format.

## Branches

- `master` - main resume
- `devops` / `kubernetes-terraform` - variant resumes emphasizing different skill areas
- `updated-resume-20240521` - dated snapshot
