## Project parent repositories

 * [https://github.com/sucho-oai](https://github.com/sucho-oai)
 * [https://sr.ht/~justinkelly/SUCHO/](https://sr.ht/~justinkelly/SUCHO/)

## About

This is a repository of the full harvest of the OAI-PMH server: http://conference.nau.edu.ua/index.php/Congress/oai using [metha](https://github.com/miku/metha)

The purpose of this project to take harvests of as many Ukrainian OAI-PMH repository servers metadata and source files as possible. Refer [https://github.com/sucho-oai](https://github.com/sucho-oai) for all the repositories harvested. 1 Git repository per OAI repository server.

With the intent that if a Ukrainian repository is taken offline - it can be rebuild using these source files.

This project and repositories align with the [SUCHO.org](https://sucho.org) Saving Ukrainian Cultural Heritage Online project. SUCHO is doing an AMAZING job archiving to the [Internet Archive](https://archive.org) Ukraines curltural hertiage (libraries, galleries, musuems etc..) web site as possible as quickly as possible. It's focus is to crawl and archive Ukraines web pages in WACZ format - so they will be availble in perpetuity. If you are a cultural heritage profesional please consider volunteering.

### Why OAI-PMH

OAI-PMH is a standard which most academic and archival software repositores use for interoperability.

This projects focus is on OAI-PMH, as in the OAI data is the full metadata the repository - be that MARC, DUiblin Core, MARC XML or other.

### Why Metha

Metha saves the oai-pmh data in gzipped xml files. Metha is a fantasic suite of oai tools that include harvesting (incrementaly and full), viewing, querying, and inspecting OAI data. 

For convienciance I have used `metha-cat` to create 1 big xml file per metadataPreifx/format per oai host and uploaded these to BackBlaze B2 (simialr to AWS S3). These files can be too large for git repositories

## Details

OAI Server: 

 * http://conference.nau.edu.ua/index.php/Congress/oai

BackBlaze B2 public bucket:

 * Name: sucho-oai
 * URL:
https://f001.backblazeb2.com/file/sucho-oai/
 * S3 URL: https://sucho-oai.s3.us-west-001.backblazeb2.com/

Cloudflare CDN 

 * https://cdn.biblio.ai/file/sucho-oai/

Formats/metadataPrefixes harvested: oai_dc, oai_marc, marcxml, marc, mods,mets

## Complete OAI feed per format as in indiviual file

* https://cdn.biblio.ai/file/sucho-oai/sucho-conference.nau.edu.ua__index.php__Congress__oai/oai_dc.xml
* https://cdn.biblio.ai/file/sucho-oai/sucho-conference.nau.edu.ua__index.php__Congress__oai/oai_marc.xml
* https://cdn.biblio.ai/file/sucho-oai/sucho-conference.nau.edu.ua__index.php__Congress__oai/marcxml.xml
* https://cdn.biblio.ai/file/sucho-oai/sucho-conference.nau.edu.ua__index.php__Congress__oai/marc.xml
* https://cdn.biblio.ai/file/sucho-oai/sucho-conference.nau.edu.ua__index.php__Congress__oai/mods.xml
* https://cdn.biblio.ai/file/sucho-oai/sucho-conference.nau.edu.ua__index.php__Congress__oai/mets.xml


**Note: If the above xmls files are blank it means that the harvested repository was not publishing in this metadata format. If this repository is blank except for the READMET - it means that the OAI-PMH server has not been fully harvested yet or in unable to be harvested**
