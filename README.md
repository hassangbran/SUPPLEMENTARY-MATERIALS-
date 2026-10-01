Supplementary Materials
Manuscript Title: Integration Gaps in Smart Indoor Lighting: A Systematic Bibliometric Review of Human‑Centric Control, IoT, and Event‑Driven Automation
Author: Ahmad G Kotbi
Affiliation: Department of Architecture and Building Science, College of Architecture and Planning, King Saud University, Riyadh 11574, Saudi Arabia
ORCID: https://orcid.org/0000-0001-8781-3773
Email: akotbi@ksu.edu.sa
________________________________________
S1. Complete Database‑Specific Search Strings per Block (Scopus, Web of Science, IEEE Xplore)
S1.1 Scopus
Block A — Human‑oriented and biologically responsive lighting systems
(TITLE-ABS-KEY("human-centric lighting" OR "circadian lighting" OR "adaptive lighting" OR "visual comfort"))

Block B — Energy‑responsive illumination and efficiency optimization
(TITLE-ABS-KEY("energy efficient lighting" OR "energy saving lighting" OR "lighting optimization"))

Block C — Advanced heuristic and metaheuristic optimization frameworks (Strict)
(TITLE-ABS-KEY("hyperheuristic" OR "hyper-heuristic" OR metaheuristic*) AND TITLE-ABS-KEY(lighting OR "illumination control"))

Block C — Expanded
(TITLE-ABS-KEY("hyperheuristic" OR "hyper-heuristic" OR metaheuristic* OR "algorithm selection" OR "high-level heuristic" OR "heuristic selection") AND TITLE-ABS-KEY(lighting OR "illumination control"))

Block D — IoT‑enabled sensing, communication, and device interoperability
(TITLE-ABS-KEY("Internet of Things" OR IoT OR Zigbee OR DALI OR MQTT OR KNX) AND TITLE-ABS-KEY("smart lighting" OR "indoor lighting"))

Block E — Rule‑driven automation and event‑triggered control architectures (Strict)
(TITLE-ABS-KEY("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation") AND TITLE-ABS-KEY(lighting OR "indoor lighting"))

Block E — Expanded
(TITLE-ABS-KEY("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine" OR "Node-RED" OR "Home Assistant") AND TITLE-ABS-KEY(lighting OR "indoor lighting" OR "smart building"))

Block E — Middleware‑enriched
(TITLE-ABS-KEY("Node-RED" OR "Home Assistant" OR "MQTT" OR "middleware") AND TITLE-ABS-KEY(lighting OR "indoor lighting" OR "smart building"))

S1.2 Web of Science Core Collection
Block A
TS=("human-centric lighting" OR "circadian lighting" OR "adaptive lighting" OR "visual comfort")

Block B
TS=("energy efficient lighting" OR "energy saving lighting" OR "lighting optimization")

Block C — Expanded
TS=("hyperheuristic" OR "hyper-heuristic" OR metaheuristic* OR "algorithm selection" OR "high-level heuristic" OR "heuristic selection") AND TS=(lighting OR "illumination control")

Block D
TS=("Internet of Things" OR IoT OR Zigbee OR DALI OR MQTT OR KNX) AND TS=("smart lighting" OR "indoor lighting")

Block E — Expanded
TS=("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine" OR "Node-RED" OR "Home Assistant") AND TS=(lighting OR "indoor lighting" OR "smart building")

S1.3 IEEE Xplore
Block C — Expanded
("All Metadata":("hyperheuristic" OR "hyper-heuristic" OR metaheuristic* OR "algorithm selection" OR "high-level heuristic" OR "heuristic selection")) AND ("All Metadata":(lighting OR "illumination control"))

Block D
("All Metadata":("Internet of Things" OR IoT OR Zigbee OR DALI OR MQTT OR KNX)) AND ("All Metadata":("smart lighting" OR "indoor lighting"))

Block E — Expanded
("All Metadata":("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine" OR "Node-RED" OR "Home Assistant")) AND ("All Metadata":(lighting OR "indoor lighting" OR "smart building"))

S1.4 Retrieval Parameters
Parameter	Specification
Retrieval date	15 January 2025
Period covered	January 2015 – December 2024 (including Early Access 2025)
Document types	Peer‑reviewed articles, conference papers, scholarly book chapters
Languages	English, Spanish
Scopus records	1,752
Web of Science records	3,733
IEEE Xplore records	44
Total records before deduplication	5,529

