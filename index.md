---
layout: default
title: Home
---

# Oops!... I did it again

Supplementary Website

## Abstract

Mining software repositories is a popular means to gain insights into
a software project’s evolution, monitor project health, support decisions and
derive best practices. Tools supporting the mining process are commonly applied by 
researchers and practitioners, but their limitations and agreement are
often not well understood.

This study investigates some threats to validity in complex tool
pipelines for evolutionary software analyses and evaluates the tools’ agreement 
in terms of data, study outcomes and conclusions for the same research
questions.

We conduct a lightweight literature review to select *three* studies
on collaboration and coordination, software maintenance and software quality
from high-ranked venues, which we formally replicate with *four* independent,
systematically selected mining tools to quantitatively and qualitatively compare 
the extracted data, analysis results and conclusions.

We find that numerous technical details in tool design and implementation accumulate
along the complex mining pipelines and can cause substantial differences in the 
extracted baseline data, its derivatives, subsequent results
of statistical analyses and, under specific circumstances, conclusions.

Users must carefully choose tools and evaluate their limitations
to assess the scope of validity in an adequate way. Reusing tools is recommended. 
Researchers and tool authors can promote reusability and help reducing 
uncertainties by reproduction packages and comparative studies following
our approach.

## Study repository

Visit our [git repository](https://github.com/nicolehoess/emse2025) to get a copy of 
the reproduction setup including the tool snapshots of 
[Codeface](https://github.com/lfd/codeface),
[git2net](https://github.com/gotec/git2net),
[GrimoireLab](https://github.com/chaoss/grimoirelab) and
[Kaiaulu](https://github.com/sailuh/kaiaulu)
as well as all scripts for
data extraction, processing, study reproduction, results comparison and visualisation.

## Supplementary material

For analyses covering multiple subject projects or experiments, 
we provide supplementary material which is not included in the publication.

### Literature review

The annotated tools table can be found here: [tools.xlsx](/literature/tools.xlsx)

The annotated venue lists can be found here:
- [emse.xlsx](/literature/emse.xlsx)
- [fse.xlsx](/literature/fse.xlsx)
- [icse.xlsx](/literature/icse.xlsx)
- [msr.xlsx](/literature/msr.xlsx)
- [saner.xlsx](/literature/saner.xlsx)
- [tosem.xlsx](/literature/tosem.xlsx)
- [tse.xlsx](/literature/tse.xlsx)

Study counts for the categories are summarised here: [plot_summary.csv](/literature/plot_summary.csv)

### Collaboration and coordination

#### Agreement of count- and network-based operationalisations

The agreement plots for all subject projects and analysis ranges are available [here](/collaboration/index.html#metrics-agreement).

Example:
![Agreement for subject project GCC](/collaboration/gcc_agreement_107-104.png)

#### Hierarchy stability

The agreement plots for all subject projects and analysis ranges are available [here](/collaboration/index.html#hierarchy-stability).

Example:

![Hierarchy stability for subject project GCC](/collaboration/gcc_stability_107-104.png)

#### Agreement across tools per metrics

The agreement plots for all subject projects and analysis ranges are available [here](/collaboration/index.html#tools-agreement).

Example:
![Tool agreement for subject project GCC](/collaboration/gcc_tool_agreement_107-104.png)


### Software maintenance

#### Correlations

Correlation matrix (adjacency version):

![Correlation between productivity and collaboration (adjacency version)](/productivity/corr_adjacency.png)

Correlation matrix (edgelist version):

![Correlation between productivity and collaboration (edgelist version)](/productivity/corr_edgelist.png)

#### Regression models

Linear and quadratic models (adjacency version):

![Linear and quadratic models (adjacency version)](/productivity/reg_adjacency.png)

Linear and quadratic models (edgelist version):

![Linear and quadratic models (edgelist version)](/productivity/reg_edgelist.png)

Linear and quadratic models with control variables (adjacency version):

![Linear and quadratic models with control variables (adjacency version)](/productivity/reg_adjacency_controls.png)

Linear and quadratic models with control variables (edgelist version):

![Linear and quadratic models with control variables (edgelist version)](/productivity/reg_edgelist_controls.png)


### Software quality

Correlation between turnover and bug density (with lines of code counted for all files identified by cloc):

![Correlation between turnover and bug density (cloc)](/quality/corr.png)

Correlation table (with lines of code counted for files identified by cloc *and* the MSR tool):

![Correlation between turnover and bug density (tool)](/quality/corr_filtered.png)