# TRACE Ontology

**Tactics, Roles, Actors, Coercion, and Ecology: A Structured Ontology for Human Trafficking**

TRACE is the first structured, cross-disciplinary ontology for human trafficking tactics, techniques, and procedures, modeled on the [MITRE ATT&CK](https://attack.mitre.org/) framework. It provides a shared knowledge architecture for law enforcement, clinical practice, intelligence analysis, social work, and victim advocacy.

## Overview

| Component | Count | Description |
|---|---|---|
| Tactics | 6 | Trafficking lifecycle phases (Targeting through Scaling) |
| Techniques | 48 | Specific methods mapped to tactics |
| Sub-techniques | 141 | Implementation-level detail |
| Threat Actor Profiles | 10 | Typified trafficking operator categories |
| Coercion Methods | 8 | Biderman framework unified with Hassan BITE model |
| Typologies | 30 | Polaris Project types plus additional forms |
| Radicalization Pathways | 9 | Victim trajectory models |
| Classification Crosswalks | ICD-10, DSM-5, NIBRS, Immigration | Integration with existing systems |

## Tactic-Phase Mapping

| Tactic | Phase | Objective |
|---|---|---|
| **Targeting** | Pre-trafficking | Identify and profile vulnerable individuals |
| **Recruitment** | Transition | Establish initial trafficking relationship |
| **Coercion** | Early/Sustained | Maintain forced compliance through psychological, economic, and physical means |
| **Exploitation** | Sustained | Extract labor, control economic output, maintain harm |
| **Concealment** | Throughout | Avoid detection and evade accountability |
| **Scaling** | Expansion | Increase victim volume and geographic reach |

## Repository Structure

```
TRACE-Ontology/
  data/
    trace_ontology_v1.1.yaml    # Machine-readable structured ontology
  docs/
    TRACE_Ontology_Framework_v1.md  # Comprehensive reference document
  LICENSE                        # CC BY 4.0
  README.md
```

## Data Format

The ontology is distributed as a YAML file with the following top-level keys:

- `meta` - Version, authorship, and description
- `tactics` - Six lifecycle phases with descriptions and role relevance
- `techniques` - 48 techniques, each with sub-techniques, role-specific indicators for five professional roles, mitigations, and source framework mappings
- `threat_actors` - 10 profiles with characteristic technique usage
- `coercion_methods` - Biderman x BITE unification with trafficking manifestations
- `typologies` - 30 trafficking forms organized by category
- `radicalization_pathways` - 9 victim trajectory models
- `crosswalks` - Mappings to ICD-10, DSM-5, NIBRS, and immigration classifications

## Role-Specific Indicator Architecture

Every technique includes indicators observable by five professional roles:

- **Law Enforcement** - Evidence, testimony, and investigative indicators
- **Clinical/SANE** - Trauma presentations, health consequences, screening cues
- **Intelligence** - Network patterns, operational signatures, threat analysis
- **Social Work** - Service access barriers, client presentations, system indicators
- **Victim Advocacy** - Recovery needs, rights-based considerations, empowerment indicators

## Source Frameworks

TRACE synthesizes nine evidence-based frameworks:

1. Polaris Project Typology of Modern Slavery
2. ILO Indicators of Forced Labour (2012, 2025 revision)
3. Zimmerman Social-Ecological Model
4. Biderman's Framework of Coercive Control
5. Hassan's BITE Model of Authoritarian Control
6. Crime Scripting Theory (Cornish; Brayley, Cockbain & Laycock)
7. Routine Activity Theory (Cohen & Felson)
8. Social Network Analysis applied to trafficking
9. Victim-centered trauma frameworks

## Citation

If you use TRACE in your research, please cite:

> Hurst, D. A. (2026). TRACE: A structured ontology for human trafficking tactics, techniques, and procedures modeled on the MITRE ATT&CK framework. *Journal of Human Trafficking*. DOI https://zenodo.org/badge/DOI/10.5281/zenodo.19458175.svg

## License

This work is licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). You are free to share and adapt the material with appropriate attribution.

## Contact

David A. Hurst
School of Security and Global Studies, American Military University
ORCID: [0009-0008-3009-4438](https://orcid.org/0009-0008-3009-4438)
