---
title: Mathematica Notes
date: 2021-06-28
categories:
- Mathematica
---

### Load and Use FeynCalc and LoopTools The Same Time
```Mathematica
Block[{$ContextPath}, 
    BeginPackage["LoopTools`"];
    Install["LoopTools"];
    EndPackage[];
    ];
<< FeynCalc`
```