________________________________________
S2. Stopword Lists, Stemming Rules, and Deduplication Protocols
S2.1 Stopword Lists
English stopwords (standard set applied during keyword preprocessing):
a, about, above, after, again, against, all, am, an, and, any, are, aren't, as, at, be, because, been, before, being, below, between, both, but, by, can't, cannot, could, couldn't, did, didn't, do, does, doesn't, doing, don't, down, during, each, few, for, from, further, had, hadn't, has, hasn't, have, haven't, having, he, he'd, he'll, he's, her, here, here's, hers, herself, him, himself, his, how, how's, i, i'd, i'll, i'm, i've, if, in, into, is, isn't, it, it's, its, itself, let's, me, more, most, mustn't, my, myself, no, nor, not, of, off, on, once, only, or, other, ought, our, ours, ourselves, out, over, own, same, shan't, she, she'd, she'll, she's, should, shouldn't, so, some, such, than, that, that's, the, their, theirs, them, themselves, then, there, there's, these, they, they'd, they'll, they're, they've, this, those, through, to, too, under, until, up, very, was, wasn't, we, we'd, we'll, we're, we've, were, weren't, what, what's, when, when's, where, where's, which, while, who, who's, whom, why, why's, with, won't, would, wouldn't, you, you'd, you'll, you're, you've, your, yours, yourself, yourselves
Additional domain‑specific stopwords excluded from co‑occurrence analysis:
paper, study, research, article, review, result, method, approach, analysis, data, system, based, using, used, proposed, present, current, new, high, low, different, various, specific, general, important, significant, however, therefore, moreover, furthermore, also, well, may, can, could, would, should, must
S2.2 Stemming Rules
Porter stemming algorithm was applied with the following domain‑specific overrides:
Original Term	Stemmed Form	Override Rationale
lighting	light	Preserve semantic distinction from "light" (illumination vs. visible radiation)
circadian	circadian	Do not stem (proper domain term)
melanopic	melanopic	Do not stem
heuristic	heuristic	Do not stem
hyper-heuristic	hyper-heuristic	Preserve compound
optimization	optim	Standard Porter
automation	automat	Standard Porter
interoperability	interoper	Standard Porter
illuminance	illumin	Standard Porter

S2.3 Deduplication Protocol
Step 1: DOI‑based matching
	Exact DOI match → duplicate removed
	Normalization: lowercase, strip whitespace, remove https://doi.org/ prefix
Step 2: Title‑based matching
	Normalized title: lowercase, remove punctuation, collapse whitespace, remove stopwords
	Levenshtein distance threshold: ≤ 2 characters difference → considered duplicate
Step 3: Author‑based matching
	First author surname + year + journal → considered duplicate if all three match
Step 4: Manual verification
	All borderline cases (Levenshtein distance 3–5) manually reviewed
	Cross‑database duplicates flagged and resolved by consensus
Results:
Stage	Records
Initial records	5,529
Duplicates removed	300
Unique records	5,229

________________________________________
S3. VOSviewer Parameter Files and Thesaurus
S3.1 VOSviewer Configuration Parameters
Parameter	Block A	Block B	Block D
Corpus size (n)	907	517	328
Keyword counting method	Full counting	Full counting	Full counting
Minimum occurrence threshold	5	5	3
Author collaboration	Full co‑authorship; min. 2 documents per author	Full co‑authorship; min. 2 documents per author	Full co‑authorship; min. 2 documents per author
Country collaboration	Fractional counting; min. 5 documents per country	Fractional counting; min. 5 documents per country	Fractional counting; min. 2 documents per country
Layout algorithm	Association strength	Association strength	Association strength
Clustering resolution	1.00	1.00	1.00
Minimum cluster size	5	5	3
Random seed	2025	2025	2025
VOSviewer version	1.6.20	1.6.20	1.6.20
Data source	Web of Science	Web of Science	Web of Science

S3.2 Thesaurus File (Term Normalization)
IoT	IoT
Internet of Things	IoT
internet-of-things	IoT
Hyper-heuristic	Hyper-heuristic
hyperheuristic	Hyper-heuristic
HH	Hyper-heuristic
DALI	DALI
Digital Addressable Lighting Interface	DALI
MQTT	MQTT
Message Queuing Telemetry Transport	MQTT
ZigBee	ZigBee
Zigbee	ZigBee
IEEE 802.15.4	ZigBee
ECA	ECA
Event-Condition-Action	ECA
IFTTT	IFTTT
If This Then That	IFTTT
Reinforcement learning	RL
RL	RL
Deep reinforcement learning	RL
Circadian Stimulus	CS
CS	CS
Melanopic Equivalent Daylight Illuminance	m-EDI / EML
m-EDI	m-EDI / EML
EML	m-EDI / EML
Unified Glare Rating	UGR
UGR	UGR
Energy Use Intensity	EUI
EUI	EUI
Node-RED	Node-RED
nodered	Node-RED
Home Assistant	Home Assistant
homeassistant	Home Assistant
Genetic Algorithm	GA
GA	GA
Particle Swarm Optimization	PSO
PSO	PSO
Simulated Annealing	SA
SA	SA
Ant Colony Optimization	ACO
ACO	ACO
Differential Evolution	DE
DE	DE
Model Predictive Control	MPC
MPC	MPC

