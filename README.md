# BlackOut Redactor

A simple, open-source NLP side-project that delves into the concept of entity-extraction.

### What does it do?

Upload any document. The model (dslim/bert-large-NER) will scan through, detecting any sensitive entities and redact them using black bars. Now you can share any sensitive documents without worry!

DISCLAIMER: The model's not perfect, some things can still slip through. Additionally, the model can only detect entities that fall under the categories of

*   `PER` (Person)
*   `ORG` (Organization)
*   `LOC` (Location)
*   `MISC` (Miscellaneous)

Other entities such as GPE (Geopolitical entity), DATE, or CARDINAL are not recognized and censored.

### How to run

Simply open the notebook using Google Colab, connect to a hosted runtime (T4 GPU was used during my testing) and click `Run all`. For an in-depth explanation on what each code cell does, see the Markdown cell before it for more details.

For testing purposes, you can use Sample.pdf to verify the program works properly before using your own documents.
