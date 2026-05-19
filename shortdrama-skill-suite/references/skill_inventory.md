# Skill Inventory

Use this inventory as the mandatory first pass for `shortdrama-skill-suite`. Review every row before selecting which source skills to load.

## Input And Long Text

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `file-reference` | `../file-reference` | Parse uploaded or referenced files and extract usable production context. | User mentions files, `@` references, natural-language file references, or asks to use provided materials. | Common |
| `text-splitter` | `../text-splitter` | Split long text into semantic chunks for batch analysis. | Source text is too long for one-pass analysis or needs chunk workflow. | Common |
| `text-truncator` | `../text-truncator` | Truncate general text while preserving coherence. | Need a shorter version under a token/length limit. | Common |
| `novel-truncator` | `../novel-truncator` | Truncate novel text while preserving story continuity. | Novel source exceeds processing limit. | Optional |

## Story Understanding

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `story-summarizer` | `../story-summarizer` | Extract main plot and complete synopsis from story text. | Need quick story understanding or adaptation summary. | Common |
| `story-outliner` | `../story-outliner` | Summarize characters, relationships, and plot into a clean outline. | Need a usable development outline from source text. | Common |
| `novel-summarizer` | `../novel-summarizer` | Produce a 500-800 character novel synopsis for screening. | Source is a novel or novel-like IP. | Common |
| `story-five-elements` | `../story-five-elements` | Analyze genre, synopsis, character profiles, relationships, and major plot points. | Need comprehensive adaptation prep or story bible basics. | Common |
| `story-type-analyzer` | `../story-type-analyzer` | Identify genre, creative elements, and market-facing story features. | Need positioning, genre judgment, or audience framing. | Common |
| `series-analyzer` | `../series-analyzer` | Analyze aired series, pull scenes apart, and learn craft patterns. | User asks to study an existing series or episode. | Optional |

## Characters And Relationships

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `character-profile` | `../character-profile` | Build detailed character biographies and traits from story text. | Need actor reference, role design, or character continuity. | Common |
| `character-relationships` | `../character-relationships` | Analyze relationship types, changes, and plot function. | Need relationship network, emotional conflict, or ensemble logic. | Common |

## Plot And Dramatic Structure

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `plot-keypoints` | `../plot-keypoints` | Extract main story line and stage-based major plot points. | Need quick structural grasp or adaptation beats. | Common |
| `plot-points-analyzer` | `../plot-points-analyzer` | Identify key plot points and turning points. | Need deeper structural validity analysis. | Common |
| `detailed-plot-analyzer` | `../detailed-plot-analyzer` | Expand major plot points into detailed development. | Need to refine an outline or guide writing. | Common |
| `plot-workflow` | `../plot-workflow` | Orchestrate major and detailed plot point generation. | Long story needs modular structural analysis. | Common |
| `drama-analyzer` | `../drama-analyzer` | Extract main plot points and dramatic function. | Need dramatic beats, emotional nodes, or turning points. | Common |
| `drama-workflow` | `../drama-workflow` | Coordinate long-text dramatic function analysis. | Need preprocessing, parallel analysis, and integrated report. | Optional |

## Planning And Creation

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `drama-planner` | `../drama-planner` | Build vertical short-drama planning with emotional value, hooks, and three-act structure. | Need project planning, commercial proposal, or writing guide. | Common |
| `drama-creator` | `../drama-creator` | Create or optimize vertical short-drama scripts, hooks, and outlines. | Need writing, rewriting, concept generation, or precise optimization. | Common |
| `shanyin-screenwriting-master` | `../shanyin-screenwriting-master` | Write full-format screenplays: concept shorts, narrative shorts, feature films, and series with staged workflow and screenwriting methodology. | User asks to write scripts, screenplays, short films, films, series, beat sheets, scene breakdowns, or script-doctor revisions. | Common |
| `knowledge-query` | `../knowledge-query` | Query short-drama knowledge, tropes, high-energy plots, craft, and operations. | Need professional short-drama reference knowledge. | Optional |
| `web-search` | `../web-search` | Search current market information, trends, and cases. | Need latest market, industry, platform, or case data. | Optional |

## Evaluation And Scoring

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `novel-evaluator` | `../novel-evaluator` | Score story text for market potential, innovation, and highlights. | Need novel screening or quality judgment. | Common |
| `story-outline-evaluator` | `../story-outline-evaluator` | Evaluate story outline quality and adaptation potential. | Need outline review or project decision support. | Common |
| `drama-evaluator` | `../drama-evaluator` | Score short-drama adaptation potential and market competitiveness. | Need vertical short-drama viability judgment. | Common |
| `script-evaluator` | `../script-evaluator` | Evaluate scripts from ideological, artistic, and viewing dimensions. | Need script development review or approval advice. | Optional |
| `ip-evaluator` | `../ip-evaluator` | Research and score IP adaptation value. | Need network/IP information and multi-dimensional adaptation score. | Optional |
| `score-analyzer` | `../score-analyzer` | Analyze multi-round scores and calculate S/A/B ratings. | Need score trends, rating aggregation, or comparison. | Optional |

## Video Production

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `shortdrama-production-memory` | `../shortdrama-production-memory` | Apply local video teaching memory, storyboard, first-frame image fusion, Seedance prompts, continuity, camera, lighting, and voice rules. | Any serious Chinese vertical short-drama production, storyboard, fusion image prompt, or video prompt task. | Common |
| `seedance-storyboard` | `../seedance-storyboard` | Convert ideas into Seedance 2.0 professional storyboard prompts. | User asks for Seedance, 即梦, 剪映 AI video, video generation, or storyboard prompts. | Common |
| `.system/imagegen` | `../.system/imagegen` | Generate or edit bitmap images. | User asks to create/edit raster image assets or visual mockups. | Optional |
| `mind-map-generator` | `../mind-map-generator` | Generate visual mind maps for story structure or plot relationships. | Need visual structure map, plot map, or relationship diagram. | Optional |

## Integration And Output

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `result-integrator` | `../result-integrator` | Deduplicate, classify, sort, and synthesize multiple analysis outputs. | Need to combine several analysis passes into one report. | Common |
| `output-formatter` | `../output-formatter` | Format integrated results into structured final outputs. | Need clean final report, structured document, or standardized deliverable. | Common |

## System And Maintenance

| Skill | Path | Use | Trigger | Production Frequency |
| --- | --- | --- | --- | --- |
| `.system/openai-docs` | `../.system/openai-docs` | Use official OpenAI documentation for API/product questions. | User asks how to build with OpenAI products or needs current model/API guidance. | Rare |
| `.system/plugin-creator` | `../.system/plugin-creator` | Create and scaffold Codex plugins. | User asks to create or update a local plugin. | Rare |
| `.system/skill-creator` | `../.system/skill-creator` | Create or update Codex skills. | User asks to create, revise, validate, or package a skill. | Rare |
| `.system/skill-installer` | `../.system/skill-installer` | Install Codex skills from curated or GitHub sources. | User asks to list or install skills. | Rare |
