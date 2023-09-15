name: Bug Report
description: Template for bug reports
title: '[Bug]: '
assignees:
  - asheroto
body:
  - type: markdown
    attributes:
      value: >-
        Please check to see if your problem already exists with a quick search
        of the issues. Start with one relevant term and then add others if you
        get too many results.


        Name your issue appropriately: give it a sentence that reads well enough
        for anyone seeing this in the release notes to know what it is.


        When writing out the issue details, please ensure you are writing it as
        if you were explaining it to somebody else, even if you will be working
        on and resolving the issue yourself. This helps others to understand the
        reasons for the issue and for it to be searchable in the future.
  - type: checkboxes
    id: checklist
    attributes:
      label: Checklist
      description: Before continuing, make sure you have done the following.
      options:
        - label: I have verified no other issues exist related to my problem.
          required: true
        - label: 'I have verified this issue is not security related. '
          required: true
        - label: >-
            I have verified that the latest version of [.NET
            Framework](https://dotnet.microsoft.com/en-us/download/dotnet-framework)
            has been installed.
          required: true
        - label: >-
            I have restarted my computer to confirm this is not a transitory
            problem.
          required: true
  - type: textarea
    id: what-are-you-seeing
    attributes:
      label: What You Are Seeing?
      description: >-
        In your own words, please describe the problem that you are
        experiencing. Please include images if possible, as this can give a
        clearer indication of the problem.
    validations:
      required: true
  - type: textarea
    id: what-is-expected
    attributes:
      label: What is Expected?
      description: >-
        Instead of the behavior that you were seeing, what did you expect would
        be happening instead?
    validations:
      required: true
  - type: textarea
    id: how-did-you-get-this-to-happen
    attributes:
      label: How Did You Get This To Happen?
      description: >-
        Please include a complete set of reproducible steps that another user or
        maintainer of the repository can follow to get the same behavior that
        you are seeing.  NOTE: We may be unable to troubleshoot/respond to
        issues without reproducible steps. If you do not complete this section,
        there is a high chance your issue may be closed.
      value: |-
        1. I ran this
        2. I clicked on this
        3. But it only happens with this game
    validations:
      required: true
  - type: textarea
    id: system-details
    attributes:
      label: System Details
      description: >-
        Please include as many details about your system as possible. Sometimes,
        a problem may only happen on specific systems, and this information can
        be vital to resolving your issue. At minimum, please include your
        operating system and seDirector version.
      value: |-
        - Windows 11 Pro
        - seDirector 7.3.3
    validations:
      required: true
  - type: textarea
    id: additional-context
    attributes:
      label: Additional Context
      description: >-
        Please include any other information here that you feel may be relevant
        to the problem you are seeing but is not covered in the previous
        sections.
      value: Screenshots, etc
  - type: textarea
    id: sedirector-error-log
    attributes:
      label: seDirector_error.log Output
      description: >-
        If you have the file `C:\Program Files\seDirector\seDirector_error.log`
        please paste the output here, otherwise ignore this step
  - type: markdown
    attributes:
      value: >-
        This template was generated with [Issue Forms
        Creator](https://issue-forms-creator.netlify.app)