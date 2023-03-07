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
    <h2 id="introduction">Knowledge Graph Construction</h2>
    <div>
        <div>
        </div>
        <div class="home-highlight">
            Graphlet AI is a data engineering, data science and artificial intelligence consultancy specializing in <i>knowledge graph construction</i>, also known as <b>property graph construction</b>. We transform and refine raw data on your data lake to build large networks ranging in the millions, billions or even trillions of nodes and edges that model entire business domains to solve complex problems with global footprints. We use big data tools and go beyond simple ETL by using machine learning and artificial intelligence to construct a graph model of your business domain that maps closely to solutions to your business problems. Using a modern graph database, your data science and machine learning teams can then efficiently mine this refined graph to find solutions to your most pressing data science problems.
        </div>
    </div>
</div>
<div class="problem-definition">
    <div>
        <div style="margin-top: 2%;"></div>
        <h2>We build knowledge graph <i>factories</i></h2>
        <div>
            <center>
                <img style="width: 80%; margin-top: 1%;" alt="Knowledge Graph Construction Architecture" src="assets/slides/KG-Factory-System-Architecture-Diagram.jpg" />
            </center>
        </div>
        <div style="margin-top: 3%;"></div>
        <h2>We build <i>property graphs</i> in 3 steps</h2>
        <div style="margin-top: 2%;"></div>
        <div style="margin-bottom: 2%;">
            1) Transform myriad datasets into a common ontology. This means we Extract, Transform, Load (ETL) [or ELT] multiple, large and small datasets from different sources with different formats into a common property graph schema using tools like Python, PySpark, Databricks or Snowflake. How much ETL varies by industry from minimal with cybersecurity applications to simplified graph model with fewer makes it easy to access, query, analyze and model in a graph database such as Neo4j, TigerGraph, ArangoDB or Neptune.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-1-Bronze-ETL.png" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Transformed, Cleaned Data in Silver Tables" src="assets/slides/Entity-Resolution-Phase-1-Silver-ETL.png" />
            </center>
        <div style="margin-top: 2%;"></div>
        <div>
            <b>2)</b> Extract a graph from text using Natural Language Processing (NLP) via a chain of operations: NER —> IE —> EL. Named entity recognition (NER) points out entities corresponding to nodes. Information Extraction (IE) creates relationships [edges] between entities. Entity linking links nodes and edges extracted from text documents into single into a core graph established via ETL.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            Initially a process of exploratory data analysis (EDA) reveals patterns that can be used to handle the combinatoric problems arising from the need in entity matching to compare every node in the graph with every node. The complexity of this comparison is n^2, where n is the number of nodes. This can quickly get out of hand with millions or billions of nodes! Blocking is a strategy to prune the set of nodes compared down to groups that are more manageable.
        </div>
        <div style="margin-top: 2%;"></div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-2---Blocking.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-2---Manual-Matching.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <b>3)</b> Entity resolution using network topology and natural language processing. Recent developments in Large Language Models [LLMs] and Graph Neural Networks (GNNs) allow us to encode nodes and edges as XML-like text using a language model and then combine them based on semantic inferences made by the LLM in combination with those made about the network via a GNN. LLMs have seen many similar documents as the nodes’ text representation on the world wide web.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            Manual blocking and matching for numerous datasets is a cumbrsome and expensive activity. Advances in AI - representation learning and an architecture from Google called Grale - make a generic entity resolution (ER) system possible. This system is configurable to work across multiple datasets by embedding records using large language models (LLMs) such as GPT-3 or ChatGPT, but tuned specifically for the entity matching task.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution---Ditto-Encoding.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-3---LSH-Blocking.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-3---Embedding-Distance.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-3---Fine-Tuned-Classifier.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div style="margin-top: 2%;"></div>
        <div style="margin-top: 2%;"></div>
    </div>
    <div style="margin-top: 3%;" >
    </div>
    <div>
        <h2>What is a property graph, knowledge graph and triple store?</h2>
        <div>
            A property graph is a set of objects representing nodes [also known as vertex/vertices] and edges [also known as links].
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 80%;" alt="Property graphs vs RDF Triples. Both are knowledge graphs." src="assets/slides/RDF-Triple-Stores-vs-Property-Graphs.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <h2>Why should I build a knowledge graph for my business?</h2>
        <div>
            I'll let you in on a secret that is driving the popularity of enterprise knowledge graphs, property graphs, graph databases and Graph Neural Networks (GNNs): MOST DATA IS GRAPH DATA. To compose a single table to get the corresponding vectors, matrices and tensors we load into GPUs to drive machine learning algorithms, several tables have usually been combined [squashed] into one table. There's a problem with this... it is a lossy process. We threw away the relationships. Graph neural networks are able to learn better to build more powerful models because they have a greater potential by matching the structure of the data’s entities and their relationships.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 900px;" alt="" src="assets/home/types_of_graph.png">
            </center>
        </div>
    </div>
    <!-- Next section -->
    <div>
        <div style="margin-top: 2%;"></div>
        <h2>What’s the real story with Graph Neural Networks (GNNs)?</h2>
        <div>I'll let you in on a secret that is driving the popularity of enterprise knowledge graphs, property graphs, graph databases and Graph Neural Networks (GNNs): MOST DATA IS GRAPH DATA. To compose a single table to get the corresponding vectors, matrices and tensors we load into GPUs to drive machine learning algorithms, several tables have usually been combined [squashed] into one table. There's a problem with this... it is a lossy process. We threw away the relationships. Graph neural networks are able to learn better to build more powerful models because they have a greater potential by matching the structure of the data’s entities and their relationships.
        </div>
        <div style="margin-top: 2%;"></div>
            <div>
                <center>
                    <img style="width: 900px;" alt="Property Graphs vs Triple Stores: Reification, making objects out of properties" src="assets/home/different_types_of_networks.png">
                </center>
            </div>
    </div>
    <div>
        <div style="margin-top: 2%;"></div>
        <h2>I use a certain tool or platform. Can you help me?</h2>
        <div>
            We can build knowledge graphs for any platform, but here are a few tools that are more up our alley to create business value using graphs and networks:
        </div>
        <li>
            <ul>Python tools like <a href="https://pandas.pydata.org/">Pandas</a> and <a href="https://networkx.org/">NetworkX</a>, <a href="https://graph-tool.skewed.de/">graph-tool</a>, <a href="https://networkit.github.io/">NetworKit</a> or <a href="https://www.graphifi.com/easygraph">EasyGraph</a></ul>
            <ul><a href="https://www.r-project.org/">R</a> tools like <a href="https://igraph.org/">iGraph</a>, <a href="https://tidygraph.data-imaginist.com/">tidygraph</a> and <a href="https://ggraph.data-imaginist.com/">ggraph</a></ul>
            <ul>Big data tools like <a href="https://spark.apache.org/docs/latest/api/python/">PySpark</a>, <a href="https://www.databricks.com/">Databricks</a>, <a href="https://www.dask.org/">Dask</a>, <a href="https://www.snowflake.com/en/">Snowflake</a>  or <a href="https://graphframes.github.io/graphframes/docs/_site/index.html">GraphFrames</a></ul>
            <ul>GPU-accelerated compute tools like RAPIDS <a href="https://github.com/rapidsai/cugraph">cuGraph</a></ul>
            <ul>Property graph databases like <a href="https://neo4j.com/">Neo4j</a>, <a href="https://www.tigergraph.com/">TigerGraph</a>, <a href="https://www.arangodb.com/graph-database/">ArangoDB</a>, <a href="https://www.oracle.com/">Oracle Graph Studio</a> or Oracle Graph Studio</ul>
            <ul>Enterprise knowledge graphs that use RDF Triple Stores / SPARQL like <a href="https://www.stardog.com/">StarDog</a> or <a href="https://www.ontotext.com/">Ontotext</a></ul>
            <ul>Large knowledge bases like <a href="https://query.wikidata.org/">WikiData Query Service</a></ul>
            <ul><a href="https://jupyter.org/">Jupyter</a>, <a href="https://www.databricks.com/">Databricks</a> and <a href="https://www.snowflake.com/en/">Snowflake</a> Notebooks</ul>
            <ul>Natural Language Processing (NLP) users of tools such as <a href="https://spacy.io/">spaCy</a>, <a href="https://github.com/flairNLP/flair">FlairNLP</a>, <a href="https://blinkforhome.com/">BLINK</a>, <a href="https://radimrehurek.com/gensim/">Gensim</a> or <a href="https://www.nltk.org/">NLTK</a></ul>
            <ul>Network visualization tools like <a href="https://gephi.org/">Gephi</a>, <a href="https://www.graphistry.com/">Graphistry</a> or <a href="https://cambridge-intelligence.com/keylines/">Cambridge Intelligence Keylines</a> / <a href="https://cambridge-intelligence.com/regraph/">ReGraph</a></ul>
        </li>
    </div>
    <div>
        <h2>Principal Consultant</h2>
        <div>
            My name is Russell Jurney. I work at the intersection of big data, large networks - property graphs or knowledge graphs, representation learning with Graph Neural Networks (GNNs), Natural Language Processing (NLP) and Understanding (NLU), model explainability using network visualization and vector search for information retrieval.
            I am a startup product and engineering executive focused on building products driven by billion node+ networks. I have worked at cool places like Ning, LinkedIn and Hortonworks. I co-founded Deep Discovery to use networks, GNNs and visualizations to build an explainable risk score for KYC / AML.
        </div>
        <div>
            I am a four-time O'Reilly author with 120 citations on Google Scholar for being the first to write about “agile data science” - agile development as applied to data science and machine learning. I am an applied researcher and product manager with 17 years of experience building and shipping data-driven products.
        </div>
        <div>
            I am currently fascinated by knowledge graph / property graph construction, graph representation learning, graph neural networks (GNNs), NLP/NLU techniques such as information extraction, named entity resolution (NER), coreference resolution, fact extraction, and entity linking. I do network science and machine learning - so I get stuff done :)
            Check out my network science portfolio, my blog and my O’Reilly Radar posts.
        </div>
    </div>
</div>