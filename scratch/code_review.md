Reviewer
========

Improve
-------

* Increase throughput
* Decrease efforts
* Limit delay


Behave
------

* Contribute your specific expertise. Are your comments valuable?
* Judge. No personal preferences.
* Do not criticise. Suggest improvement.


Algorithm
---------

* Auto check first
* Throughput
* Limit delay - 1 day for revision max. Devote the time slot. 3 review per day. 5 would be ineffective! Sort out: delegate or skip.
* Limit revisions: 2 is OK, 3 is hard limit
* Reject immediately when unclear. Talk to author
* No priorities. No assignee. Do it all. In parallel
* 3 categories of defects

Three iterations at max 

* 1st revision: assessment, 1st pass, 2nd pass
  * Assesment: Are you really an expert in that specific area and may contribute a value? Skip the review if not sure you're able to contribute.
  * Assesment: Reject immediately if the code or commit message does not communicate the intention clearly. Do not waste time for reverse engineering. But ask youself first: _are you really en expert_ in that specific area? Even if you are the boss / lead / architect it does not mean you are necessary the expert. Just skip the review otherwise.
  * Assesment: If you see a flaw that may require massive rework - reject the commit. _Reject_ does not mean "it's a piece of crap", the only criteria is: it requires _massive_ rework so I'd better spend time when it's ready. Provide specific feedback to point the flaw, why and how it should be fixed.
  * It is important to reject early so others won't waste a time. OTOH do not reject ever once accessment is passed.
  * 1st pass: Consider any major issues and bugs which may cause the contract violation, including edge cases. Provide the clear feedback and propose the fix.
  * 2nd pass: Consider "not a bug" defects and possible improvements: naming, code style, comments, code layout improvements, etc.
Now the committer is supposed to address the reviewer comments and issues. 
_Committer:_  once assessment is passed, it is impportant that you do not provide any changes beside of those requested in the reviewer's feedback. If you feel you have to rework then revoke the commit and start over. It's not right time for improvements, provide a separate commit instead.
* 2nd revision: no more assessment! Found defects fixed or postponed.
  * _Committer_ is supposed to address the issues found. You may provide the fix or postpone the defect if it is not critical and the fix may be decomposed to separate improvement. Do not postpone the issues that breaks correctness. However a partial or interim solution may make sense sometimes.
  * _Reviewer:_ as committer daes ont contribute any changes but the review feedback, you may do a quick pass to make sure your request is addressed. If the fix is inclumplete or unclear, ask yourself: was your feedback clear and specific enough? Consider direct communication to the author to ensure the next round will be the last one.
  * _Reviewer:_ If you found the issue that has not been discovered before - it's probably your fault. Or does this issue introduces lately? Was your feedback clear enough, have you proposed a good improvement? Do not block the commit by extra round of review. Consider as a separate improvenet and postpone if possible.
* 3d revision. No more time spent. Accept or reject quickly. Talk to author if needed. 

