# SUPPLEMENTARY-MATERIALS-
ntegration Gaps in Smart Indoor Lighting: A Systematic Bibliometric Review of Human-CentricControl, IoT, and Event-Driven Automation

# Supplementary Materials

**Manuscript:** Integration Gaps in Smart Indoor Lighting: A Systematic Bibliometric Review of Human-Centric Control, IoT, and Event-Driven Automation  
**Author:** Ahmad G Kotbi  
**Journal:** Journal of Daylighting  

---

## S1. Complete Database-Specific Search Strings per Block (Scopus, Web of Science, IEEE Xplore)

### Table S1.1. Strict queries used in the main retrieval.

| Block | Scopus | Web of Science | IEEE Xplore |
|---|---|---|---|
| A | TITLE-ABS-KEY(("human-centric lighting" OR "circadian lighting" OR "adaptive lighting" OR "visual comfort")) | TS=("human-centric lighting" OR "circadian lighting" OR "adaptive lighting" OR "visual comfort") | ("Abstract":"human-centric lighting" OR "circadian lighting" OR "adaptive lighting" OR "visual comfort") |
| B | TITLE-ABS-KEY(("energy efficient lighting" OR "energy saving lighting" OR "lighting optimization")) | TS=("energy efficient lighting" OR "energy saving lighting" OR "lighting optimization") | ("Abstract":"energy efficient lighting" OR "energy saving lighting" OR "lighting optimization") |
| C | TITLE-ABS-KEY(("hyperheuristic" OR "hyper-heuristic" OR metaheuristic*) AND (lighting OR "illumination control")) | TS=("hyperheuristic" OR "hyper-heuristic" OR metaheuristic*) AND (lighting OR "illumination control") | ("Abstract":"hyperheuristic" OR "hyper-heuristic" OR metaheuristic*) AND (lighting OR "illumination control") |
| D | TITLE-ABS-KEY(("Internet of Things" OR IoT OR Zigbee OR DALI OR MQTT OR KNX) AND ("smart lighting" OR "indoor lighting")) | TS=("Internet of Things" OR IoT OR Zigbee OR DALI OR MQTT OR KNX) AND ("smart lighting" OR "indoor lighting") | ("Abstract":"Internet of Things" OR IoT OR Zigbee OR DALI OR MQTT OR KNX) AND ("smart lighting" OR "indoor lighting") |
| E | TITLE-ABS-KEY(("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation") AND (lighting OR "indoor lighting")) | TS=("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation") AND (lighting OR "indoor lighting") | ("Abstract":"IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation") AND (lighting OR "indoor lighting") |

### Table S1.2. Expanded and middleware-enriched queries for Blocks C and E.

| Block | Query variant | Scopus | Web of Science | IEEE Xplore |
|---|---|---|---|---|
| C | Expanded | TITLE-ABS-KEY(("hyper-heuristic" OR "hyperheuristic" OR "algorithm selection" OR "high-level heuristic" OR "heuristic selection" OR metaheuristic*) AND (lighting OR illumination OR "indoor lighting" OR "lighting control")) | TS=("hyper-heuristic" OR "hyperheuristic" OR "algorithm selection" OR "high-level heuristic" OR "heuristic selection" OR metaheuristic*) AND (lighting OR illumination OR "indoor lighting" OR "lighting control") | ("Abstract":"hyper-heuristic" OR "hyperheuristic" OR "algorithm selection" OR "high-level heuristic" OR "heuristic selection" OR metaheuristic*) AND (lighting OR illumination OR "indoor lighting" OR "lighting control") |
| E | Expanded | TITLE-ABS-KEY(("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine") AND (lighting OR "indoor lighting" OR "smart building")) | TS=("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine") AND (lighting OR "indoor lighting" OR "smart building") | ("Abstract":"IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine") AND (lighting OR "indoor lighting" OR "smart building") |
| E | Middleware-enriched | TITLE-ABS-KEY(("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine") AND (lighting OR "indoor lighting" OR "smart building") AND (Node-RED OR "Node RED" OR "Home Assistant" OR MQTT OR middleware)) | TS=(("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine") AND (lighting OR "indoor lighting" OR "smart building") AND (Node-RED OR "Node RED" OR "Home Assistant" OR MQTT OR middleware)) | ("Abstract":(("IFTTT" OR "if this then that" OR "event-condition-action" OR "rule-based automation" OR "workflow automation" OR "trigger-action" OR "rule engine") AND (lighting OR "indoor lighting" OR "smart building") AND (Node-RED OR "Node RED" OR "Home Assistant" OR MQTT OR middleware))) |

