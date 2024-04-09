# Fundamentals of a data-processing pipeline

Automation in the form of robust pipelines described as _code_ is a key foundation for the success of large-scale data processing
as it demonstrates it is technically possible to process the data without intervention

## When to use a pipeline/workflow

- Anytime you find yourself running sequential commands that are predictable/repetitive (with mostly the same settings everytime)
- When operations can be run in parallel, especially when individual steps take a few minutes to run
- When you need to:
  - ensure that the same steps are run in the same order every time
  - ensure that the same settings are used every time
  - ensure that the same software versions are used every time
  - ensure that the same data is used every time

## Re-use existing code, tools, containers, and other assets

- chances are someone else has already tackled a similar problem, and you may be able to reuse/augment their work
- this can save time and effort, and also help to ensure that your pipeline is robust and well-tested

## Sources used in writing this document

[Ten Simple Rules for large-scale data processing](https://terra.bio/ten-simple-rules-4-automate-your-workflows/)

[Automate Your Workflows](https://terra.bio/ten-simple-rules-4-automate-your-workflows/)