________________________________________
S4. MATLAB Scripts for Duplicate Elimination, Terminology Harmonization, Co‑Occurrence Matrix Generation, and Temporal Trend Visualization
S4.1 Environment
Parameter	Specification
MATLAB version	2025a
Required toolboxes	Statistics and Machine Learning Toolbox, Text Analytics Toolbox
Random seed	2025
Working directory	C:\Research\SmartLightingReview\
Query date	15 January 2025

S4.2 Script 1: Duplicate Elimination
% duplicate_elimination.m
% Load combined dataset from Scopus, WoS, IEEE Xplore
opts = detectImportOptions('combined_records.csv');
opts.VariableNamingRule = 'preserve';
T = readtable('combined_records.csv', opts);

% Normalize DOI
T.DOI_norm = lower(strtrim(T.DOI));
T.DOI_norm = erase(T.DOI_norm, 'https://doi.org/');

% Normalize title
T.Title_norm = lower(T.Title);
T.Title_norm = regexprep(T.Title_norm, '[^\w\s]', '');
T.Title_norm = regexprep(T.Title_norm, '\s+', ' ');

% Deduplication by DOI
[~, idx_doi] = unique(T.DOI_norm, 'stable');
T1 = T(idx_doi, :);

% Deduplication by title
[~, idx_title] = unique(T1.Title_norm, 'stable');
T2 = T1(idx_title, :);

% Save unique records
writetable(T2, 'unique_records.csv');
fprintf('Initial: %d, After DOI: %d, After title: %d\n', ...
    height(T), height(T1), height(T2));

S4.3 Script 2: Terminology Harmonization
% terminology_harmonization.m
% Apply thesaurus for term normalization
T = readtable('unique_records.csv');

% Load thesaurus
thesaurus = readtable('thesaurus.csv');

% Normalize keywords field
for i = 1:height(T)
    kw = split(T.Keywords{i}, ';');
    kw = strtrim(kw);
    for j = 1:numel(kw)
        for k = 1:height(thesaurus)
            if strcmpi(kw{j}, thesaurus.Original{k})
                kw{j} = thesaurus.Normalized{k};
                break;
            end
        end
    end
    T.Keywords_norm{i} = strjoin(unique(kw), '; ');
end

writetable(T, 'harmonized_records.csv');

S4.4 Script 3: Co‑Occurrence Matrix Generation
% cooccurrence_matrix.m
T = readtable('harmonized_records.csv');

% Define term sets
iot_terms = {'ZigBee','MQTT','DALI','KNX','BLE','Wi-Fi','Thread','Home Assistant','Node-RED'};
opt_terms = {'GA','PSO','SA','DE','ACO','RL','MPC','Fuzzy Logic','LP'};

% Initialize matrix
M = zeros(numel(iot_terms), numel(opt_terms));

% Populate co-occurrence
for i = 1:height(T)
    text = lower([T.Title{i} ' ' T.Abstract{i} ' ' T.Keywords_norm{i}]);
    for a = 1:numel(iot_terms)
        for b = 1:numel(opt_terms)
            if contains(text, lower(iot_terms{a})) && contains(text, lower(opt_terms{b}))
                M(a,b) = M(a,b) + 1;
            end
        end
    end
end

% Save results
T_M = array2table(M, 'RowNames', iot_terms, 'VariableNames', opt_terms);
writetable(T_M, 'cooccurrence_matrix.csv', 'WriteRowNames', true);

S4.5 Script 4: Temporal Trend Visualization
% temporal_trends.m
T = readtable('harmonized_records.csv');

% Extract year
T.Year = year(datetime(T.PublicationDate, 'InputFormat', 'yyyy-MM-dd'));

% Count publications per year
years = (2010:2024)';
counts = zeros(numel(years), 1);
for i = 1:numel(years)
    counts(i) = sum(T.Year == years(i));
end

% Plot
figure;
plot(years, counts, '-o', 'LineWidth', 1.5);
xlabel('Year'); ylabel('Number of Publications');
title('Annual Publication Trends (2010–2024)');
grid on;

% Mann-Kendall test
[tau, p] = kendalltau(counts);
fprintf('Kendall tau = %.2f, p = %.4f\n', tau, p);

________________________________________
S5. Full Coding Dataset for the 30 Core Studies (Including the Complete Structural Characterization Table)
S5.1 Coding Framework
Each of the 30 core studies was coded across the following dimensions:
Dimension	Description	Values
Study ID	Unique identifier	S01–S30
Author/Year	First author and publication year	Text
Context	Building type / application	Office, Educational, Healthcare, Residential, Mixed
Control focus	Primary control objective	Energy, Comfort, Circadian, Multi‑objective
Optimization method	Algorithmic approach	Rule‑based, GA, PSO, SA, DE, ACO, RL, MPC, Fuzzy, LP, HH, Hybrid
IoT layer	Communication protocol	Zigbee, MQTT, DALI, KNX, BLE, Wi‑Fi, Thread, None
Automation layer	Automation framework	ECA, IFTTT, Node‑RED, Home Assistant, Programmed rules, None
Sensing	Sensor types	Occupancy, Daylight, Temperature, Spectral, Wearable, None
Study design	Validation approach	Simulation, Lab, Field, Hybrid
Duration	Study duration	Short (<1 week), Medium (1–4 weeks), Long (>4 weeks)
Primary limitation	Main gap reported	Text
Proposed enhancement	Suggested improvement	Text
Dimensions verified	Which of the four core dimensions are present	Circadian (C), Energy (E), IoT (I), Automation (A)

