# Form Model
This page describes a form in a technology-independent manner.

A <span class="concept-reference">form</span> is not a <span class="concept-reference">page</span>, although there is often a 1-to-1 relation between a form and the page it contains.
A <span class="concept-reference">page</span> is a concept used in the context of web sites. It is 
In general a page can contain zero, one or more forms.
A <span class="concept-definition">form</span> is an artifact a user can manipulate to view and modify a collection of data.

A form calls methods to retrieve data and save new or modified data. 

Users may expect particular features from a modern form implementation, such as:
+ change detection 
+ undo/redo at the level of individual characters or fields
+ input validation with clear error messages

Change detection means that the current state of the main data context is compared to its original state after each modification. As soon as there is a difference the commit button is enabled. But, when the current state becomes equal again to the original state - for instance, by a sequence of undo operations - the commit button is disabled.
If the current state of a data part is the same as its original state, it is said to be <span class="concept-definition">pristine</span>; if they are different, the data is said to be <span class="concept-definition">dirty</span>.
