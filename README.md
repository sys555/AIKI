# AIKI

[![codecov](https://codecov.io/gh/OpenKILab/AIKI/branch/main/graph/badge.svg?token=AIKI_token_here)](https://codecov.io/gh/OpenKILab/AIKI)
[![CI](https://github.com/OpenKILab/AIKI/actions/workflows/main.yml/badge.svg)](https://github.com/OpenKILab/AIKI/actions/workflows/main.yml)

Knowledge Infrastructure for AI.

## Install it from PyPI

```bash
pip install aiki
```

## Usage

```py
from aiki import KnowledgeBase

kb = KnowledgeBase(name = "Environment")

# 1. add
# 2. update
# 3. query
# 4. config

# 1. add
result = kb.add(path = "/file_path")
# Create knowledge: Doc -> Knowledge
# result: {doc_id: str}

# 2. update
result = kb.update(path = "/file_path")
# Update knowledge

# 3. query
result = kb.query(query = "what's the weather like in shanghai", optimition="")
# Query input

# 4. config
config = {stratege="Summary"}
kb.config(config)
# 1. choose stratege: "RawImage": Option1; "Summary": Option2; "Complex": Option3;
```

```bash
$ python -m aiki
#or
$ aiki
```

## Development

Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
