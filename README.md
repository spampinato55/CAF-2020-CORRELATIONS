+-----------------------------------------------------------------+
| AI SEMANTIC CORRELATION ANALYSIS OF                             |
|                                                                 |
| CAF 2020 MODEL                                                  |
+=================================================================+

![](./media/media/image1.png){width="6.6930555555555555in"
height="7.154166666666667in"}

A screenshot of the interactive graph

  -----------------------------------------------------------------
  SEMANTIC ANALYSIS
  -----------------------------------------------------------------

  -----------------------------------------------------------------

It has been created a Python semantic analysis script whose primary goal
is to calculate the semantic correlation between all CAF 2020 model
examples, using their embedding vectors previously generated and saved
in a CSV file (using another python script).

The final function of the script is to produce a cosine similarity
matrix that quantifies how semantically related each CAF example is to
all the others.

The output provides highly valuable insights into the **CAF 2020**
criteria, revealing which examples serve as central **hubs** for the
entire framework.

**🧠 Analysis of Results**

Here\'s a breakdown of what the analysis reveals and why the identified
hubs are significant:

The restriction to the first 5 correlations (at point 1) does not affect
the computation of the entire similarity matrix or the construction of
the network graph.

This restriction is used exclusively to display a small portion of the
matrix for the following purposes:

• Sanity Check: Displaying the first values ​​of the matrix is ​​used for a
quick check that the cosine similarity computation was successful and
that the generated values ​​(which should be close to 1.0 on the diagonal)
make sense.

• Concise Presentation: Printing the entire matrix, especially with a
large number of examples, would be unmanageable and unnecessary.
Displaying only the top-left corner provides a sense of the data format
without cluttering the output.

------------------------------------------------------------------------

**1. Semantic Correlation**

The **similarity_matrix** confirms the embedding quality:

- **High Intra-Criterion Similarity:** The first five examples (C1.1.a
  through C1.1.e) are all under **Criterion 1 (Leadership)**,
  Subcriterion 1.1 (\"Provide direction for the organisation\...\"). The
  similarity scores between them are extremely high, ranging from
  **0.812 to 0.921**. This validates that the Gemini embeddings
  accurately group texts with the same topic and context
  (Leadership/Direction).

- **The highest correlation is C1.1.c vs. C1.1.e (0.921):**

  - **C1.1.c:** Ensure that mission, vision and values are in line with
    local, national, international and supranational strategies\...

  - **C1.1.e:** Ensure organisational agility by periodically reviewing
    the mission, vision, values and strategies reflecting changes in the
    external environment\...

  - This makes perfect sense: **Aligning** strategies (C1.1.c) is
    semantically very close to **reviewing/adjusting** strategies
    (C1.1.e) to stay relevant.

------------------------------------------------------------------------

**2. Central Hubs**

The \"Top 5 Examples (**Hubs**)\" are the most semantically
interconnected examples across the *entire* CAF framework, connecting
different criteria and concept groups (Enablers and Results).

  --------------------------------------------------------------------------------------
  **Rank**   **ID**       **Criterion**   **Text Summary**               **Centralità
                                                                         (Degree
                                                                         Centrality)**
  ---------- ------------ --------------- ------------------------------ ---------------
  1          **C1.2.e**   Leadership      **Internal and external        **0.6061**
                          (1.2)           communication**\...            

  2          C1.4.c       Leadership      **Align** the organisation's   0.5202
                          (1.4)           performance to **public        
                                          policies**\...                 

  3          C2.4.d       Strategy &      **Manage change** effectively  0.5202
                          Planning (2.4)  and **inform and involve**     
                                          employees\...                  

  4          C5.1.b       Processes (5.1) **Match processes** on a       0.5152
                                          regular basis to the needs and 
                                          expectations of **employees    
                                          and stakeholders**\...         

  5          C7.1.f       People Results  The organisation's **openness  0.5101
                          (7.1)           for change and                 
                                          innovation**\...               
  --------------------------------------------------------------------------------------

The most central example is **C1.2.e (Communication)**, with a
centrality score of **0.6061**, meaning it is semantically related
(above the 0.8 threshold) to about 60% of all other examples in the
entire CAF model.

**The Significance of C1.2.e: Communication (The Master Key)**

Effective communication is revealed as the **single most crucial
enabling activity** (Enabler) that connects to success in every other
area of the CAF model. It underpins:

- **Results:** Communicating performance and results to stakeholders.

- **People:** Informing and involving employees (C2.4.d).

- **Strategy:** Aligning the organization with policy (C1.4.c).

- **Processes:** Matching processes to stakeholder needs (C5.1.b).

------------------------------------------------------------------------

  -----------------------------------------------------------------
  QUALITATIVE ANALYSIS
  -----------------------------------------------------------------

  -----------------------------------------------------------------

Qualitative analysis is the step that **transforms numerical data
(embeddings and correlations) into conceptual and interpretable
information.**

**🧠 Qualitative Analysis of the CAF Hub: C1.2.e (Communication)**

The text of example **C1.2.e** is: \"Ensure good internal and external
communication in the whole organisation and use new means of
communication.\"

The similarity analysis identified this element as the most connected
(**Hub**) in the semantic network, highlighting its **crucial role** in
connecting the concepts of \"**Enablers**\" and \"**Results**\" in the
CAF 2020 model.

------------------------------------------------------------------------

**1. Connection with \"Enablers\"**

The **Enablers** (Criteria 1-5) describe what the organization does and
how it does it. Communication is **essential** to activate and
coordinate all these factors:

- **C1 (Leadership):** **Leadership** must communicate the mission,
  vision, and strategic changes (as evidenced by your initial high
  correlations). Without good communication, direction remains
  theoretical.

- **C2 (Strategy and Planning):** Strategic plans must be communicated
  in clear operational objectives at all levels.
  Example **C2.4.d** (Change Management and Engagement) emerged as a
  hub, confirming that change must be communicated promptly and with
  stakeholder involvement.

- **C3 (People):** **Internal communication** is the primary tool for
  engaging staff, managing performance, and ensuring everyone
  understands their roles.

------------------------------------------------------------------------

**2. Connection with \"Results\"**

The **Results** (Criteria 7-9) measure what the organization achieves.
Communication is the vehicle through which results are influenced,
perceived, and improved:

- **C7 (People Results):** Positive results (motivation, satisfaction)
  directly depend on a transparent work environment and **clear
  feedback** (effective internal communication). Your
  hub **C7.1.f** (Openness to Change) is a result derived from good
  change communication.

- **C8 (Customer/Citizen Results):** Measuring citizen satisfaction
  requires **effective communication** (surveys, feedback). Furthermore,
  the positive perception of services (a key result) is shaped by the
  organization's **external communication**.

- **C9 (Key Performance Results):** Results must
  be **communicated** transparently and understandably to all
  stakeholders to ensure accountability and trust.

------------------------------------------------------------------------

**🔑 Conclusion: Communication as a Cross-Cutting Element**

**C1.2.e** is not just a **Leadership** criterion; it is the **common
thread** that translates the Enablers\' intention into the impact of the
Results.

Its high **centrality (0.6061)** in your analysis demonstrates that in
the CAF model, **communication** is the management activity that has
the **greatest semantic resonance** with the largest number of other
concepts. It is the element that makes the other criteria operational
and the results visible.

  ----------------------------------------------------------------------
  **Dimensionality Reduction (t-SNE/UMAP)**
  ----------------------------------------------------------------------

  ----------------------------------------------------------------------

This step is essential for visualizing the overall conceptual structure
of the CAF model.

**Objective**: Use algorithms such as t-SNE (t-distributed Stochastic
Neighbor Embedding) or UMAP to map high-dimensional embedding vectors
onto a 2D graph.

**Insight**: The resulting graph (scatter plot) would allow you to see
natural clusters of examples based on semantic similarity and visualize
the central position of your \"**hubs**\" relative to other groups. You
could color the points according to the 9 main criteria to see if the
semantic similarity exceeds the formal boundaries of the model.

![](./media/media/image2.png){width="7.268055555555556in"
height="5.7in"}

**🖼️ Interpreting the Plot: Semantic Structure of the CAF Model**

The plot visualizes the **Semantic Structure of the CAF Model**. The
**CAF (Common Assessment Framework)** is a European quality management
instrument designed for self-assessment and continuous improvement in
public sector organizations. The model is structured around nine
criteria, further broken down into 28 sub-criteria, focusing on
*Enablers* (what an organization does) and *Results* (what it achieves).

**1. Data Points and Similarity**

- **Each dot (data point)** in the plot likely represents an individual
  concept, criterion, sub-criterion, or perhaps a document/text segment
  related to the CAF Model.

- **The proximity of the dots** signifies their semantic similarity or
  correlation in the original high-dimensional feature space (e.g., how
  often they are used together, or how related their underlying
  principles are).

**2. Clusters and Groups**

- The plot shows **distinct clusters or groupings** of colored dots.
  **Clusters** indicate groups of data points (CAF concepts/criteria)
  that share **strong similarities** in the original data.

- The **colors** are likely used to label these points based on an a
  priori category, such as the major CAF Criteria (e.g., \"Leadership,\"
  \"Strategy & Planning,\" \"Results,\" etc.).

  - **Interpretation:** The color groupings suggest that the original
    CAF criteria (or components) form **cohesive, separate clusters** in
    the semantic space. This indicates that the concepts within a single
    criterion are more strongly related to each other than they are to
    concepts in other criteria.

  - **The shape and spread** of a cluster can offer clues about the
    diversity within that group; a tight cluster means high similarity,
    while a more spread-out cluster suggests internal variation.

**3. Key Cautions for t-SNE Interpretation**

- **Distance Between Clusters:** In a t-SNE plot, the **distance between
  separate clusters is often meaningless** and can be unreliable,
  although it may give a general idea of separation. You **cannot**
  reliably conclude that the large distance between, say, the red and
  green clusters means they are *extremely* dissimilar---only that they
  are distinct groups.

- **Plot Axes:** The X and Y axes themselves **do not have a direct,
  interpretable meaning** (e.g., \"higher on the Y-axis means more
  \'result-oriented\'\"). The plot\'s value is purely in the relative
  distances between points.

- **Density and Size:** The size or density of a cluster is generally
  **not informative** of the number of points in the original data, and
  the visual clusters can be influenced by the chosen **perplexity**
  hyperparameter.

**💡 Summary of Conclusions**

The t-SNE plot successfully projects the high-dimensional semantic
structure of the CAF Model into 2D, revealing **multiple, well-separated
semantic groups** that align closely with the pre-defined categories
(represented by the colors). This suggests that the CAF Model\'s
components are **internally consistent** and **semantically distinct**
from one another, which is a sign of a well-defined and clearly
structured framework.

  ----------------------------------------------------------------------
  **A. Hierarchical Clustering Analysis (Dendrogram)**
  ----------------------------------------------------------------------

  ----------------------------------------------------------------------

Beyond the raw similarity matrix, hierarchical clustering can reveal how
examples cluster based on meaning.

- Objective: Create a Dendrogram that visualizes the semantic distance
  (dissimilarity) between all examples.

- Insight: They can be found clustering that doesn\'t perfectly match
  the CAF 9 Criteria/28 Subcriteria structure, suggesting a strong
  semantic connection that isn\'t explicit in the formal CAF structure.

The dendogram image in the next page (It is obviously recommended to use
the page zoom).

**1. 🌲 Dendrogram (The Tree Diagram)**

The upper part of the image features a **dendrogram**, which is the
visualization of the results from **hierarchical clustering**.

- **What it is:** A dendrogram is a tree-like diagram that displays the
  hierarchical relationship between objects (in this case, the nine CAF
  Criteria) and the order in which they were merged.

- **The Axes:**

  - The **leaves** (bottom) represent the individual CAF Criteria (C1
    through C9).

  - The **height of the branches (vertical lines)** represents the
    **distance or dissimilarity** between the clusters when they were
    merged. A greater height indicates a greater difference between the
    groups.

- **Interpretation of Grouping:**

  - The dendrogram shows a clear division into two major branches:

    - **Branch 1 (Left/Enablers):** The group containing C1 to C5, which
      are the **Enabler Criteria** (Leadership, Strategy & Planning,
      People, Partnerships & Resources, and Processes).

    - **Branch 2 (Right/Results):** The group containing C6 to C9, which
      are the **Result Criteria** (Citizen/Customer-oriented Results,
      People Results, Social Responsibility Results, and Key Performance
      Results).

  - **Conclusion:** This split confirms the **fundamental two-part
    structure of the CAF Model**---*Enablers* (what the organization
    does) and *Results* (what the organization achieves)---as the most
    significant division in the model\'s semantic space. This is
    visually demonstrated by the large vertical line (dissimilarity)
    required to merge the C1-C5 group with the C6-C9 group.

![](./media/media/image3.png){width="10.693055555555556in"
height="5.868055555555555in"}

**🔄 Parsing dei vettori di Embedding (pulizia forzata)...**

Vettori caricati: 199 vettori di dimensione 768.

**📊 Matrice di Similarità (Prime 5 x 5 Correlazioni):**

Example_ID C1.1.a C1.1.b C1.1.c C1.1.d C1.1.e Example_ID C1.1.a 1.000
0.812 0.850 0.899 0.855 C1.1.b 0.812 1.000 0.885 0.819 0.858 C1.1.c
0.850 0.885 1.000 0.839 0.921 C1.1.d 0.899 0.819 0.839 1.000 0.842
C1.1.e 0.855 0.858 0.921 0.842 1.000

**🔗 Analisi di Rete (Soglia \> 0.8):**

Nodi totali (Esempi): 199 Archi totali (Correlazioni significative):
4681 (coppie correlate)

**🌟 Top 5 Esempi (Hubs) - Maggiore Correlazione:**

ID: C1.2.e \| Criterio: Leadership (1.2) Testo: Ensure good internal and
external communication in the whole organisation and use new means of
commu... Centralità: 0.6061 ID: C1.4.c \| Criterio: Leadership (1.4)
Testo: Align the organisation's performance to public policies and
political decisions.... Centralità: 0.5202 ID: C2.4.d \| Criterio:
Strategy and Planning (2.4) Testo: Manage change effectively and inform
and involve employees and stakeholders at an early stage.... Centralità:
0.5202 ID: C5.1.b \| Criterio: Processes, Products, and Services (5.1)
Testo: Match the processes on a regular basis to the needs and
expectations of employees and relevant stake... Centralità: 0.5152 ID:
C7.1.f \| Criterio: People Results (7.1) Testo: The organisation's
openness for change and innovation... Centralità: 0.5101

Word processor software

**🎯 1. Analisi della Centralità per Criterio (Intra-Criterion Hubs)**

Risultati: Hubs per Criterio (Centralità calcolata solo sugli esempi
interni) Criterion_ID Hub_ID Intra_Centrality Hub_Text_Snippet 0 C1
C1.2.e 0.913043 Ensure good internal and external communicatio... 1 C2
C2.2.b 0.941176 Involve stakeholders and use information about... 2 C3
C3.2.a 0.750000 Implement a human resource development strateg... 3 C4
C4.4.g 0.666667 Ensure access to and exchange of relevant info... 4 C5
C5.1.h 0.857143 Drive process innovation and optimisation forw... 5 C6
C6.1.e 0.800000 The transparency, openness and information pro... 6 C7
C7.1.p 0.821429 The approach to social issues (e.g. flexibilit... 7 C8
C8.1.b 0.833333 The reputation of the organisation as a contri... 8 C9
C9.1.e 1.000000 Results of benchmarking (comparative analysis)...

**🌉 D. Analisi degli Elementi Ponte (Correlazione Inter-Criterio \>
0.85)**

Trovati 331 elementi ponte con Similarità \>= 0.85: Example_A_ID
Criterion_A Example_B_ID Criterion_B Similarity_Score 285 C6.1.j C6
C7.1.h C7 1.000000 292 C6.1.k C6 C7.1.g C7 0.971223 324 C7.1.g C7 C9.2.e
C9 0.965554 249 C6.1.a C6 C7.1.a C7 0.957484 295 C6.1.k C6 C9.2.e C9
0.949736 16 C1.1.d C1 C2.3.c C2 0.922356 238 C4.5.e C4 C5.1.i C5
0.920901 254 C6.1.a C6 C8.1.b C8 0.920337 206 C3.3.d C3 C7.1.d C7
0.918461 275 C6.1.i C6 C7.1.f C7 0.915911

💡 Ponte più Forte (Score 1.0000): C6.1.j (C6): \"The agility of the
organisation...\" \<\--\> C7.1.h (C7): \"The agility of the
organisation...\"

**🧊 E. Analisi degli Isolati Semantici (Centralità di Grado \< 0.1)**

Trovati 36 Isolati Semantici (Esempi con Centralità bassa): ID: C6.2.l
\| Criterio: C6 \| Centralità: 0.0152 Testo: Opening hours of the
different services (departments)... ID: C6.2.m \| Criterio: C6 \|
Centralità: 0.0152 Testo: Cost price of the services... ID: C8.2.c \|
Criterio: C8 \| Centralità: 0.0202 Testo: The amount and importance of
positive and negative media coverage... ID: C7.2.c \| Criterio: C7 \|
Centralità: 0.0253 Testo: The number of ethical dilemmas (e.g. possible
conflicts of interest) reported... ID: C7.2.d \| Criterio: C7 \|
Centralità: 0.0253 Testo: The frequency of voluntary participation in
the context of activities related to...

Do

  ----------------------------------------------------------------------
  CONCLUSIONS
  ----------------------------------------------------------------------

  ----------------------------------------------------------------------

This work is intended as an experiment to see how AI can help us explore
new territories.

A semantic analysis of the CAF 2020 model examples has been conducted,
and the results are open to discussion. I believe it is worth sharing
them because they can stimulate criticism and ideas.

I have been able to confirm that AI is above all a collaborative tool;
results emerge after long sessions of trial and error, during which
further ideas arise to be explored.

Several Python scripts, were required.

Salvatore
