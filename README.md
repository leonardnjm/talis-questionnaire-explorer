# TALIS Questionnaire Explorer

A remote MCP connector for searching, reading and comparing the questionnaires of TALIS, the Teaching and Learning International Survey. It works with Claude, ChatGPT and any client that supports remote MCP servers.

It answers from the published teacher and principal questionnaires (2008, 2013, 2018 and 2024): exact question wording, items, response scales, routing, defined terms and dataset variable names, traced across survey cycles.

**What it does not do:** it holds no survey responses or results. It can tell you what was asked, of whom and how, but not what respondents answered (no percentages, averages or country results).

## Connect

**Claude:** open the Connectors Directory, search for *TALIS Questionnaire Explorer* and click **Connect**. No account or sign-in is needed.

**Any other MCP client:** add a remote MCP server with this URL (Streamable HTTP, no authentication):

```
https://az-talis-mcp-ca-prod-vnrk.thankfulwater-7598f59e.francecentral.azurecontainerapps.io/mcp
```

## Examples

- *Which TALIS 2024 teacher questions cover professional development?*
- *Compare the job satisfaction items between TALIS 2018 and 2024. Which were kept, added or dropped?*
- *Show the exact wording and response scale of the principal questionnaire item on school leadership.*
- *What changed in the teacher questionnaire between 2018 and 2024?*
- *Which dataset variable holds teachers' years of experience in each cycle?*

## Tools

All tools are read-only.

| Area | Tools |
|---|---|
| Find questions | `talis_search_questions`, `talis_search_items`, `talis_list_topic`, `talis_get_question` |
| Browse the questionnaires | `talis_list_instruments`, `talis_list_structure`, `talis_list_domains`, `talis_list_definitions`, `talis_list_variables`, `talis_list_scales`, `talis_get_scale`, `talis_trace_routing` |
| Follow a concept over time | `talis_get_concept`, `talis_concept_coverage`, `talis_compare_items`, `talis_compare_questions` |
| Compare instruments | `talis_compare_instruments`, `talis_find_parallel_questions`, `talis_find_cross_instrument_parallels` |

## Limitations

- Questionnaire content only: no survey responses, results or microdata.
- National adaptations of the questionnaires are not included unless stated in the results.

## Privacy

See the [privacy policy](PRIVACY.md).

## Support

Email [EDUTALIS@oecd.org](mailto:EDUTALIS@oecd.org) or [leonard.najman@oecd.org](mailto:leonard.najman@oecd.org), or open an issue in this repository.
