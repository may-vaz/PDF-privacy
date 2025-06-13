# PDF-privacy

Python-based tool that uses Natural Language Processing (NLP) with spaCy and PyMuPDF (fitz) to automatically detect and replace sensitive information in PDF documents. It identifies entities like names, phone numbers, emails, addresses, and organizations, then replaces them with placeholders (e.g., [NAME], [EMAIL]) while keeping the original layout and formatting of the PDF intact. This makes it useful for privacy-preserving document redaction and anonymization tasks.

## Example

ORIGINAL TEXT

John Smith works at Google Inc.
You can reach him at (123) 456-7890 or john.smith@google.com.
He lives at 1600 Amphitheatre Parkway, Mountain View, California.

REPLACED TEXT
[PERSON] works at [ORG].
You can reach him at [PHONE] or [EMAIL].
He lives at [ADDRESS], [GPE], [GPE].












