---
layout: single
classes: wide
title: Evaluation
permalink: /evaluation/
author_profile: true
author: Billy Rick
---

Metrics for cell annotation-specific functional enhancer prediction aim to characterize how well the ranked list of enhancers correspond to experimentally validated enhancer collections.

Rank adjusted scoring (RAS): Let modelRankenhancerj,kbe the rank of enhancer for a given team where $k\inK$ is the set of all cell annotations, $onTargetenhancer_i,k$ indicate experimentally validated on-target enhancers and $offTargetenhancer_i,k$ indicate experimentally validated off-target enhancers. For reference on enhancer scoring please go to our (Experimental validation)[LINK] page.

Then each model is scored as follows:

$$ RAS = KI  modelRankenhanceri,k *I(onTargetenhanceri,k | offTargetenhanceri,k) 

			Where:
				I(onTarget)           = 1
				I(on/offTarget)  = -1
				I(offTarget)         = -1$$
