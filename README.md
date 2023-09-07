![alt text](https://github.com/CHC-Computations/Harmonize/blob/main/logo-1.png?raw=true)
## Enrich: LOD-based Data Mapper

### Overview

Enrich is a Python-based tool developed using the [Django](https://www.djangoproject.com/) framework. Its primary goal is to enhance any given set of keywords with rich metadata, leveraging Linked Open Data (LOD) technologies. The tool pulls information from [Wikidata](https://www.wikidata.org/) and employs string similarity mechanisms like `difflib`, `SequenceMatcher`, and `Levenshtein` to match these keywords with records from the National Library of Poland via its API at [data.bn.org.ok](http://data.bn.org.ok/).

### Workflow

1. **Keyword Input**: Users start by inputting a keyword or a set of keywords that they wish to enrich.

2. **Data Enrichment**: 
    - **[Wikidata](https://www.wikidata.org/)**: Information related to the provided keywords is fetched from Wikidata, adding context and relevant metadata.
    
3. **String Similarity Mechanisms**: 
    - Utilizing Python's built-in [difflib](https://docs.python.org/3/library/difflib.html) library and additional sequence matching libraries such as `Levenshtein`, Enrich identifies words that closely resemble the user-provided keywords.
    
4. **National Library of Poland API**: 
    - Enrich connects to the National Library of Poland through its API available at [data.bn.org.pl](http://data.bn.org.pl/). It links the similar keywords to subject terms from the library.
  
### Technologies Used
- [Django](https://www.djangoproject.com/)
- [Wikidata](https://www.wikidata.org/)
- [difflib](https://docs.python.org/3/library/difflib.html)
- [Levenshtein](https://pypi.org/project/python-Levenshtein/)
- [National Library of Poland API](http://data.bn.org.pl/)

Enrich offers a comprehensive data mapping solution, capable of providing contextual information to any keyword and enhancing it with reputable bibliographic data from Poland's National Library.


![alt_text](https://github.com/CHC-Computations/Harmonize/blob/main/Zrzut%20ekranu%202022-12-19%20o%2017.48.49.png?raw=true)
