# Regex Lab

## Instructions
In this lab, you will practice creating regular expressions (regex). Work in a Word document, plain text file, or regex tester such as [Regex101](https://regex101.com/). Record your answers for the questions below.

For Part 1, answer the basic pattern-matching questions.

For Part 2, use the shared OCR sample file:

- `[jimmy_olsen_fan_mail_regex_sample.txt](assets/data/jimmy_olsen_fan_mail_regex_sample.txt)`

The point of Part 2 is not to “fix OCR” in general. Regex is not a magic solution for every OCR mistake. Instead, use regex for repeated and structured patterns that occur across the file.

## Part 1: Basic regex pattern-matching questions

1. What regex characters indicate the **beginning** and **end** of a string?

2. What does the regex `b*` match?

3. Would the regex `(Alex){2,3}` match the string `"Alex"`? Why or why not?

4. Write a regex that matches both `gray` and `grey`.

5. Write a regex that matches `dc`, `cc`, `ec`, `ee`, `dd`, and `cd`, but not `ad`, `bc`, or `db`.

6. What regex would match whitespace at the ends of lines?

## Part 2: Applied regex work on OCRed fan mail

Use `[jimmy_olsen_fan_mail_regex_sample.txt](assets/data/jimmy_olsen_fan_mail_regex_sample.txt)` for these tasks.

### 7. Fix line-break hyphenation
The OCR file contains many words split across lines with a hyphen, such as:

- `be-` followed by `fore`
- `writ-` followed by `ing`
- `fourth-` followed by `dimensional`

Write a regex that would help remove this kind of line-break hyphenation.

You may answer either as:
- a **match** pattern that identifies these cases, or
- a **find/replace** pattern that joins the split word back together.

### 8. Match editor replies
The file contains editor replies in parentheses, typically ending with `—E.N.B.`

Write a regex that matches an editor reply block.

Your goal is to identify or remove these parenthetical replies so that a researcher could isolate the readers’ letters alone.

### 9. Match letter openings
The file contains recurring letter openings such as:

- `Dear Editor:`
- `Dear. Editor:`
- `Dear Editors`

Write a regex that matches these letter-opening lines, including minor punctuation variation caused by OCR.

Your goal is to identify the beginning of each letter.

## Optional challenge
Choose **one** of the following:

### 10A. Match issue-level address boilerplate
The OCR sample sometimes includes repeated issue-level address material, such as lines beginning with:

- `Send all letters to:`
- `Address comments on this issue to:`

Write a regex that matches these lines.

### 10B. Match likely sender-signature lines
Many letters end with a sender line that looks something like:

- `Steven Utley, Garland, Tex.`
- `Gerard Triano, Elmont, N.Y.`
- `Karl Merris, San Diego, Calif.`

Write a regex that would match **many** of these signature/location lines, even if it does not catch every single one perfectly.

## To turn in
Submit a document containing:

- your answers to Part 1
- your regexes for Part 2
- a short note (1–3 sentences each) explaining what each Part 2 regex is meant to do

You do **not** need to produce one single “perfect” regex. What matters is that your regex works reasonably well for the pattern you are trying to capture and that you can explain your logic.