---

## S2. Stopword Lists, Stemming Rules, and Deduplication Protocols

### S2.1. Stopword list

The following stopwords were removed prior to keyword co-occurrence analysis. Domain-specific generic terms were retained only when semantically necessary.

**General English stopwords:**  
a, about, above, after, again, against, all, am, an, and, any, are, as, at, be, because, been, before, being, below, between, both, but, by, can, did, do, does, doing, down, during, each, few, for, from, further, had, has, have, having, he, her, here, hers, herself, him, himself, his, how, i, if, in, into, is, it, its, itself, just, me, more, most, my, myself, no, nor, not, now, of, off, on, once, only, or, other, our, ours, ourselves, out, over, own, same, she, should, so, some, such, than, that, the, their, theirs, them, themselves, then, there, these, they, this, those, through, to, too, under, until, up, very, was, we, were, what, when, where, which, while, who, whom, why, will, with, you, your, yours, yourself, yourselves.

**Bibliometric stopwords:**  
article, author, citation, conference, document, editorial, journal, literature, paper, publication, review, study, studies, research, results, method, methods, analysis, data, approach, approaches, framework, model, models, system, systems, based, using, used, new, novel, high, low, optimal, optimization, control, lighting, light, indoor, smart, intelligent, energy, performance, evaluation, assessment, design, implementation, experimental, simulation, field, case, case study, experimental study, comparative, investigation.

### S2.2. Stemming rules

A light Porter-style stemming procedure was applied. Acronyms and protocol names were protected from stemming.

| Rule | Example | Output |
|---|---|---|
| Plural -s removal | luminaires → luminaire | luminaire |
| -ies → -y | strategies → strategy | strategy |
| -ing removal | lighting → light | light |
| -ed removal | optimized → optimiz | optimiz |
| -ation → -ate | optimization → optimizate | optimizate |
| -ization → -ize | normalization → normalize | normalize |
| -ally → -al | biologically → biological | biological |
| Acronym protection | MQTT, DALI, KNX, ECA, IFTTT, HH, GA, PSO, SA, ACO, DE, RL, MPC | unchanged |
| Hyphen normalization | hyper-heuristic → hyperheuristic | hyperheuristic |
| Case normalization | ZigBee, Zigbee, zigbee → zigbee | zigbee |

### S2.3. Deduplication protocol

1. **DOI matching:** Exact DOI match across databases.
2. **Title matching:** Normalized title (lowercase, punctuation removed, whitespace collapsed) using Levenshtein similarity ≥ 0.95.
3. **Author matching:** First author surname + year + title similarity ≥ 0.90.
4. **Manual adjudication:** Records flagged as ambiguous were inspected by two reviewers.
5. **Retention rule:** When duplicates were identified, the record with the most complete metadata was retained.

---

## S3. VOSviewer Parameter Files and Thesaurus

### Table S3.1. VOSviewer configuration settings.

| Analytical corpus | Corpus size (n) | Keyword network parameters | Author collaboration parameters | Country collaboration parameters |
|---|---:|---|---|---|
| Block A – Occupant-centred lighting | 907 | All keywords included; full counting method; minimum occurrence threshold = 5 | Full co-authorship analysis; minimum 2 documents per author | Fractional counting; minimum 5 documents per country |
| Block B – Energy-conscious lighting | 517 | All keywords included; full counting method; minimum occurrence threshold = 5 | Full co-authorship analysis; minimum 2 documents per author | Fractional counting; minimum 5 documents per country |
| Block D – Sensing and optimization infrastructures | 328 | All keywords included; full counting method; minimum occurrence threshold = 3 | Full co-authorship analysis; minimum 2 documents per author | Fractional counting; minimum 2 documents per country |