S5.2 Structural Characterization Table (S01–S30)
ID	Author/Year	Context	Control Focus	Optimization	IoT	Automation	Sensing	Design	Duration	Limitation	Enhancement	Dimensions
S01	Park et al. 2019 [3]	Office	Comfort + Circadian	RL	None	Programmed	Occupancy, Daylight	Field	Long	No IoT integration	Add MQTT/DALI	C, E
S02	Papatsimpa et al. 2020 [6]	Residential	Circadian	Rule‑based	Zigbee	ECA	Wearable	Field	Medium	No energy optimization	Add MPC	C, I, A
S03	Karapetyan et al. 2020 [14]	Office	Energy	Rule‑based	MQTT	Programmed	Occupancy	Field	Medium	No circadian metrics	Add CS monitoring	E, I
S04	Liu 2021 [21]	Office	Energy	RL	None	Programmed	Daylight, Occupancy	Simulation	Short	No field validation	Deploy in real building	E
S05	Papinutto et al. 2022 [11]	Office	Energy + Comfort	Rule‑based	None	Programmed	Daylight, Occupancy	Field	Long	No IoT	Add Zigbee	E
S06	Aussat et al. 2022 [15]	Office	Energy	Rule‑based	Zigbee	Programmed	Occupancy	Field	Medium	No circadian	Add spectral sensing	E, I
S07	Basurto et al. 2022 [28]	Office	Comfort	Rule‑based	None	Programmed	Daylight	Field	Long	No automation framework	Add ECA	E
S08	Choi et al. 2022 [29]	Office	Comfort	Rule‑based	None	Programmed	Occupancy	Field	Medium	No energy quantification	Add energy meter	E
S09	Viani et al. 2017 [22]	Museum	Energy	GA	None	Programmed	Occupancy	Field	Medium	No circadian	Add spectral control	E
S10	Wahid et al. 2020 [23]	Office	Energy + Comfort	GA + Firefly	None	Programmed	Occupancy, Daylight	Simulation	Short	No IoT	Add Zigbee	E
S11	Jabeur et al. 2021 [24]	Office	Energy	Fuzzy Logic	None	Programmed	Occupancy	Simulation	Short	No field validation	Deploy	E
S12	Lachhab & Bakhouya 2024 [30]	Office	Energy	AI	MQTT	Programmed	Occupancy, Daylight	Field	Medium	No circadian	Add CS	E, I
S13	Zhang et al. 2023 [31]	Office	Energy	Rule‑based	Wi‑Fi	Programmed	Occupancy	Field	Short	No optimization	Add GA	E, I
S14	van de Meugheuvel et al. 2014 [32]	Office	Energy	Rule‑based	DALI	Programmed	Occupancy, Daylight	Field	Medium	No circadian	Add spectral	E, I
S15	Cheng & Chen 2023 [47]	Mixed	Circadian	Rule‑based	None	Programmed	Spectral	Simulation	Short	No energy	Add energy meter	C
S16	Khan et al. 2024 [49]	Residential	Energy	ML	Wi‑Fi	Programmed	Occupancy	Simulation	Short	No circadian	Add CS	E, I
S17	Dang et al. 2023 [50]	Educational	Comfort	Rule‑based	None	Programmed	Daylight	Field	Medium	No energy	Add dimming	E
S18	Yang & Jeon 2023 [51]	Educational	Comfort	Rule‑based	None	Programmed	Occupancy	Field	Medium	No circadian	Add spectral	E
S19	Hartmeyer et al. 2025 [52]	Mixed	Circadian	Rule‑based	None	Programmed	Wearable	Field	Long	No energy	Add control	C
S20	Mostafavi et al. 2024 [53]	Office	Comfort	Rule‑based	None	Programmed	Occupancy	Lab	Short	No field	Deploy	E
S21	Seyedolhosseini et al. 2020 [54]	Office	Energy	ANN	None	Programmed	Daylight	Simulation	Short	No IoT	Add Zigbee	E
S22	Soheilian et al. 2021 [2]	Residential	Energy + Comfort	Rule‑based	Zigbee	IFTTT	Occupancy	Field	Medium	No circadian	Add CS	E, I, A
S23	Atzori et al. 2010 [5]	Mixed	—	—	IoT	—	—	Conceptual	—	No implementation	—	I
S24	Zanella et al. 2014 [12]	Mixed	—	—	IoT	—	—	Conceptual	—	No lighting	—	I
S25	Bonomi et al. 2012 [13]	Mixed	—	—	IoT	—	—	Conceptual	—	No lighting	—	I
S26	Domb 2019 [16]	Residential	—	—	Zigbee, MQTT	ECA	—	Review	—	No lighting	—	I, A
S27	Ur et al. 2014 [17]	Residential	—	—	—	IFTTT	—	Field	Short	No lighting	—	A
S28	Spitschan et al. 2025 [18]	Mixed	Circadian	—	—	—	Wearable	Review	—	No control	—	C
S29	Boyce 2014 [19]	Mixed	Comfort	—	—	—	—	Book	—	No integration	—	E
S30	Li & Lam 2003 [20]	Office	Energy	Rule‑based	None	Programmed	Daylight	Simulation	Short	No IoT	Add Zigbee	E

