# AI Fairness for People with Disabilities: Point of View
_S Trewin_
---

Main idea: Fairness with relation to disabilities is much different than for other protected classes for two main reasons: the diversity of ways in which disabilities can manifest themselves, and the typically hidden/unshared nature of disability. This leads to a lack of data which of course affects the bias of any datasets and therefore, models.

This paper looks at different forms of fairness and how those might work in the disability space, as well as how to approach this problem.

Bias in this case comes from a combination of systemic bias, lack of representation in datasets (1 in 5 Americans have some form of disability, but these might not be identified/included in datasets), and the measurement of proxy characteristics rather than true objectives (e.g. test taking time rather than actual level of skill).

The disabled community contains many outliers, which often are dropped as "noise" from datasets. It is not easy to determine or gather a "balanced" dataset because of the multiple forms and degrees of disability.

People often keep their disability information private due to fears of discrimination.

With speech and communication systems, the primary concern is algorithmic fairness, i.e. "the models should work equally well for membrs of different groups."

For algorithms that place people into favored or less-favored groups, allocative fairness is the concern, through one of:
	- Fairness through unawareness (no information about protected attributes is gathered or used in the decision-making process)
	- Fairness through awareness (membership in a protected group is known, and fairness can be formally defined and enforced)
	- Group fairness (the proportion of selected individuals in the protected group should be approximately the same as those in the non-protected group)
	- Individual fairness (similar individuals should have similar outcomes. BUT, what's a fair similarity metric?)