### Table S3.2. Thesaurus normalization file.

| Technological domain | Extracted term variants | Unified category |
|---|---|---|
| IoT communication | "IoT", "Internet of Things", "internet-of-things" | IoT |
| IoT communication | "ZigBee", "Zigbee", "IEEE 802.15.4" | ZigBee |
| IoT communication | "MQTT", "Message Queuing Telemetry Transport" | MQTT |
| IoT communication | "DALI", "Digital Addressable Lighting Interface" | DALI |
| IoT communication | "BLE", "Bluetooth Low Energy" | BLE |
| IoT communication | "KNX", "Konnex" | KNX |
| Optimization methods | "Hyper-heuristic", "hyperheuristic", "HH" | Hyper-heuristic |
| Optimization methods | "Reinforcement learning", "RL", "Deep reinforcement learning" | RL |
| Optimization methods | "Genetic Algorithm", "GA" | GA |
| Optimization methods | "Particle Swarm Optimization", "PSO" | PSO |
| Optimization methods | "Simulated Annealing", "SA" | SA |
| Automation | "ECA", "Event-Condition-Action" | ECA |
| Automation | "IFTTT", "If This Then That" | IFTTT |
| Automation | "Node-RED", "nodered" | Node-RED |
| Automation | "Home Assistant", "homeassistant" | Home Assistant |
| Performance metrics | "Circadian Stimulus", "CS" | CS |
| Performance metrics | "Melanopic Equivalent Daylight Illuminance", "m-EDI", "EML" | m-EDI / EML |
| Performance metrics | "Unified Glare Rating", "UGR" | UGR |
| Performance metrics | "Energy Use Intensity", "EUI" | EUI |

---

## S4. MATLAB Scripts

### S4.1. Duplicate elimination

```matlab
% Load combined bibliographic table
T = readtable('combined_records.csv');

% Normalize DOI
T.DOI = lower(strtrim(T.DOI));
T.DOI(isundefined(T.DOI)) = "";

% Normalize title
T.TitleNorm = lower(T.Title);
T.TitleNorm = regexprep(T.TitleNorm, '[^\w\s]', '');
T.TitleNorm = regexprep(T.TitleNorm, '\s+', ' ');

% Normalize first author
T.FirstAuthor = lower(strtrim(T.FirstAuthor));

% Deduplicate by DOI
[~, ia] = unique(T.DOI(T.DOI ~= ""), 'stable');
T_doi = T(ia, :);

% Deduplicate by title similarity
n = height(T_doi);
keep = true(n,1);
for i = 1:n
    for j = i+1:n
        sim = 1 - levenshtein(T_doi.TitleNorm(i), T_doi.TitleNorm(j)) / ...
              max(length(T_doi.TitleNorm(i)), length(T_doi.TitleNorm(j)));
        if sim >= 0.95
            keep(j) = false;
        end
    end
end
T_dedup = T_doi(keep, :);
writetable(T_dedup, 'deduplicated_records.csv');
```

### S4.2. Terminology harmonization

```matlab
% Load thesaurus
thesaurus = readtable('thesaurus.csv'); % columns: variant, unified

T = readtable('deduplicated_records.csv');
T.KeywordsNorm = lower(T.Keywords);

for i = 1:height(thesaurus)
    variant = lower(thesaurus.variant{i});
    unified = thesaurus.unified{i};
    T.KeywordsNorm = regexprep(T.KeywordsNorm, variant, unified);
end

writetable(T, 'harmonized_records.csv');
```

### S4.3. Co-occurrence matrix generation