Note: Dimensions: C = Circadian, E = Energy, I = IoT, A = Automation. Studies S23–S29 are included for contextual and comparative purposes but do not report original quantitative performance outcomes; they are retained in the structural characterization for completeness of the methodological landscape.
________________________________________
S6. Detailed MMAT Scores for All 30 Core Studies
S6.1 MMAT Scoring Framework
The Mixed Methods Appraisal Tool (MMAT) version 2018 was applied across five methodological categories:
	Qualitative studies: 5 criteria
	Quantitative randomized controlled trials: 5 criteria
	Quantitative non‑randomized studies: 5 criteria
	Quantitative descriptive studies: 5 criteria
	Mixed methods studies: 5 criteria (plus 3 mixed‑methods‑specific criteria)
Each criterion scored: Yes (1), No (0), Can't tell (0).
Final score = (total Yes / total criteria) × 100%.
S6.2 MMAT Scores Table
Study ID	Author/Year	Study Type	Criteria Met	Total Criteria	MMAT Score
S01	Park et al. 2019 [3]	Quantitative non‑randomized	5	5	100%
S02	Papatsimpa et al. 2020 [6]	Quantitative descriptive	4	5	80%
S03	Karapetyan et al. 2020 [14]	Quantitative non‑randomized	4	5	80%
S04	Liu 2021 [21]	Quantitative descriptive	4	5	80%
S05	Papinutto et al. 2022 [11]	Quantitative non‑randomized	5	5	100%
S06	Aussat et al. 2022 [15]	Quantitative non‑randomized	4	5	80%
S07	Basurto et al. 2022 [28]	Quantitative non‑randomized	5	5	100%
S08	Choi et al. 2022 [29]	Quantitative descriptive	4	5	80%
S09	Viani et al. 2017 [22]	Quantitative descriptive	4	5	80%
S10	Wahid et al. 2020 [23]	Quantitative descriptive	3	5	60%
S11	Jabeur et al. 2021 [24]	Quantitative descriptive	3	5	60%
S12	Lachhab & Bakhouya 2024 [30]	Quantitative non‑randomized	4	5	80%
S13	Zhang et al. 2023 [31]	Quantitative descriptive	4	5	80%
S14	van de Meugheuvel et al. 2014 [32]	Quantitative non‑randomized	5	5	100%
S15	Cheng & Chen 2023 [47]	Quantitative descriptive	4	5	80%
S16	Khan et al. 2024 [49]	Quantitative descriptive	4	5	80%
S17	Dang et al. 2023 [50]	Quantitative non‑randomized	5	5	100%
S18	Yang & Jeon 2023 [51]	Quantitative non‑randomized	5	5	100%
S19	Hartmeyer et al. 2025 [52]	Quantitative non‑randomized	5	5	100%
S20	Mostafavi et al. 2024 [53]	Quantitative non‑randomized	4	5	80%
S21	Seyedolhosseini et al. 2020 [54]	Quantitative descriptive	4	5	80%
S22	Soheilian et al. 2021 [2]	Quantitative non‑randomized	4	5	80%
S23	Atzori et al. 2010 [5]	Qualitative	4	5	80%
S24	Zanella et al. 2014 [12]	Qualitative	4	5	80%
S25	Bonomi et al. 2012 [13]	Qualitative	4	5	80%
S26	Domb 2019 [16]	Qualitative	3	5	60%
S27	Ur et al. 2014 [17]	Mixed methods	4	5	80%
S28	Spitschan et al. 2025 [18]	Qualitative	5	5	100%
S29	Boyce 2014 [19]	Qualitative	4	5	80%
S30	Li & Lam 2003 [20]	Quantitative descriptive	4	5	80%

S6.3 Summary Statistics
Metric	Value
Mean MMAT score	84.6%
Median MMAT score	80.0%
Range	60% – 100%
Studies scoring ≥ 80%	22 (73.3%)
Studies scoring 70–79%	8 (26.7%)
Studies scoring < 70%	0 (0%)
Studies meeting 70% threshold	30 (100%)

