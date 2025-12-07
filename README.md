SEMANTIC ANALYSIS
It has been created a Python semantic analysis script whose primary goal is to calculate the semantic correlation between all CAF 2020 model examples, using their embedding vectors previously generated and saved in a CSV file (using another python script).
The final function of the script is to produce a cosine similarity matrix that quantifies how semantically related each CAF example is to all the others.
The output provides highly valuable insights into the CAF 2020 criteria, revealing which examples serve as central hubs for the entire framework.
🧠 Analysis of Results
Here's a breakdown of what the analysis reveals and why the identified hubs are significant:
The restriction to the first 5 correlations (at point 1) does not affect the computation of the entire similarity matrix or the construction of the network graph.
This restriction is used exclusively to display a small portion of the matrix for the following purposes:
• Sanity Check: Displaying the first values of the matrix is used for a quick check that the cosine similarity computation was successful and that the generated values (which should be close to 1.0 on the diagonal) make sense.
• Concise Presentation: Printing the entire matrix, especially with a large number of examples, would be unmanageable and unnecessary. Displaying only the top-left corner provides a sense of the data format without cluttering the output.
________________________________________
1. Semantic Correlation
The similarity_matrix confirms the embedding quality:
•	High Intra-Criterion Similarity: The first five examples (C1.1.a through C1.1.e) are all under Criterion 1 (Leadership), Subcriterion 1.1 ("Provide direction for the organisation..."). The similarity scores between them are extremely high, ranging from 0.812 to 0.921. This validates that the Gemini embeddings accurately group texts with the same topic and context (Leadership/Direction).
•	The highest correlation is C1.1.c vs. C1.1.e (0.921):
o	C1.1.c: Ensure that mission, vision and values are in line with local, national, international and supranational strategies...
o	C1.1.e: Ensure organisational agility by periodically reviewing the mission, vision, values and strategies reflecting changes in the external environment...
o	This makes perfect sense: Aligning strategies (C1.1.c) is semantically very close to reviewing/adjusting strategies (C1.1.e) to stay relevant.
________________________________________

2. Central Hubs
The "Top 5 Examples (Hubs)" are the most semantically interconnected examples across the entire CAF framework, connecting different criteria and concept groups (Enablers and Results).
Rank	ID	Criterion	Text Summary	Centralità (Degree Centrality)
1	C1.2.e	Leadership (1.2)	Internal and external communication...	0.6061
2	C1.4.c	Leadership (1.4)	Align the organisation’s performance to public policies...	0.5202
3	C2.4.d	Strategy & Planning (2.4)	Manage change effectively and inform and involve employees...	0.5202
4	C5.1.b	Processes (5.1)	Match processes on a regular basis to the needs and expectations of employees and stakeholders...	0.5152
5	C7.1.f	People Results (7.1)	The organisation‘s openness for change and innovation...	0.5101
The most central example is C1.2.e (Communication), with a centrality score of 0.6061, meaning it is semantically related (above the 0.8 threshold) to about 60% of all other examples in the entire CAF model.
The Significance of C1.2.e: Communication (The Master Key)
Effective communication is revealed as the single most crucial enabling activity (Enabler) that connects to success in every other area of the CAF model. It underpins:
•	Results: Communicating performance and results to stakeholders.
•	People: Informing and involving employees (C2.4.d).
•	Strategy: Aligning the organization with policy (C1.4.c).
•	Processes: Matching processes to stakeholder needs (C5.1.b).
________________________________________
 
QUALITATIVE ANALYSIS

Qualitative analysis is the step that transforms numerical data (embeddings and correlations) into conceptual and interpretable information.
🧠 Qualitative Analysis of the CAF Hub: C1.2.e (Communication)
The text of example C1.2.e is: "Ensure good internal and external communication in the whole organisation and use new means of communication."
The similarity analysis identified this element as the most connected (Hub) in the semantic network, highlighting its crucial role in connecting the concepts of "Enablers" and "Results" in the CAF 2020 model.
________________________________________
1. Connection with "Enablers" 
The Enablers (Criteria 1-5) describe what the organization does and how it does it. Communication is essential to activate and coordinate all these factors:
•	C1 (Leadership): Leadership must communicate the mission, vision, and strategic changes (as evidenced by your initial high correlations). Without good communication, direction remains theoretical.
•	C2 (Strategy and Planning): Strategic plans must be communicated in clear operational objectives at all levels. Example C2.4.d (Change Management and Engagement) emerged as a hub, confirming that change must be communicated promptly and with stakeholder involvement.
•	C3 (People): Internal communication is the primary tool for engaging staff, managing performance, and ensuring everyone understands their roles.
________________________________________
2. Connection with "Results" 
The Results (Criteria 7-9) measure what the organization achieves. Communication is the vehicle through which results are influenced, perceived, and improved:
•	C7 (People Results): Positive results (motivation, satisfaction) directly depend on a transparent work environment and clear feedback (effective internal communication). Your hub C7.1.f (Openness to Change) is a result derived from good change communication.
•	C8 (Customer/Citizen Results): Measuring citizen satisfaction requires effective communication (surveys, feedback). Furthermore, the positive perception of services (a key result) is shaped by the organization’s external communication.
•	C9 (Key Performance Results): Results must be communicated transparently and understandably to all stakeholders to ensure accountability and trust.
________________________________________

🔑 Conclusion: Communication as a Cross-Cutting Element
C1.2.e is not just a Leadership criterion; it is the common thread that translates the Enablers' intention into the impact of the Results.
Its high centrality (0.6061) in your analysis demonstrates that in the CAF model, communication is the management activity that has the greatest semantic resonance with the largest number of other concepts. It is the element that makes the other criteria operational and the results visible.
 
 