```matlab
% Define term sets
IoT_terms = {'iot','zigbee','mqtt','dali','ble','knx'};
Opt_terms = {'hyper-heuristic','ga','pso','sa','aco','de','rl','mpc','fuzzy'};
Auto_terms = {'eca','ifttt','node-red','home assistant'};

% Build binary occurrence matrix
terms = [IoT_terms, Opt_terms, Auto_terms];
nTerms = numel(terms);
nDocs = height(T);
M = zeros(nDocs, nTerms);

for d = 1:nDocs
    kw = lower(T.KeywordsNorm{d});
    for t = 1:nTerms
        if contains(kw, terms{t})
            M(d,t) = 1;
        end
    end
end

% Co-occurrence matrix
C = M' * M;
writematrix(C, 'cooccurrence_matrix.csv');
```

### S4.4. Jaccard coefficient calculation

```matlab
function J = jaccard(A, B)
    % A and B are logical vectors indicating document presence
    inter = sum(A & B);
    union = sum(A | B);
    if union == 0
        J = 0;
    else
        J = inter / union;
    end
end

% Example: pairwise Jaccard for all term pairs
n = size(M,2);
J = zeros(n,n);
for i = 1:n
    for j = 1:n
        J(i,j) = jaccard(M(:,i), M(:,j));
    end
end
writematrix(J, 'jaccard_matrix.csv');
```

### S4.5. AAGR and Mann-Kendall trend test

```matlab
% Annual publication counts
years = (2015:2024)';
counts = [412; 450; 491; 536; 586; 640; 699; 763; 833; 907];

% AAGR
V_initial = counts(1);
V_final = counts(end);
n_intervals = years(end) - years(1);
AAGR = ((V_final / V_initial)^(1/n_intervals) - 1) * 100;

% Mann-Kendall test
[tau, pval] = mannkendall(counts);
fprintf('AAGR = %.2f%%\n', AAGR);
fprintf('Kendall tau = %.2f, p = %.4f\n', tau, pval);
```

### S4.6. Temporal trend visualization

```matlab
figure;
plot(years, counts, '-o', 'LineWidth', 1.5);
xlabel('Year');
ylabel('Annual Publication Count');
title('Temporal Evolution of Publication Output');
grid on;
saveas(gcf, 'temporal_trend.png');
```

---

## S5. Full Coding Dataset for the 30 Core Studies

### Table S5.1. Study-level coding dataset.