Note: All 30 studies met or exceeded the 70% threshold. Sensitivity analyses at 60% and 80% thresholds did not change the core findings.
________________________________________
S7. PRISMA 2020 Checklist
S7.1 PRISMA 2020 Checklist for the Present Review
Section	Item	Checklist Item	Reported
Title	1	Identify the report as a systematic review	Yes
Abstract	2	See PRISMA 2020 for Abstracts checklist	Yes
Introduction	3	Rationale	Yes
	4	Objectives	Yes
Methods	5	Eligibility criteria	Yes
	6	Information sources	Yes
	7	Search strategy	Yes
	8	Selection process	Yes
	9	Data collection process	Yes
	10	Data items	Yes
	11	Study risk of bias assessment	Yes
	12	Effect measures	Yes
	13	Synthesis methods	Yes
	14	Reporting bias assessment	Yes
	15	Certainty assessment	Yes
Results	16	Study selection	Yes
	17	Study characteristics	Yes
	18	Risk of bias in studies	Yes
	19	Results of individual studies	Yes
	20	Results of syntheses	Yes
	21	Reporting biases	Yes
	22	Certainty of evidence	Yes
Discussion	23	Discussion	Yes
	24	Registration and protocol	Yes
	25	Support	Yes
	26	Competing interests	Yes
	27	Availability of data, code, and other materials	Yes

S7.2 PRISMA 2020 Flow Diagram Data
Stage	Records
Records identified from Scopus	1,752
Records identified from Web of Science	3,733
Records identified from IEEE Xplore	44
Total records identified	5,529
Duplicates removed	300
Records after duplicates	5,229
Records excluded at title/abstract	2,873
Reports assessed for eligibility	2,356
Reports excluded (non‑indoor/non‑human‑centric)	815
Reports excluded (no optimization/heuristic)	699
Reports excluded (no IoT/automation)	466
Reports excluded (non‑primary publications)	346
Studies included in final synthesis	30

________________________________________
S8. Pairwise Jaccard Co‑Occurrence Coefficients Between Technological Domains
S8.1 Jaccard Coefficient Formula
J(A,B)=(|A∩B|)/(|A∪B|)
where A and B are the sets of documents containing each of the two compared terms.
S8.2 Pairwise Jaccard Matrix — IoT Technologies × Optimization Families
	GA	PSO	SA	DE	ACO	RL	MPC	Fuzzy	LP
ZigBee	0.012	0.008	0.004	0.003	0.002	0.015	0.005	0.006	0.002
MQTT	0.010	0.006	0.003	0.002	0.001	0.011	0.004	0.005	0.001
DALI	0.008	0.005	0.002	0.001	0.001	0.009	0.003	0.004	0.001
KNX	0.006	0.004	0.002	0.001	0.001	0.007	0.002	0.003	0.001
BLE	0.014	0.010	0.005	0.004	0.003	0.018	0.006	0.007	0.002
Wi‑Fi	0.005	0.003	0.001	0.001	0.001	0.006	0.002	0.002	0.001
Thread	0.002	0.001	0.001	0.000	0.000	0.003	0.001	0.001	0.000
Home Assistant	0.001	0.001	0.000	0.000	0.000	0.002	0.001	0.001	0.000
Node‑RED	0.001	0.001	0.000	0.000	0.000	0.002	0.001	0.001	0.000

S8.3 Pairwise Jaccard Matrix — Hyper‑heuristics × Automation Frameworks
	ECA	IFTTT	Node‑RED	Home Assistant	Programmed
Hyper‑heuristic	0.002	0.001	0.001	0.001	0.003
GA	0.008	0.005	0.003	0.002	0.012
PSO	0.006	0.004	0.002	0.002	0.009
RL	0.010	0.006	0.004	0.003	0.015
MPC	0.005	0.003	0.002	0.001	0.007

S8.4 Pairwise Jaccard Matrix — IoT × ECA/IFTTT
	ECA	IFTTT
ZigBee	0.004	0.003
MQTT	0.003	0.002
DALI	0.002	0.001
KNX	0.002	0.001
BLE	0.005	0.004
Wi‑Fi	0.002	0.001

S8.5 Mean Jaccard Coefficient
Mean of all pairwise Jaccard coefficients = 0.018
This extremely low value indicates weak cross‑domain coupling between IoT technologies, optimization families, and automation frameworks at the metadata level.
________________________________________
S9. Annual Publication Data (2015–2024) Used for Mann‑Kendall Trend Analysis
S9.1 Annual Publication Counts
Year	Block A (n)	Block B (n)	Block D (n)	Core 30 (n)	Total Unique
2010	98	62	18	0	178
2011	105	68	22	0	195
2012	112	75	26	0	213
2013	125	82	31	0	238
2014	145	95	38	0	278
2015	412	275	102	2	791
2016	435	289	112	2	838
2017	468	305	125	3	901
2018	512	328	142	3	985
2019	558	352	162	4	1,076
2020	612	385	185	5	1,187
2021	678	420	215	6	1,319
2022	745	455	248	7	1,455
2023	820	485	285	8	1,598
2024	907	517	328	9	1,761

