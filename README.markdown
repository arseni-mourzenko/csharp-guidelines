# C# guidelines

This is the list of guidelines that can be applied during code reviews for C# projects. The goal is to cover the patterns that are not necessarily covered by the official Microsoft style or Microsoft's Code Analysis, and to highlight the incorrect practices that are common in C# projects. The goal of those guidelines is to improve the expressiveness and the correctness of the code, through how it looks (formatting) and what it means (semantics).

Each guideline starts by a summary and an example of wrong piece of code and a correct one. It then follows with the explanation about what makes it wrong.

## Formatting

1. [FR0001](guidelines/fr0001.markdown) Do not use arbitrary indentation to “align” code.
1. [FR0002](guidelines/fr0002.markdown) Use consistent line breaks between arguments.
1. FR0003 Call chains: break before every call or not at all; don't mix.
1. [FR0004](guidelines/fr0004.markdown) Do not cut words for variable names in the middle.
1. FR0005 Do not use arbitrary number of letters for variable names.

## Semantics

1. [SM0001](guidelines/sm0001.markdown) Do not repeat the same type twice during initialization.
1. SM0002 Do not comment unnecessarily.
1. [SM0003](guidelines/sm0003.markdown) Do not use leading zeros in numbers (JavaScript octal notation).
1. SM0004 Do not loop on collections with a `for`, a `while`, or a `do while`.
1. [SM0005](guidelines/sm0005.markdown) Make types of parameters as abstract as possible: example of incompatible types being requested from the caller by two consecutive methods.
1. [SM0006](guidelines/sm0006.markdown) Do not use arrays.
1. SM0007 Methods should do one and one only thing (misconception that the reader should not have to jump through lots of methods: if he does, there is something wrong with abstraction, such as unhelpful methods, etc.)