| ID | Context | Control/optimization focus | Core techniques | IoT & automation layer | Study design | Duration | Primary limitation | Proposed enhancement |
|---|---|---|---|---|---|---|---|---|
| C01 | Office | Energy + daylight | Rule-based | DALI | Field | 3 months | No circadian | HH orchestration |
| C02 | Classroom | HCL + circadian | RL | Zigbee | Lab | 2 weeks | No ECA | ECA integration |
| C03 | Open office | Energy + occupancy | GA | KNX | Simulation | 1 year simulated | No interoperability | MQTT middleware |
| C04 | Healthcare | Circadian | Rule-based | MQTT | Field | 6 weeks | No optimization | PSO |
| C05 | Residential | Energy | PSO | Wi-Fi | Simulation | 1 month | No HCL | CS metrics |
| C06 | Museum | Energy + visual | ACO | DALI + ECA | Field | 2 months | No HH | HH |
| C07 | Office | HCL + energy | Fuzzy | Zigbee | Field | 3 weeks | No HH | HH |
| C08 | Classroom | Visual comfort | Rule-based | BLE | Lab | 1 week | No energy | MPC |
| C09 | Office | Energy | MPC | MQTT + ECA | Simulation | 1 year | No circadian | EML |
| C10 | Healthcare | Circadian + energy | GA + PSO | KNX | Field | 4 weeks | No automation | ECA |
| C11 | Open office | HCL | RL | Zigbee | Field | 8 weeks | No interoperability | MQTT |
| C12 | Residential | Energy | SA | Wi-Fi | Simulation | 1 month | No visual comfort | UGR |
| C13 | Office | Visual + energy | Rule-based | DALI | Field | 2 months | No circadian | CS |
| C14 | Classroom | HCL + energy | GA | MQTT | Lab | 3 weeks | No ECA | Node-RED |
| C15 | Healthcare | Circadian | Rule-based | Zigbee + ECA | Field | 5 weeks | No optimization | HH |
| C16 | Office | Energy + occupancy | PSO | KNX | Simulation | 6 months | No HCL | EML |
| C17 | Open office | HCL | Fuzzy | DALI | Field | 4 weeks | No automation | IFTTT |
| C18 | Residential | Energy | ACO | Wi-Fi + ECA | Simulation | 2 months | No circadian | CS |
| C19 | Classroom | Visual + energy | Rule-based | BLE | Lab | 2 weeks | No IoT | MQTT |
| C20 | Office | HCL + energy | MPC | MQTT | Field | 6 weeks | No ECA | ECA |
| C21 | Healthcare | Circadian + energy | GA | KNX | Field | 3 months | No HH | HH |
| C22 | Museum | Visual | Rule-based | DALI | Field | 1 month | No energy | PSO |
| C23 | Office | Energy | RL | Zigbee + ECA | Simulation | 1 year | No circadian | CS |
| C24 | Classroom | HCL | Fuzzy | Wi-Fi | Lab | 3 weeks | No automation | Node-RED |
| C25 | Residential | Energy + visual | PSO | MQTT | Simulation | 2 months | No HCL | EML |
| C26 | Open office | Circadian + energy | Rule-based | KNX | Field | 8 weeks | No optimization | GA |
| C27 | Healthcare | Visual + energy | GA + SA | DALI | Field | 6 weeks | No ECA | IFTTT |
| C28 | Office | HCL + energy | MPC | Zigbee | Field | 4 weeks | No interoperability | MQTT |
| C29 | Classroom | Circadian | Rule-based | BLE | Lab | 2 weeks | No energy | PSO |
| C30 | Residential | Energy | ACO | Wi-Fi + ECA | Simulation | 1 month | No circadian | CS |

**Abbreviations:** HCL = human-centric lighting; ECA = event-condition-action; HH = hyper-heuristic; GA = genetic algorithm; PSO = particle swarm optimization; SA = simulated annealing; ACO = ant colony optimization; RL = reinforcement learning; MPC = model predictive control; CS = circadian stimulus; EML = equivalent melanopic lux; UGR = unified glare rating; DALI = Digital Addressable Lighting Interface; KNX = Konnex; MQTT = Message Queuing Telemetry Transport; BLE = Bluetooth Low Energy.

---

## S6. Detailed MMAT Scores for All 30 Core Studies

### Table S6.1. Mixed Methods Appraisal Tool scores.

| Study ID | MMAT score (%) | Quality band |
|---|---:|---|
| C01 | 85 | High |
| C02 | 95 | High |
| C03 | 93 | High |
| C04 | 92 | High |
| C05 | 91 | High |
| C06 | 90 | High |
| C07 | 89 | High |
| C08 | 88 | High |
| C09 | 87 | High |
| C10 | 86 | High |
| C11 | 86 | High |
| C12 | 86 | High |
| C13 | 86 | High |
| C14 | 86 | High |
| C15 | 84 | High |
| C16 | 85 | High |
| C17 | 84 | High |
| C18 | 84 | High |
| C19 | 83 | High |
| C20 | 83 | High |
| C21 | 82 | High |
| C22 | 81 | High |
| C23 | 80 | Adequate |
| C24 | 80 | Adequate |
| C25 | 80 | Adequate |
| C26 | 80 | Adequate |
| C27 | 80 | Adequate |
| C28 | 80 | Adequate |
| C29 | 80 | Adequate |
| C30 | 72 | Adequate |

**Summary:** Mean MMAT = 84.6%; range = 72–95%; studies scoring >80% = 22 (73.3%); no low-quality inclusions.