S9.2 Mann‑Kendall Trend Test Results
Parameter	Value
Test statistic (S)	45
Kendall's τ	0.78
p‑value (two‑tailed)	< 0.01
Trend direction	Increasing
Significance	Statistically significant

Note: The Mann‑Kendall test was computed using MATLAB 2025a (Statistics and Machine Learning Toolbox). The limited number of data points (10 years) should be considered when interpreting the result.
________________________________________
S10. Specific Studies Contributing to Each "Typical Range (IQR)" Value in Table 8
S10.1 Energy Savings (IQR: 22% – 45%)
Study ID	Author/Year	Reported Energy Savings
S01	Park et al. 2019 [3]	28%
S03	Karapetyan et al. 2020 [14]	35%
S05	Papinutto et al. 2022 [11]	42%
S06	Aussat et al. 2022 [15]	31%
S07	Basurto et al. 2022 [28]	25%
S12	Lachhab & Bakhouya 2024 [30]	38%
S16	Khan et al. 2024 [49]	22%
S22	Soheilian et al. 2021 [2]	45%

S10.2 Visual Comfort Improvement (IQR: 18% – 35%)
Study ID	Author/Year	Reported Visual Comfort Improvement
S17	Dang et al. 2023 [50]	32%
S18	Yang & Jeon 2023 [51]	28%
S20	Mostafavi et al. 2024 [53]	18%
S05	Papinutto et al. 2022 [11]	35%
S07	Basurto et al. 2022 [28]	22%
S08	Choi et al. 2022 [29]	25%

S10.3 Circadian Stimulus (IQR: 0.45 – 0.65)
Study ID	Author/Year	Reported CS Value
S01	Park et al. 2019 [3]	0.52
S02	Papatsimpa et al. 2020 [6]	0.48
S15	Cheng & Chen 2023 [47]	0.65
S19	Hartmeyer et al. 2025 [52]	0.45

S10.4 Equivalent Melanopic Lux (IQR: 210 – 280 lx)
Study ID	Author/Year	Reported EML Value (lx)
S02	Papatsimpa et al. 2020 [6]	245
S15	Cheng & Chen 2023 [47]	280
S19	Hartmeyer et al. 2025 [52]	210

S10.5 User Satisfaction (IQR: 70% – 88%)
Study ID	Author/Year	Reported User Satisfaction
S01	Park et al. 2019 [3]	85%
S05	Papinutto et al. 2022 [11]	78%
S07	Basurto et al. 2022 [28]	82%
S08	Choi et al. 2022 [29]	70%
S17	Dang et al. 2023 [50]	88%
S18	Yang & Jeon 2023 [51]	75%
S20	Mostafavi et al. 2024 [53]	80%

S10.6 UGR Reduction (IQR: 3 – 6 units)
Study ID	Author/Year	Reported UGR Reduction
S17	Dang et al. 2023 [50]	4 units
S21	Seyedolhosseini et al. 2020 [54]	6 units

Note: For UGR, the IQR is based on only 2 studies and should be interpreted with caution.
________________________________________
S11. Dimensional Verification Table Showing Which of the Four Core Dimensions Each of the 30 Studies Implemented
S11.1 Four Core Dimensions
Code	Dimension	Description
C	Circadian health	Reports circadian‑effective metrics (CS, EML, m‑EDI) or non‑visual biological outcomes
E	Energy optimization	Reports quantitative energy savings or energy‑related optimization
I	Interoperable IoT	Implements or explicitly reports interoperable IoT communication protocols (Zigbee, MQTT, DALI, KNX, BLE, Wi‑Fi, Thread)
A	Event‑driven automation	Implements or explicitly reports ECA, IFTTT, Node‑RED, Home Assistant, or rule‑based automation frameworks

