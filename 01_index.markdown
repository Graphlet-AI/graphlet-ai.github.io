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
    <div style="margin-top: -5%;"></div>
    <h2 id="introduction">Knowledge Graph Construction</h2>
    <div>
        <div>
            Graphlet AI is a data engineering, data science and artificial intelligence consultancy specializing in <i>knowledge graph construction</i>, also known as <b>property graph construction</b>. We build data pipelines that take raw data and feed your graph database clean data. We transform and refine raw data on your data lake to build large networks ranging in the millions, billions or even trillions of nodes and edges that model entire business domains to solve complex problems with global footprints.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            We love big data and large networks. We use big data tools to scale data pipelines that go beyond traditional ETL and entity resolution using artificial intelligenecs - graph machine learning - to construct a high fidelity network model of your business domain that maps directly to solutions to your business problems. It lets you run the queries that answer problems vexing you and driving features your customers demand. Using a modern graph database, your data science and machine learning teams can then efficiently mine this refined graph to find solutions to your most pressing data science problems.
        </div>
    </div>
</div>
<div class="problem-definition">
    <div>
        <div style="margin-top: 3%;"></div>
        <center><h2>We build property graph <i>factories</i></h2></center>
        <div>
            <center>
                <img style="width: 70%; margin-top: 1%;" alt="Knowledge Graph Construction Architecture" src="assets/slides/KG-Factory-System-Architecture-Diagram.jpg" />
            </center>
        </div>
        <div style="margin-top: 4%;"></div>
        <h2>Property graph factories build <i>property graphs</i> in <b>4 steps</b>...</h2>
        <div style="margin-top: 2%;"></div>
        <h3>Step 1) Extract, Transform, Load Datasets to a Common Format</h3>
        <div>
            The first step in building an enterprise knowledge graph is to build the raw node and edge lists making up your network by combining multiple, structured datasets from your organization into a common schema. In larger domains this will warrant a full blown ontology, but starting with a smaller network and building out one use case is a good strategy.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            We Extract, Transform, Load (ETL) multiple, large and small datasets from different sources with different formats into a common property graph schema using tools like Python, Spark, Databricks or Snowflake. How much ETL varies by industry from relatively little in cybersecurity applications to a significant amount with business graph applications like KYC /AML / financial compliance. A well defined graph model with fewer makes it easy to access, query, analyze and model your business domain in a graph database such as Neo4j, TigerGraph, ArangoDB or Neptune.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            Why not load your raw data directly into a graph database and do ETL inside it? Graph databases aren't ETL platforms. They are not designd for it. Python based tools are. Modern ETL increasingly involves using machine learning techniques rather than simple transformations. Graph databases are typically build on top of the Java Virtual Machine (JVM) or C++. Ask your data engineers how productive they will be doing ETL in Python versus Java or C++. Python shines at ETL. The JVM and C++ shine at interactively querying clean graph data.
        </div>
        <div style="margin-top: 2%;"></div>
        <h4>Adding Unstructured Data</h4>
        <div>
            Once a core knowledge graph built from structured datasets is established, then it is time to bring in unstructured datasets to extend that network to a larger knowledge base using Natural Language Processing (NLP). Starting with unstructured data can be much more difficult - there is no anchor on which to peg the entities [nodes] and relationships [edges] you extract from text.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-1-Bronze-ETL.png" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Transformed, Cleaned Data in Silver Tables" src="assets/slides/Entity-Resolution-Phase-1-Silver-ETL.png" />
            </center>
        <div style="margin-top: 3%;"></div>
        <h3>Entity Resolution (ER): Node and Edge Deduplication</h3>
        <div>
            Entity Resolution (ER) is the process of deduplicating and combining duplicate nodes and splitting up mistakenly merged nodes. In a similar manner, edges can also be merged or split up. This is important as it is difficult to detect patterns in networks if there are disconnected duplicates that are each a part of different, important relationships.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Clean Data in Silver Tables" src="assets/slides/Entity-Resolution-Enables-Motif-Search.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <h4>Manual Block and Match</h4>
        <div>
            Traditional entity resolution involves two phases: blocking and matching. Querying data as part of exploratory data analysis (EDA) reveals strategies to match records. This was traditionally done by hand, and it still can be for a limited number of small datasets.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            The next step is to compare records for matching. This presents a problem. The naive complexity of comparing every node with every other node is n^2 / 2, where n is the number of nodes. This can quickly get out of hand with millions or billions of nodes! Blocking is a strategy to prune the set of nodes compared down to groups that are more manageable.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-2---Blocking.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Clean Data in Silver Tables" src="assets/slides/Entity-Resolution-Phase-2---Manual-Matching.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <h4>Automatic Deduplication</h4>
        <div>
            When dealing with big data, especially when there are a a number of datasets large and small, the traditional entity resolution model of manual blocking and matching starts to break down. It is cumbersome and takes too much developer time. What is needed is a <i>generic approach to entity resolution</i>.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>    
            Recent developments in Large Language Models [LLMs] like <a href="https://chat.openai.com/chat/">ChatGPT</a> and Graph Neural Networks (GNNs) allow us to ETL nodes and edges into XML-like text and sentence encode them using a large language model and then combine them based on semantic inferences made by the LLM in combination with the network topology. LLMs have seen many similar documents as the nodes’ text representation on the world wide web, and if we provide a few clues... they provide state of the art entity resolution for both the blocking and matching stages!
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            Manual blocking and matching for numerous datasets is a cumbersome and expensive activity. Advances in AI - representation learning and an architecture from Google called Grale - make a generic entity resolution (ER) system possible. This system is configurable to work across multiple datasets by embedding records using large language models (LLMs) such as GPT-3 or ChatGPT, but tuned specifically for the entity matching task.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution---Ditto-Encoding.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-3---LSH-Blocking.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-3---Embedding-Distance.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Raw Data in Bronze Tables" src="assets/slides/Entity-Resolution-Phase-3---Fine-Tuned-Classifier.jpg" />
            </center>
        </div>
        <div style="margin-top: 3%;"></div>
        <h3>Step 4) Pattern Matching: Network Motif Search</h3>
        <div style="margin-top: 2%;"></div>
        <div>
            While it is nice to think that a single version of your data can be encoded in a graph, the reality is that you must make decisions as to which business logic to encode in the representation you choose for your knowledge graph.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Multiple chain indirect ownership is a way of tracking Ultimate Beneficial Ownership (UBO)" src="assets/slides/Multiple-Path-Indirect-Ownership-Motif.jpg" />
            </center>
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="A business graph risk motif showing how an incorporation services company was purchased and used to create fake companies to launder money." src="assets/slides/Corrupt-Incorporation-Services-Motif.jpg" />
            </center>
        </div>
    </div>
    <div style="margin-top: 3%;" >
    <div>
        <h2>How can a graph model my data?</h2>
        <div>
            Property graphs can represent data from any database you throw at them. They are objects and their relationships just like the world around us. Objects have properties just like a baseball has a width. Relationships can as well, just like a pitch between a pitcher and batter has a speed.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Property graph model" src="assets/slides/Property-Graph-Models.jpg" />
            </center>
        </div>
        <div style="margin-top: 4%;"></div>
        <div>
            You may be used to thinking of graphs as simple, mathematical concepts but property graphs have different types of nodes and edges that are much more powerful for data science and artificial intelligence than simple graphs are.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 900px;" alt="Simple vs property graphs" src="assets/slides/Heterogeneous-Graph-Diagram.png">
            </center>
        </div>
    </div>
    <div>
        <div style="margin-top: 2%;"></div>
        <h2>What is a property graph, knowledge graph and triple store?</h2>
        <div>
            A property graph is a set of objects representing nodes [also known as vertex/vertices] and edges [also known as links].
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 70%;" alt="Property graphs vs RDF Triples. Both are knowledge graphs." src="assets/slides/RDF-Triple-Stores-vs-Property-Graphs.jpg" />
            </center>
        </div>
        <div style="margin-top: 3%;"></div>
        <h2>What is graph machine learning (graph ML)? What is a GNN?</h2>
        <div>
            I'll let you in on a secret that is driving the popularity of enterprise knowledge graphs, property graphs, graph databases and Graph Neural Networks (GNNs): MOST DATA IS GRAPH DATA. To compose a single table to get the corresponding vectors, matrices and tensors we load into GPUs to drive machine learning algorithms, several tables have usually been combined [squashed] into one table. There's a problem with this... it is a lossy process. We threw away the relationships. Knowledge graphs modeled using graph machine learning (Graph ML) and graph neural networks (GNNs) are able to learn better to build more powerful models because they have a greater potential by matching the structure of the data’s entities and their relationships.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            <center>
                <img style="width: 900px;" alt="Networks vs sequence representations. Networks preserve inherent relational bias of data" src="assets/home/different_types_of_networks.png">
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
        <div style="margin-top: 2%;"></div>
        <h2>Our Principal Consultant, <a href="https://www.linkedin.com/in/russelljurney/">Russell Jurney</a></h2>
        <img align="left" style="margin-left: 0%; margin-right: 2%; width: 17%" src="assets/home/russell_jurney_headshot.jpg" alt="The beautiful face of Russell Jurney. Bald. Shiny." />
        <div>
            My name is Russell Jurney. I work at the intersection of big data, large networks - property graphs or knowledge graphs, representation learning with Graph Neural Networks (GNNs), Natural Language Processing (NLP) and Understanding (NLU), model explainability using network visualization and vector search for information retrieval.
            I am a startup product and engineering executive focused on building products driven by billion node+ networks. I have worked at cool places like Ning, LinkedIn and Hortonworks. I co-founded Deep Discovery to use networks, GNNs and visualizations to build an explainable risk score for KYC / AML.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            I am a four-time O'Reilly author with 122 citations on Google Scholar for being the first to write about “agile data science” - agile development as applied to data science and machine learning. I am an applied researcher and product manager with 17 years of experience building and shipping data-driven products.
        </div>
        <div style="margin-top: 2%;"></div>
        <div>
            I am currently fascinated by knowledge graph / property graph construction, graph representation learning, graph neural networks (GNNs), NLP/NLU techniques such as information extraction, named entity resolution (NER), coreference resolution, fact extraction, and entity linking. I do network science and machine learning - so I get stuff done :)
            Check out my network science portfolio, my blog and my O’Reilly Radar posts.
        </div>
    </div>
</div>