# Custom RAGAS Experiments

## Setup

**Step 1:** Clone your RAGAS implementation
```
cd packages
git clone --branch ragas-mipt https://github.com/ti3c2/ragas
cd ..
```

**Step 2:** Install dependencies with uv
```
uv sync
```

**Step 3:** Import RAGAS in your code
```
from ragas.llms import LangchainLLMWrapper
from ragas.embeddings import LangchainEmbeddingsWrapper
from ragas.testset.graph import KnowledgeGraph, Node, NodeType
# ...etc
```

**Step 4:** Adding your changes to RAGAS and syncing

1. Edit code in ./ragas folder or pull it with the following commands

```
# For reinstalling after remote changes
cd packages/ragas
git pull origin ragas-mipt
cd ../../
```

2. Rebuild the project `uv add ragas --reinstall`
