---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
permalink: "/"
header: Home
title: Home
head: Graphlet AI
subtitle: Knowledge Graph Factory
description: Extract, Transform, Resolve, Model, Predict, Explain
background: home/bg.png
---

 <div class="introduction">
    <h2 id="introduction">Introduction</h2>
    <div>
    <div>
        The workflow for the knowledge graph factory described below defines
        the process that enables enterprises to embrace and extend the data
        platforms they already use to build an enterprise knowledge graph with
        a uniform ontology that represents the domain in which their business
        operates. On top of this domain specific graph they can then use graph
        intelligence to add the types of edges in the solution space that
        solve their business problems. In addition to network construction, a
        KG factory would allow companies to easily do graph search, graph
        machine learning, and the rapid development of graph neural networks
        (GNNs) to build a high fidelity model of their problem domain which
        can drive the models that automate their business processes under a
        <strong>Software 2.0</strong> model as defined by
        <strong>Ratner, Hancock and Ré.</strong> <br /><br />
        Heterogeneous knowledge graphs offer a rich domain in which to model
        your market and its problems. When combined with heterogenous
        graphlets and motifs, motif search against null models and Motif Graph
        Neural Networks, they offer an efficient way to create automated
        solutions using representation learning that builds on top of the
        domain expertise previously expressed by an organization in the form
        of graph queries. These distributed representations of the problem
        domain of a market are the core assets that drive FAANG companies… and
        is causing other enterprises to follow them in transforming their
        companies to be model first, rather than code first.
        <br /><br />
    </div>

<div class="home-highlight">
    Without a factory to make the workflow more efficient, innovative
    enterprises spend eight figure budgets on knowledge graph projects
    that fail to provide a return on investment. If a knowledge graph
    factory could make the process above 25%, 50% or 75% faster it would
    create an enormous amount of value for its users. Spending $5M instead
    of $10M to achieve an improved outcome constitutes enterprise value.
    The graph database and knowledge graph markets have long been
    frustrated by the failure of the semantic web and many enterprise
    knowledge graph factories are closed silos based on legacy technology.
    I believe the market will explode once the Python open data stack is
    easy to apply to model a problem using graph machine learning. It is
    the mission of Graphlet AI to build a Knowledge Graph Factory that
    brings network science and graph machine learning into the operations
    of enterprises across the globe.
</div>
</div>
</div>

<div class="problem-definition">
    <div>
    <h2 id="problem-definition">Problem definition</h2>

<div style="margin-bottom: 5%;">
The knowledge graph and graph database markets have long asked
themselves: why aren’t we larger? The vision of the semantic web was
that many datasets could be cross-referenced between independent graph
databases to map all knowledge on the web from myriad disparate datasets
into one or more authoritative ontologies which could be accessed by
writing SPARQL queries to hop from one knowledge graph to another. The
reality of dirty data made this vision impossible, as Cory Doctorow
outlined in his essay <strong>Metacrap</strong>.
</div>

<img src="{{site.baseurl}}/assets/home/img.png" />
<div class="img-caption">
<hr />
<p>
    1. Semantic Web was a dead end. People think in terms of objects - not
    attributes they must reify
</p>
</div>
In reality most time is spent cleaning data - graph data isn’t in the
format you need to solve your business problems. You have multiple
datasets in different formats, each with its quirks. You need to
deduplicate data using entity resolution - an unsolved problem in
commercial tools for large graphs. Even once you merge duplicate nodes and
edges, you rarely have the edge types you need to think in terms of your
problem domain to make a problem easy to solve.

<div class="highlight">
It turns out the most likely type of edge in a knowledge graph that
solves your problem with analysis is defined by the output of an entire
program - a program in Python which employs machine learning.
</div>

<div class="paper-bg">
For large graphs, this program needs to be run on a scalable platform
based on commodity machines like <strong>Databricks</strong> or
<strong>Snowflake</strong> (which are
<strong>improving using GPUs</strong>) and extend rather than rebuild
and isolate within to provide an excellent developer experience. To
create new edges in the domain of your solution, you need to compare
candidate pairs nodes that are candidates for edges in an efficient
manner. <strong>Google Grale</strong> outlines a simple blocking or
reduce mechanism for building a graph that solves your business problem
using simple graph algorithms like connected components or other types
of querying or pattern matching. It can also be the basis for graph
machine learning on a more refined graph. <br /><br />
This document outlines the broad requirements for a knowledge graph
factory that embraces the most popular open source technologies for
machine learning, big data and information retrieval and that meets the
needs of users in enterprises by extending the data platforms they
already use. This confluence of factors are they key to unlocking the
potential of the knowledge graph and graph database markets under the
auspices of graph intelligence.
</div>
</div>
</div>