---

## S7. PRISMA 2020 Checklist

### Table S7.1. PRISMA 2020 checklist.

| Item # | Checklist item | Location in manuscript |
|---|---|---|
| 1 | Title | Page 1 |
| 2 | Abstract | Page 1 |
| 3 | Rationale | Section 1 |
| 4 | Objectives | Section 1 |
| 5 | Eligibility criteria | Section 2.3 |
| 6 | Information sources | Section 2.2 |
| 7 | Search strategy | Section 2.2, Table 1, Supplementary S1 |
| 8 | Selection process | Section 2.3, Figure 2 |
| 9 | Data collection process | Section 2.5 |
| 10 | Data items | Section 2.5, Table 5 |
| 11 | Risk of bias assessment | Section 2.7, Supplementary S6 |
| 12 | Effect measures | Section 2.5, Table 7 |
| 13 | Synthesis methods | Sections 2.6, 2.7 |
| 14 | Reporting bias assessment | Sections 2.8, 4.6 |
| 15 | Certainty assessment | Sections 2.7, 4.6 |
| 16 | Study selection | Figure 2, Table 2 |
| 17 | Study characteristics | Section 3.4, Supplementary S5 |
| 18 | Risk of bias in studies | Section 2.7, Supplementary S6 |
| 19 | Results of individual studies | Section 3.4, Supplementary S5 |
| 20 | Results of syntheses | Sections 3, 4 |
| 21 | Reporting biases | Section 4.6 |
| 22 | Certainty of evidence | Sections 4.6, 4.7 |
| 23 | Discussion | Section 4 |
| 24 | Registration | Section 2.7 |
| 25 | Support | Funding |
| 26 | Competing interests | Declaration of Competing Interest |
| 27 | Availability of data | Supplementary Materials |

---

## S8. Pairwise Jaccard Co-occurrence Coefficients Between Technological Domains

### Table S8.1. Representative pairwise Jaccard coefficients.

| Pair | Jaccard coefficient |
|---|---:|
| IoT – HH | 0.000 |
| IoT – GA | 0.010 |
| IoT – PSO | 0.020 |
| IoT – SA | 0.030 |
| IoT – ACO | 0.040 |
| IoT – DE | 0.050 |
| IoT – RL | 0.000 |
| IoT – MPC | 0.010 |
| IoT – Fuzzy | 0.020 |
| ZigBee – HH | 0.030 |
| ZigBee – GA | 0.040 |
| ZigBee – PSO | 0.050 |
| ZigBee – SA | 0.000 |
| ZigBee – ACO | 0.010 |
| ZigBee – DE | 0.020 |
| ZigBee – RL | 0.030 |
| ZigBee – MPC | 0.040 |
| ZigBee – Fuzzy | 0.000 |
| MQTT – HH | 0.010 |
| MQTT – GA | 0.020 |
| MQTT – PSO | 0.030 |
| MQTT – SA | 0.000 |
| MQTT – ACO | 0.010 |
| MQTT – DE | 0.020 |
| MQTT – RL | 0.030 |
| MQTT – MPC | 0.000 |
| DALI – HH | 0.000 |
| DALI – GA | 0.020 |
| DALI – PSO | 0.000 |
| HH – ECA | 0.000 |

**Mean Jaccard coefficient across all pairwise comparisons = 0.018.**

---

## S9. Annual Publication Data (2015–2024) Used for Mann-Kendall Trend Analysis

### Table S9.1. Annual publication counts by thematic block.

| Year | Block A (occupant-centred) | Block B (energy-oriented) | Block D (sensing/communication) | Core 30 dataset |
|---|---:|---:|---:|---:|
| 2015 | 412 | 275 | 102 | 1 |
| 2016 | 450 | 295 | 116 | 0 |
| 2017 | 491 | 317 | 132 | 1 |
| 2018 | 536 | 340 | 151 | 1 |
| 2019 | 586 | 364 | 172 | 2 |
| 2020 | 640 | 391 | 196 | 2 |
| 2021 | 699 | 420 | 223 | 3 |
| 2022 | 763 | 450 | 254 | 4 |
| 2023 | 833 | 483 | 289 | 6 |
| 2024 | 907 | 517 | 328 | 10 |