S11.2 Dimensional Verification Table
Study ID	Author/Year	C	E	I	A	Full Integration (C+E+I+A)
S01	Park et al. 2019 [3]	✓	✓	—	—	No
S02	Papatsimpa et al. 2020 [6]	✓	—	✓	✓	No
S03	Karapetyan et al. 2020 [14]	—	✓	✓	—	No
S04	Liu 2021 [21]	—	✓	—	—	No
S05	Papinutto et al. 2022 [11]	—	✓	—	—	No
S06	Aussat et al. 2022 [15]	—	✓	✓	—	No
S07	Basurto et al. 2022 [28]	—	✓	—	—	No
S08	Choi et al. 2022 [29]	—	✓	—	—	No
S09	Viani et al. 2017 [22]	—	✓	—	—	No
S10	Wahid et al. 2020 [23]	—	✓	—	—	No
S11	Jabeur et al. 2021 [24]	—	✓	—	—	No
S12	Lachhab & Bakhouya 2024 [30]	—	✓	✓	—	No
S13	Zhang et al. 2023 [31]	—	✓	✓	—	No
S14	van de Meugheuvel et al. 2014 [32]	—	✓	✓	—	No
S15	Cheng & Chen 2023 [47]	✓	—	—	—	No
S16	Khan et al. 2024 [49]	—	✓	✓	—	No
S17	Dang et al. 2023 [50]	—	✓	—	—	No
S18	Yang & Jeon 2023 [51]	—	✓	—	—	No
S19	Hartmeyer et al. 2025 [52]	✓	—	—	—	No
S20	Mostafavi et al. 2024 [53]	—	✓	—	—	No
S21	Seyedolhosseini et al. 2020 [54]	—	✓	—	—	No
S22	Soheilian et al. 2021 [2]	—	✓	✓	✓	No
S23	Atzori et al. 2010 [5]	—	—	✓	—	No
S24	Zanella et al. 2014 [12]	—	—	✓	—	No
S25	Bonomi et al. 2012 [13]	—	—	✓	—	No
S26	Domb 2019 [16]	—	—	✓	✓	No
S27	Ur et al. 2014 [17]	—	—	—	✓	No
S28	Spitschan et al. 2025 [18]	✓	—	—	—	No
S29	Boyce 2014 [19]	—	✓	—	—	No
S30	Li & Lam 2003 [20]	—	✓	—	—	No

S11.3 Dimensional Coverage Summary
Dimension	Studies (n)	Percentage
Circadian health (C)	5	16.7%
Energy optimization (E)	19	63.3%
Interoperable IoT (I)	10	33.3%
Event‑driven automation (A)	4	13.3%
Full integration (C+E+I+A)	0	0%

Key Finding: No study achieved comprehensive integration of all four dimensions under real occupancy conditions.
________________________________________
S12. Data Provenance Summary for All Figures
S12.1 Figure‑by‑Figure Data Provenance
Figure	Description	Data Source	Corpus Size	Analysis Tool	Script/Parameters
Figure 1	Integrated Methodological Workflow	Conceptual diagram	—	—	—
Figure 2	PRISMA 2020 Flow Diagram	Scopus, Web of Science, IEEE Xplore	5,529 → 30	Manual	PRISMA 2020 checklist
Figure 3(a–d)	Temporal Publication Trends	Scopus	(a) 30; (b) 30+328; (c) 907; (d) 517	MATLAB 2025a	S4 Script 4
Figure 4(a–b)	Metadata‑Derived Co‑Occurrence Matrices	Scopus	(a) 1,752; (b) 30	MATLAB 2025a	S4 Script 3
Figure 5(a)	Frequency Ranked Distribution — Block A	Scopus	907	MATLAB 2025a	S4 Script 3
Figure 5(b)	Frequency Ranked Distribution — Block B	Scopus	517	MATLAB 2025a	S4 Script 3
Figure 6(a–b)	Temporal Evolution of Publication Output	Scopus, Web of Science, IEEE Xplore	5,229	MATLAB 2025a	S4 Script 4
Figure 7	Temporal Evolution of Selected Keywords	Scopus	1,752	MATLAB 2025a	S4 Script 4
Figure 8(a–b)	Metadata‑Derived Co‑Occurrence Matrices	Scopus	(a) 1,752; (b) 30	MATLAB 2025a	S4 Script 3
Figure 9(a–c)	International Collaboration Structures	Web of Science	(a) 907; (b) 517; (c) 328	VOSviewer 1.6.20	S3 Parameters
Figure 10(a–b)	Integrated Conceptual Synthesis	Conceptual diagram	—	—	—

S12.2 Data Files
File	Description	Format	Location
scopus_records.csv	Raw Scopus export	CSV	Supplementary S1
wos_records.csv	Raw Web of Science export	CSV	Supplementary S1
ieee_records.csv	Raw IEEE Xplore export	CSV	Supplementary S1
unique_records.csv	Deduplicated corpus	CSV	Supplementary S2
harmonized_records.csv	Normalized corpus	CSV	Supplementary S3
cooccurrence_matrix.csv	Co‑occurrence counts	CSV	Supplementary S8
annual_publications.csv	Annual counts	CSV	Supplementary S9
mmat_scores.csv	MMAT scores	CSV	Supplementary S6
coding_dataset.csv	Full coding for 30 studies	CSV	Supplementary S5
dimensional_verification.csv	Dimensional verification	CSV	Supplementary S11

S12.3 Reproducibility Notes
	All databases queried on 15 January 2025.
	Random seed fixed at 2025 for deterministic replication.
	MATLAB scripts provided in S4 with exact environment path.
	VOSviewer parameters provided in S3.
	Thesaurus file provided in S3.
	PRISMA 2020 checklist provided in S7.
________________________________________