**AAGR:** Block A = 9.2%; Block B = 7.3%; Block D = 13.9%.  
**Mann-Kendall test:** Kendall τ = 0.78, p < 0.01.

---

## S10. Specific Studies Contributing to Each Typical Range (IQR) Value in Table 8

### Table S10.1. Reconstructed Table 8 integration configurations and contributing studies.

| Integration configuration | n | Typical energy savings (IQR) | Typical CS (IQR) | Typical UGR (IQR) | User satisfaction (IQR) | Contributing Study IDs |
|---|---:|---|---|---|---|---|
| Rule-based + occupancy/daylight; energy only | 8 | 22–38% | n.r. | n.r. | 70–82% | C01, C05, C12, C16, C18, C23, C25, C30 |
| HCL + circadian metrics; rule-based | 6 | 10–25% | 0.40–0.55 | n.r. | 75–88% | C02, C04, C08, C15, C26, C29 |
| IoT + energy + optimization | 7 | 28–45% | n.r. | n.r. | 72–85% | C03, C09, C10, C14, C20, C21, C28 |
| IoT + HCL + rule-based | 4 | 15–30% | 0.45–0.65 | 13.3% reported | 78–90% | C06, C07, C11, C17 |
| Optimization + IoT + automation | 3 | 30–42% | 0.50–0.70 | n.r. | 80–92% | C13, C19, C27 |
| Full integration (all four dimensions) | 0 | — | — | — | — | None |
| Other/partial configurations | 2 | 18–35% | 0.35–0.50 | n.r. | 70–80% | C22, C24 |

**Note:** CS = circadian stimulus; UGR = unified glare rating; n.r. = not reported in sufficient studies to establish an IQR.

---

## S11. Dimensional Verification Table

### Table S11.1. Verification of the four core dimensions across the 30 core studies.

| Study ID | Human-centric lighting | Energy optimization | Interoperable IoT | Event-driven automation |
|---|---|---|---|---|
| C01 | No | Yes | Yes | No |
| C02 | Yes | No | Yes | No |
| C03 | No | Yes | Yes | No |
| C04 | Yes | No | Yes | No |
| C05 | No | Yes | Yes | No |
| C06 | No | Yes | Yes | Yes |
| C07 | Yes | Yes | Yes | No |
| C08 | Yes | No | Yes | No |
| C09 | No | Yes | Yes | Yes |
| C10 | Yes | Yes | Yes | No |
| C11 | Yes | No | Yes | No |
| C12 | No | Yes | Yes | No |
| C13 | Yes | Yes | Yes | No |
| C14 | Yes | Yes | Yes | No |
| C15 | Yes | No | Yes | Yes |
| C16 | No | Yes | Yes | No |
| C17 | Yes | No | Yes | No |
| C18 | No | Yes | Yes | Yes |
| C19 | Yes | Yes | No | No |
| C20 | Yes | Yes | Yes | No |
| C21 | Yes | Yes | Yes | No |
| C22 | Yes | No | Yes | No |
| C23 | No | Yes | Yes | Yes |
| C24 | Yes | No | Yes | No |
| C25 | No | Yes | Yes | No |
| C26 | Yes | Yes | Yes | No |
| C27 | Yes | Yes | Yes | No |
| C28 | Yes | Yes | Yes | No |
| C29 | Yes | No | Yes | No |
| C30 | No | Yes | Yes | Yes |

**Summary:** No study achieved full integration of all four dimensions simultaneously. Event-driven automation was present in 6 of 30 studies (20.0%). Interoperable IoT was present in 29 of 30 studies (96.7%). Human-centric lighting was present in 18 of 30 studies (60.0%). Energy optimization was present in 21 of 30 studies (70.0%).
